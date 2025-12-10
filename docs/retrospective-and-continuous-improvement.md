# Retrospective & Continuous Improvement

## Purpose
To pause and reflect on my personal workflow. The goal is to identify bad habits (e.g., over-engineering, procrastination, rabbit holes) and fix them before the next milestone.

## When
- **Post-Milestone:** After shipping a major feature or finishing a "Sprint".
- **Post-Incident:** After breaking something badly or losing significant time on a bug.
- **Panic Check:** When I feel overwhelmed or stuck.

## The "Solo Retro" Format (15 Minutes max)
Since I have no team to talk to, I answer these questions honestly (e.g., in a dedicated issue or a private note):

### 1. What went well? (Keep doing this)
- Did the tech stack behave as expected?
- Did I estimate the effort correctly?
- When was I in the "Flow" state?

### 2. What slowed me down? (Stop doing this)
- **Distractions:** Did I spend 4 hours on CSS styling before the logic worked?
- **Rabbit Holes:** Did I try to build a custom solution when a library existed?
- **Scope Creep:** Did I build features that weren't in the plan?
- **Tooling:** Is my local environment fighting me?

### 3. Action Items (Change this)
- Create max **1-2 specific actions**. Don't create a laundry list.
- *Bad Action:* "Code faster."
- *Good Action:* "Next time, write the SQL schema on paper before coding the migration."
- *Good Action:* "Automate the deployment script because I keep forgetting the arguments."

## Tracking Improvements
- If it's a code task: Create a **"Chore"** or **"Tooling"** issue in the backlog immediately.
- If it's a process change: Update these `docs/` immediately (e.g., add a step to the Deployment Checklist).

## Continuous Improvement Philosophy
- **Don't blame yourself:** Bugs happen. Bad estimates happen.
- **Fix the system:** If I make the same mistake twice, create a checklist or script to prevent it the third time.