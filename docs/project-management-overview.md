# Project Management Overview

## Purpose
Provide a structured approach for managing this solo project to maintain focus, quality, and consistency. This document serves as the "Rulebook" for myself and context for GitHub Copilot.

## Scope
Applies to the entire lifecycle of the project, from idea validation to release and maintenance.

## Principles
- **User-Centric:** Even if I am the only user, build as if it’s for a customer.
- **Iterative Delivery:** Ship small, working increments. Avoid "Big Bang" releases.
- **Role Separation ("Wearing Hats"):** Consciously switch between managing the product and writing code. Don't plan while coding.
- **Documentation as Code:** If it's not written down in `docs/` or Issues, it doesn't exist.
- **Sustainable Pace:** Avoid burnout. Automate repetitive tasks (CI/CD, Templates).

## Core Roles (The "Hats" I Wear)
Since this is a one-person project, I switch between these modes:
- **Product Owner Mode:** Defines *what* to build and *why*. Prioritizes the backlog.
- **Project Manager Mode:** Defines *when* things happen. Manages time and scope.
- **Developer Mode:** Focuses on the implementation details and code quality.
- **QA/User Mode:** Validates if the feature actually works and solves the problem.

## Key Artifacts
- **Project One-pager:** The north star for the project (Goal & Scope).
- **Backlog:** The list of tasks (Issues in GitHub).
- **Decision Log:** Records of major technical choices (e.g., "Why I chose Database X over Y").
- **Definition of Done:** The checklist that prevents me from shipping broken code.

## Lifecycle (High-Level)
1. **Initiation:** Idea validation. Is this worth building? (See `project-initiation.md`)
2. **Planning:** Breaking the idea into small, actionable Issues. (See `project-planning.md`)
3. **Execution:** The "Deep Work" phase. Coding and testing. (See `execution-and-tracking.md`)
4. **Release:** Automated deployment and verification.
5. **Retrospective:** Brief reflection on what went well or what tool needs changing.

## How to use these docs with Copilot
- This folder (`docs/`) is the source of truth for the **Copilot Space**.
- When asking Copilot to help with planning, reference the **Product Owner** role.
- When asking Copilot to help with code, reference the **Developer** role.
- Copilot uses these docs to ensure new Issues and PRs follow the established structure.