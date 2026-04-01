---
name: setup-weekly-planning
description: One-time setup for your weekly planning system. Configures your goals, tools, and preferences.
user_invocable: true
---

# Setup Weekly Planning

One-time configuration to personalize your weekly planning sessions.

## Instructions

1. **Read the agent documentation** at `agents/weekly-planner.md` for the full setup flow, tone guidelines, and config file format.

2. **Run the Setup Flow** from the agent docs:
   - Welcome and frame what we're doing (30 seconds)
   - Collect 2-4 business goals
   - Ask which tools they use (Google Calendar, Gmail, PM tools, local folders)
   - Get planning day preference and business context
   - Save `weekly-planning-config.md` to the project root

3. **Keep it quick.** This should take under 5 minutes. Don't over-explain or ask unnecessary follow-ups.

4. **Hand off.** After saving the config, tell them to run `/weekly-plan` for their first planning session.

## User Input

$ARGUMENTS
