# Weekly Planning Plugin for Claude

A structured weekly planning system that connects your tasks to your bigger business goals. Not just a to-do list - a thinking partner that helps you stay focused on what actually moves the needle.

## What It Does

**`/setup-weekly-planning`** (run once)
- Captures your 2-4 most important business goals
- Notes which tools you want to connect (Google Calendar, Gmail, project management)
- Saves your preferences so every planning session is personalized

**`/weekly-plan`** (run weekly)
- Pulls your upcoming calendar, flagging heavy and open days
- Scans emails for items needing follow-up (if connected)
- Checks your project management tool or folders for active work
- Gives you space for a brain dump
- Maps every priority to your goals - and kindly calls out when something doesn't align
- Produces a clean weekly brief with priorities, commitments, and a Monday starter

## Installation

1. In Claude, go to **Customize** then **Personal Plugins**
2. Add this plugin from GitHub using the repo URL
3. Run `/setup-weekly-planning` to configure your goals and tools (takes ~5 minutes)
4. Run `/weekly-plan` each week

Works great as a scheduled Co-Work task on your planning day (Sunday evening or Monday morning).

## What You Can Connect

All integrations are optional. The plugin works with just a brain dump and your goals, but gets better with more context:

| Tool | What It Pulls |
|------|--------------|
| Google Calendar | Events for the upcoming week |
| Gmail | Recent emails that may need follow-up |
| Asana, Monday, Linear, Trello, ClickUp | Tasks due, overdue, or in progress |
| Local project folders | Recently modified files and active work |

## Updating Your Setup

Your configuration lives in `weekly-planning-config.md` at your project root. Open it anytime to:
- Update your goals as priorities shift
- Add or remove tool connections
- Change your planning day

## Files

```
weekly-planning-plugin/
├── README.md                    # You're here
├── setup-weekly-planning/
│   └── SKILL.md                 # Setup skill (run once)
├── weekly-plan/
│   └── SKILL.md                 # Weekly planning skill (run regularly)
└── agents/
    └── weekly-planner.md        # Detailed workflow instructions
```

---

Want to connect your weekly rhythm to bigger quarterly strategy? Check out the **Seasonal Planning Plugin** - it helps you set seasonal goals that your weekly plans build toward.
