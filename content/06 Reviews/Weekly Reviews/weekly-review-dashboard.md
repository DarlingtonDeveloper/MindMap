---
title: Weekly Review Dashboard
created: 2025-04-21
tags: [weekly-review, dashboard]
---

# 📊 Weekly Review Dashboard

```dataview
TABLE 
  file.link AS "Week",
  file.ctime AS "Created",
  length(filter(split(text, "- [ ]"), (t) => contains(t, "📌"))) + "/" + 
  (length(filter(split(text, "- [ ]"), (t) => contains(t, "📌"))) + length(filter(split(text, "- [x]"), (t) => contains(t, "📌")))) AS "Tasks (Incomplete/Total)"
FROM "content/06 Reviews/Weekly Reviews"
WHERE file.name != "weekly-review-dashboard"
SORT file.name DESC
```



