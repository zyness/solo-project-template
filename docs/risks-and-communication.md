# Risks & Decision Logging

## Purpose
To manage the specific risks of a one-person project and ensure "Future Me" understands why "Past Me" made certain decisions.

## Top Risks for Solo Devs (The "Bus Factor of 1")
In a solo project, **I am the single point of failure**.
- **Risk:** **Loss of Motivation / Time.**
  - *Mitigation:* Keep tasks small. Use the "Project Initiation" checklist to ensure I have time.
- **Risk:** **Memory Loss.** (Forgetting how the code works after a 2-month break).
  - *Mitigation:* Aggressive commenting in code and updating `docs/` immediately.
- **Risk:** **Technical Rabbit Holes.** (Getting stuck on a non-essential problem for days).
  - *Mitigation:* Strict Timeboxing. If a task takes >4 hours unexpectedly, stop and re-evaluate.

## Risk Tracking (Lightweight)
Instead of a complex table, I use a **`RISKS.md`** file or a label `Type: Risk` in GitHub Issues for:
- External dependencies that might break (APIs).
- Hacky code I wrote that needs refactoring later (Technical Debt).

## Communication = Decision Logging (ADRs)
Since I don't have a team to discuss architecture with, I must write down significant decisions to prevent changing my mind in circles.

### The Decision Log (Architecture Decision Records)
When I choose a major technology (e.g., "Use Firebase instead of SQL") or a pattern, I write a quick note in `docs/decisions/` or an Issue:
- **Context:** Why did I need to choose?
- **Decision:** What did I pick?
- **Alternatives:** What did I reject and why?
- **Consequences:** What is the trade-off? (e.g., "Faster dev speed, but vendor lock-in").

## "Escalation" Path (Getting Unstuck)
Since I cannot escalate to a manager, I follow this process when blocked:
1.  **Timebox:** Struggle for max 1 hour.
2.  **Research:** Read docs / StackOverflow.
3.  **Ask AI:** Use Copilot / ChatGPT to explain the error or suggest alternatives.
4.  **Pivot:** If still stuck, can I simplify the feature or remove it for the MVP?
5.  **Sleep:** Stop coding. The solution usually comes the next morning.

## Incident "Communication"
If the live app breaks:
1.  **Fix it.**
2.  **Write a Post-Mortem note:** Why did it break? (e.g., "Forgot to set env variable").
3.  **Prevent:** Add a check to the `deployment-checklist.md` so it doesn't happen again.