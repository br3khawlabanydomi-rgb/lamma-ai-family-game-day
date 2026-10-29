# LAMMA AI — Family AI Game Day

A five-game, bilingual (English/Arabic), offline-first family game website for the Abu Dhabi University Cycle 2 competition.

## Start in under a minute
1. Extract the ZIP (do not run directly inside the compressed archive).
2. Open `index.html` in Chrome or Microsoft Edge. No installation, account, internet connection, or API key is required for the packaged content.
3. Register players, select teams and a host, choose a game, and follow on-screen controls.
4. To run via a local web server instead: `python -m http.server 8000`, then open `http://localhost:8000`.

## Five games
- Football Fusion: teams, timer, human-entered goals, AI-assisted tactical prompts.
- Pearl Quest: expedition decisions and resource tradeoffs.
- Falcon Flight: route choices and energy planning.
- Souq Masters: market and budget decisions.
- Oasis Builders: cooperative sustainability and resource allocation.

## AI disclosure
The included scenarios are **pre-generated AI-assisted content**, stored locally. **There is no live AI model or API call** in this build. The human host confirms outcomes. Review scenarios for cultural and age appropriateness before public use.

## Files
- `index.html` — complete runnable HTML/CSS/JS application (the authoritative source).
- `source/README.md` — explains where the source code lives.
- `assets/README.md` — explains embedded assets and offline behavior.
- `tests/` — executable tests and recorded results.
- `documentation/TEST_REPORT.md` — earlier QA status; `documentation/RETEST_2026-10-29.md` — packaging retest and Souq budget fix.
- `documentation/PUBLISH_AND_VERIFY.md` — GitHub Pages deployment and verification.
- `documentation/FINAL_ACCEPTANCE_CHECKLIST.md` — manual acceptance tests.

## Automated tests
Requires Node.js 18+ for the JS harness: `node tests/run_vm.js` (from the extracted project root). The recorded test evidence is in `tests/evidence/`. The packaging retest passed 10 simulated JavaScript/DOM groups; this does not prove physical browser clicks, touch layout, accessibility, or true timer passage.

## Data, safety, and limits
Use nicknames rather than children's full names. Game state is stored locally in the browser; clearing site data can erase it. Do not place private student information or API keys in this public folder. No backend or remote database is included. Review the included test report for outstanding verification items.

## Publishing
See `documentation/PUBLISH_AND_VERIFY.md`. A hosted URL has **not** been created or verified by this ZIP package.
