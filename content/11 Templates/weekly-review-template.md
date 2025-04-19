<%*
const fileName = tp.date.now("YYYY-MM-DD");
await tp.file.rename(fileName);

const reviewFolder = "content/06 Reviews/Weekly Reviews";
const files = app.vault.getFiles()
  .filter(f => f.path.startsWith(reviewFolder) && f.name.endsWith(".md") && f.basename !== fileName)
  .sort((a, b) => b.basename.localeCompare(a.basename)); // latest first

const lastReview = files[files.length - 1];
let previousTasks = "No tasks found.";
let lastFileName = "N/A";

if (lastReview) {
  const content = await app.vault.read(lastReview);
  lastFileName = lastReview.basename;

  const match = content.match(/##\s*📌\s*Next Week Priorities[\s\S]*?(?=\n## |\n# |$)/i);
  if (match) {
    previousTasks = match[0].replace(/##\s*📌\s*Next Week Priorities/i, "").trim();
  }
}

const now = new Date();
const weekNumber = Math.ceil((((now - new Date(now.getFullYear(), 0, 1)) / 86400000) + now.getDay() + 1) / 7);
const isoWeek = now.getFullYear() + "-W" + String(weekNumber).padStart(2, '0');

tR += `---
title: Weekly Review - ${fileName}
created: ${fileName}
tags: [weekly-review, observer, system-sync]
review: true
week: ${isoWeek}
---

# 🌿 Weekly Review

## ⏪ Previous Week's Focus (from [[${lastFileName}]])
${previousTasks}

## ✅ Highlights
- 

## 🚫 Lowlights
- 

## 🎯 Alignment Check
- [ ] Aligned with mission?
- [ ] Deep work time protected?
- [ ] Feeling states: Aligned / Flow / Energized?

## 🌱 Sprout Log
| Date       | Task/Goal              | Duration | Outcome | Focus (1-5) |
|------------|------------------------|----------|---------|-------------|
| ${fileName} |  |  |  |  |

## 📊 Metrics
- Deep Work Hours: 
- Distractions Logged: 
- Rituals Completed: 
- Physical Activity: 
- Sleep Quality: 

## 🧠 Insight of the Week
> 

## 🔁 Observer Feedback Loop
- [ ] Add/remove rituals?
- [ ] Adjust goals?
- [ ] Add to long-term backlog?

## 📌 Next Week Priorities
- [ ] 
- [ ] 
- [ ] 
`
%>
