# Roles & Personas (The "Hats" I Wear)

## Purpose
In a one-person project, trying to do everything at once leads to chaos. This document defines the specific **"Modes of Thinking"** (Hats) I must consciously switch between to ensure I don't just write code, but actually ship a product.

---

## 🎩 The Product Manager Hat (The "Why")

### Role Summary
Combines the roles of Product Manager, Project Manager, and Business Analyst. When wearing this hat, I am **not allowed to write code**.

### Responsibilities
- **Ruthless Prioritization:** Deciding what NOT to build (Scope Hammer).
- **The "Why":** Defining the problem before looking for a solution.
- **Backlog Grooming:** Breaking big ideas into small, actionable GitHub Issues.
- **Time Management:** Deciding if a feature is worth the time investment.

### When to wear this hat
- Before starting a new Milestone.
- When a feature takes longer than expected (to decide if we cut scope).
- **Trigger:** "I'm feeling overwhelmed." -> Switch to PM mode and re-plan.

---

## 🎩 The Developer Hat (The "How")

### Role Summary
The executor. When wearing this hat, I trust the decisions made by the "Product Manager" and focus purely on implementation quality.

### Responsibilities
- **Implementation:** Writing clean, maintainable code.
- **Tests:** Writing unit tests for my own logic.
- **Refactoring:** Keeping technical debt low.

### The "No-Design" Rule
- When in Developer Mode, do not invent UI designs. Implement what was decided or sketch it first.
- Do not question the "Why" (that's the PM's job). Just build it well.

---

## 🎩 The UX/UI Designer Hat (The "Feel")

### Role Summary
Focuses on usability and visuals. Logic doesn't matter here, only the experience.

### Responsibilities
- **Sketching:** Drawing screens on paper/iPad before coding HTML/CSS.
- **User Flow:** Ensuring the button placement makes sense.
- **Design System:** Picking colors and fonts so I don't have to choose every time.

### When to wear this hat
- **Before** the Developer Hat. Never design CSS while writing React/Python logic.

---

## 🎩 The DevOps & QA Hat (The "Safety Net")

### Role Summary
Combines DevOps Engineer and QA Lead. This is the pessimistic mode that assumes everything is broken.

### Responsibilities
- **Pipeline:** Ensuring `git push` triggers tests and deployment automatically.
- **Testing:** Clicking through the app trying to break it (Edge Cases).
- **Security:** Checking for committed keys or open ports.
- **Release:** Monitoring the deployment and verifying it works in production.

---

## 🤖 The Stakeholder (The User / Copilot)

### Role Summary
The ultimate judge. Since I have no real users yet, **GitHub Copilot** or a **Trusted Friend** can simulate this role.

### How to use Copilot for these roles
Since I am alone, I use Copilot Spaces to simulate the team members I don't have:

- **"Act as the QA Lead:"** Ask Copilot to find edge cases in my code.
- **"Act as the Product Manager:"** Ask Copilot to critique my backlog or suggest missing features.
- **"Act as the Security Engineer:"** Ask Copilot to review a file for vulnerabilities.