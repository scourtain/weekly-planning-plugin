---
name: weekly-plan
description: Run your weekly planning session. Pulls your calendar, checks projects, brain dumps, and builds a goal-aligned weekly plan.
user_invocable: true
---

# Weekly Plan

Run a structured weekly planning session that connects your week to your bigger goals.

## Instructions

1. **Read the agent documentation** at `agents/weekly-planner.md` for the full workflow, tone guidelines, and output format.

2. **Load configuration** by reading `weekly-planning-config.md` from the project root. If it doesn't exist, tell the user to run `/setup-weekly-planning` first and stop.

3. **Execute the Main Weekly Planning Workflow** from the agent docs:
   - **Phase 2: Automated Pulls** - Pull calendar, email, and project data BEFORE asking the user anything. Present a briefing of what you found.
   - **Phase 3: Brain Dump** - Ask the user what else is on their mind. Accept freeform input.
   - **Phase 4: Synthesize** - Merge automated pulls with brain dump. Deduplicate and categorize.
   - **Phase 5: Priority Alignment** - Map priorities to stored goals. Challenge items with no goal connection (kindly, once, then accept their answer).
   - **Phase 6: Weekly Brief** - Produce the structured weekly plan. Ask if it feels right. Adjust and save.

4. **Follow the rules:**
   - Do automated pulls FIRST, before asking the user anything
   - Brain dump comes AFTER the briefing
   - One challenge per unaligned item, then accept
   - Keep the session to 15-20 minutes
   - Skip any tool that isn't configured or fails to connect

## User Input

$ARGUMENTS
