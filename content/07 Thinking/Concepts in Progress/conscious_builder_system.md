
# Conscious Builder System

## Overview

A 3-layer personal operating system to align long-term vision with daily action, specifically designed for developers, creatives, and founders. The system helps you define who you're becoming, break down your goals into sprints, and execute them intentionally day by day.

---

## System Layers

### 1. North Star Navigator (Vision Layer)

**Purpose**: Define long-term vision, values, and quarterly goals.

**Cadence**: Yearly → Quarterly → Monthly

**Features**:
- North Star Statement
- Life Principles and Core Values
- Life Domains (Health, Work, Relationships, etc.)
- 1-Year Goals per Domain
- Quarterly Reflection Workflow
- Vision Timeline
- Syncs Goals to Sprint Planner

**Data Exported to Planner**:
```json
{ "goalId": "", "title": "", "domain": "", "why": "", "deadline": "" }
```

---

### 2. Sprint Planner (Mid-Term Focus Layer)

**Purpose**: Break long-term goals into trackable weekly sprints and tasks.

**Cadence**: Monthly → Weekly

**Features**:
- Kanban-style goal/task breakdown
- Weekly Sprint Planning
- Task alignment with Navigator goals
- Weekly Review and Progress Reflection

**Data Exported to Daily System**:
```json
{ "taskId": "", "goalId": "", "domain": "", "priority": "", "plannedDate": "" }
```

**Data Received from Daily System**:
```json
{ "taskId": "", "date": "", "timeSpent": "", "focusRating": "", "notes": "" }
```

---

### 3. Daily System (Execution Layer)

**Purpose**: Set daily intentions and execute tasks with focus.

**Cadence**: Daily

**Features**:
- Morning Intention Prompt
- Deep Work Dashboard (Pomodoro, music, session tracking)
- Task Execution and Distraction Logging
- Evening Reflection

**Data Returned to Planner**:
- Session logs, reflection, time on task

---

## Data Flow Summary

### Top-Down (Intention Flow):
- **Navigator → Planner → Daily System**
- Long-term goals shape weekly focus and daily tasks

### Bottom-Up (Feedback Loop):
- **Daily System → Planner → Navigator**
- Task data and reflections roll up into sprint progress and domain alignment

---

## Technical Architecture (Suggested)

- Shared Supabase backend with tables:
  - `users`, `domains`, `goals`, `tasks`, `sessions`, `reflections`
- Clear foreign keys to connect layers
- Optionally, a local-first model with ElectricSQL or IndexedDB

---

## Suggested Domain Examples

- Health & Fitness
- Work & Career
- Relationships
- Personal Growth
- Finances & Freedom
- Creativity & Expression
- Spirituality / Meaning
- Environment & Lifestyle

---

## Future Ideas

- Vision Wordcloud
- Drift Detection Alerts
- GitHub / Calendar / Health sync
- Template Sharing via System Builder Toolkit
