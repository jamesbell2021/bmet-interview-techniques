# Anchorlight Games — Design Interview Simulator

A browser-based mock interview for a junior game-design role. Students play as a candidate meeting **Priya Osei**, a lead designer at the fictional studio Anchorlight Games, and answer six interview questions by picking between three responses — one weak, one adequate, one strong.

**Play it live:** https://jamesbell2021.github.io/bmet-interview-techniques/

Built for the **B1 (Year 2) unit of the Level 3 Creative Media — Computer Games Development** course at Belfast Met, to support the interview-technique and professional-practice element of the unit.

## What it covers

Each of the six questions targets a specific employability skill, and every answer is followed by a short explanation of *why* it scored the way it did:

| # | Question focus | Skill assessed |
|---|---|---|
| 1 | "Walk me through your background" | Communication & structure (the pitch: hook, evidence, relevance) |
| 2 | "Tell me about a system or level you designed" | Design craft (reasoning over results) |
| 3 | "Tell me about a time you got blunt feedback" | Resilience & coachability (STAR method under pressure) |
| 4 | "How do you run playtests?" | Playtesting method (silent observation vs. asking friends) |
| 5 | "Pick a game you admire — what would you change?" | Critique & design literacy (mechanism + trade-off) |
| 6 | "An engineer says your feature is too expensive to build" | Collaboration (protecting intent, not implementation) |

At the end, students get an S/A/B/C rank, a per-skill breakdown, an answer-by-answer log explaining every choice, and a "loadout" checklist (STAR stories, a reversed decision, a two-minute critique, two questions to ask the interviewer) to take into a real interview.

## Using it in class

A suggested structure for a session:

1. **Cold run (10–15 min).** Students play through individually without discussion, so their first pass reflects instinct rather than the "correct" answer.
2. **Compare ranks (10 min).** In pairs or small groups, compare ranks and talk through *why* an answer was marked weak, adequate, or strong — the in-game notes give them the vocabulary to do this without you re-explaining each point.
3. **Apply it (remaining time).** Have students draft their own STAR story, playtest description, or game critique using the same structure the tool rewards, ready for a real mock interview or portfolio review.

It works well as a warm-up before a live mock-interview exercise, or as independent study before an assessment on professional practice.

## Running it

No installation, build step, or server required — it's a single self-contained HTML file.

- **Online:** use the GitHub Pages link above.
- **Offline / on a classroom machine with no internet:** download [`index.html`](index.html) and open it in any modern browser.

## Customising the questions

All content lives in the `QUESTIONS` array near the top of the `<script>` block in `index.html` — each question has a `skill`, a `prompt`, a `theory` explainer, and three `options` (`weak` / `adequate` / `strong`) with their own `text` and feedback `note`. Edit that array directly to retarget the questions at a different unit, role, or specialism (e.g. narrative design, UX, production) — no build tooling is needed, just save and reload the file.

## Tech notes

Plain HTML, CSS, and vanilla JavaScript — no frameworks, no dependencies, nothing to install. Portraits and icons are inline SVG; sound effects are generated with the Web Audio API. Respects `prefers-reduced-motion`.

---

🤖 Built with [Claude Code](https://claude.com/claude-code)
