# Sprout System – Prioritized To-Do List

## Top Priorities (High ROI / Low Friction)

### 1. [Sprout Core] Build Daily Ritual Tracker + Logging
- [ ] Create popup system for rituals (stretch, hydrate, look away)
- [ ] Store logs in local JSON or Supabase
- [ ] Track streaks and missed days
- [ ] Add plant “watering” logic based on completed rituals  
**Impact**: 9/10 – unlocks gamified flow  
**Ease**: Medium

---

### 2. [Historian] Build Dev Journal Automation Script
- [ ] Pull last 7 days of Git commits
- [ ] Pull VS Code session metadata (basic logging)
- [ ] Parse Obsidian `#devlog` notes
- [ ] Use GPT to auto-generate weekly summary  
**Impact**: 8/10 – fuels your public build logs  
**Ease**: High

---

### 3. [Connector] Design Social Relationship Tracker
- [ ] Create schema for tracking contact frequency + sentiment
- [ ] Manually log ~10 close contacts with last message date
- [ ] Create GPT prompt: “Who should I reconnect with this week?”  
**Impact**: 7/10 – increases depth of connection  
**Ease**: Medium

---

## Secondary Priorities (Medium/Longer-Term)

### 4. [Sprout Core] Add Browser Distraction Monitor
- [ ] Explore browser API (or Arc browser tracking)
- [ ] Log tab switches or high-time sites to Supabase
- [ ] Trigger nudges based on rules (e.g. "Reddit > 15min")  
**Impact**: 9/10  
**Ease**: Medium-Low

---

### 5. [Fueler/Mover] Build Voice Log to Context Pipeline
- [ ] Shortcut that lets you record a voice memo about meals/exercise
- [ ] Transcribe using Whisper or notes field
- [ ] Store structured summary in JSON or Supabase  
**Impact**: 7/10  
**Ease**: Medium

---

### 6. [Observer] Generate Weekly Life Report
- [ ] Pull logs from Sprout, Ritualist, Fueler, Connector
- [ ] Create prompt: “Summarize my week and alignment with goals”
- [ ] Output a reflection + theme of the week + 1 challenge  
**Impact**: 10/10 – ties system together  
**Ease**: Medium-Hard

---

## Foundational / Support Work

### 7. [Infrastructure] MCP Context Layer for Historian
- [ ] Fork GitHub’s MCP server
- [ ] Build `git-logs` and `obsidian-logs` providers
- [ ] Make test query from GPT using MCP-style prompt  
**Impact**: 6/10 (long-term scalability)  
**Ease**: Low

---

### 8. [Task System] Deploy Kanban Dashboard (Planka or Obsidian Enhanced)
- [ ] Choose: Planka (host at tasks.darlington.dev) or Obsidian + Kanban Plugin
- [ ] Set up columns by agent (Sprout, Connector, Fueler, etc.)
- [ ] Add priority scoring system  
**Impact**: 8/10  
**Ease**: High

---

## TL;DR: Top 3 to Start This Week
- Build daily ritual tracker with plant logic (Sprout Core)
- Script Dev Journal → Quartz auto-publish (Historian)
- Log core social connections and generate GPT check-in prompt (Connector)