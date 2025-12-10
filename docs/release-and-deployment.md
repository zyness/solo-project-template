# Release & Deployment Guide

## Purpose
Standardize how I release features to production. The goal is **automation** and **safety**—making deployments boring and repeatable so I can focus on coding.

## Release Strategy
- **Continuous Delivery:** The goal is to have the `main` branch always in a deployable state.
- **Semantic Versioning (SemVer):**
  - **Patch (v1.0.x):** Bug fixes. Safe to deploy immediately.
  - **Minor (v1.x.0):** New features (backward compatible). Requires a quick manual check.
  - **Major (vx.0.0):** Breaking changes. Requires database migration planning or downtime.

## Pre-release Requirements (Automated Gatekeepers)
Before merging to `main` (which triggers deployment):
- [ ] **CI Pass:** All automated tests and linting checks are green.
- [ ] **Local Build:** Ran the "build" command locally to ensure no compilation errors occur that dev-mode missed.
- **Database:** If the schema changed, are migration scripts ready?

## Deployment Checklist (The "DevOps Hat")
- [ ] **Backup:** If this is a major update, is the database backed up?
- [ ] **Merge:** Merge Pull Request to `main`.
- [ ] **Monitor:** Watch the CI/CD pipeline (e.g., GitHub Actions) until "Success".
- [ ] **Smoke Test:** Open the live production URL. Does it load? Can I log in? (Don't trust the green checkmark blindly).
- [ ] **Changelog:** Update `CHANGELOG.md` or Release Notes.

## Rollback & Incident Playbook (Panic Button)
If a deployment breaks production:
1.  **Don't Panic:** I am the only user (or have very few).
2.  **Revert:**
    - *Option A (Hosting Provider):* Use the "Rollback" button in the dashboard (Vercel/Netlify/Heroku).
    - *Option B (Git):* `git revert HEAD` -> Push.
3.  **Fix Forward:** Only try to fix the bug in production if it's a one-line config change. Otherwise, revert first, fix locally, then redeploy.

## Release Notes Template (Simple)
To keep track of what I did (future me will thank me):
- **Version:**
- **Date:**
- **What's New:** (Bullet points of features)
- **Fixes:** (Bugs squashed)
- **Database Changes:** (Did I alter tables?)