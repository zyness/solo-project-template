# Execution & Tracking Guidelines

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones for a single-developer workflow.

## Workflows
- **Project Board:** Use a simplified board (e.g., GitHub Projects) with columns: 
  - *Backlog* (Ideas/Future)
  - *Ready* (Specified & Planned)
  - *In Progress* (Active Coding)
  - *Done* (Merged & Verified)
- **Pull Request (PR) Workflow:**
  - Even working solo, use branches and PRs to keep `main` clean and stable.
  - Keep PRs focused on a single task or issue.
  - **Self-Review:** Before merging, review your own code in the GitHub UI. Look for debugging statements, TODOs, or logic errors as if reviewing a stranger's code.
  - Ensure CI (automated tests) passes before merging.

## Quality & Testing
- **Unit tests:** For core business logic and complex algorithms.
- **Integration tests:** Ensure database and API connections work.
- **Security:** Do not commit secrets (API keys, .env). Use GitHub Secret Scanning.
- **Manual QA:** Test the feature in the browser/app exactly as a user would before moving the ticket to "Done".

## Reporting & Metrics
- **Milestone Progress:** Check progress against the goals defined in the Project One-pager.
- **Signals:** Monitor build times and error logs.

## Execution Checklist (The "Multiple Hats" Check)
Before moving an item to **Done**, ensure:
- [ ] **Dev Hat:** Code is clean, commented where necessary, and tests pass locally.
- [ ] **Reviewer Hat:** PR diff has been self-reviewed; no accidental files included.
- [ ] **Designer Hat:** UI/UX matches the intended design and is responsive.
- [ ] **Product Hat:** The implementation actually solves the problem described in the Issue.
- [ ] **Docs Hat:** README or documentation updated if the feature changed how things work.