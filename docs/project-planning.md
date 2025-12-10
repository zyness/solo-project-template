# Project Planning Guide

## Purpose
Turn the idea (from Initiation) into a concrete list of tasks (Backlog) so I can start coding without getting lost.

## Objectives
- **Decompose:** Break big features into small, manageable Issues (1-4 hours of work).
- **Prioritize:** Decide what is essential for the MVP (Minimum Viable Product).
- **Dependency Check:** Identify external APIs or libraries needed before starting.

## Activities (The Planning Session)
1. **Backlog Creation:** create Issues in GitHub for every feature.
2. **Prioritization:** Label Issues as `Must Have`, `Should Have`, `Nice to Have`.
3. **Estimation:** roughly estimate if a task is "Small" (an evening), "Medium" (a weekend), or "Large" (needs breaking down).
4. **Milestone Mapping:** Group Issues into Milestones (e.g., "v0.1 - Authentication", "v0.2 - Core Logic").

## Backlog Item Template (for GitHub Issues)
- **Title:** Action-oriented (e.g., "Implement Login Page").
- **Description:** What needs to happen?
- **Acceptance Criteria:** "It is done when..." (Crucial to stop endless polishing).
- **Technical Notes:** Rough idea of the implementation (libraries, algorithms).
- **Estimate:** S / M / L.

## Work Mode: Milestones over Sprints
Since I work alone, strict 2-week sprints can be artificial. Instead, focus on **Milestones**:
- Focus on completing one Milestone at a time.
- Limit "In Progress" work to 1 item to maintain flow.
- Review progress weekly: "Did I move closer to the Milestone?"

## Risk & Technical Debt Management
- **Risks:** If I'm unsure how a technology works, create a "Spike" (Research Task) before the actual implementation task.
- **Dependencies:** Check if libraries are maintained before choosing them.

## Planning Checklist (The "Hats" Check)
Before writing the first line of code for a Milestone:
- [ ] **PM Hat:** Is the Backlog prioritized? Do I know what the MVP is?
- [ ] **Designer Hat:** Do I have rough sketches/wireframes? (Don't design in CSS).
- [ ] **Architect Hat:** Do I have a rough idea of the Data Model / Database Schema?
- [ ] **DevOps Hat:** Do I know where I will host this? Is the repo set up?
- [ ] **QA Hat:** Is the Definition of Done clear?