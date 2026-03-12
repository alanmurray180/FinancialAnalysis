# CLAUDE.md

This file provides guidance to AI assistants working on the FinancialAnalysis repository.
Keep this file updated as the project evolves.

---

## Project Overview

**Repository:** alanmurray180/FinancialAnalysis
**Status:** Initial setup phase — no source code, build system, or CI/CD pipeline exists yet.
**Purpose:** Financial analysis tooling. Specifics (data sources, asset classes, output formats) are to be defined as the project develops.
**Last updated:** 2026-03-12

---

## Repository Structure

The repository currently contains only this guidance file. Update this section as files are added.

```
FinancialAnalysis/
└── CLAUDE.md          # This file — guidance for AI assistants
```

When source code is added, document the layout here. Example future structure:

```
FinancialAnalysis/
├── CLAUDE.md
├── src/               # Application source code
├── tests/             # Test suite
├── data/              # Sample or fixture data (never real financial data)
├── docs/              # Documentation
└── README.md
```

---

## Tech Stack

No tech stack has been chosen yet. Before writing any code:

1. **Ask the user** about their preferred language and framework.
2. Common choices for financial analysis projects:
   - **Python** — pandas, numpy, scipy, matplotlib/plotly, yfinance, zipline, backtrader
   - **TypeScript/Node.js** — suitable for API services or dashboards
   - **R** — strong statistical and finance-specific libraries
3. Record the decision here once made and update the Development Setup section.

---

## Development Setup

_To be documented once language, framework, and tooling are established._

### Prerequisites

- TBD

### Installation

- TBD

### Running the Project

- TBD

---

## Build & Test

_No build system or test framework is configured yet._

### Build Commands

- TBD

### Test Commands

- TBD

### Linting / Formatting

- TBD

---

## Key Conventions

### Commit Messages

- Use imperative mood: "Add portfolio loader" not "Added portfolio loader"
- Keep the subject line under 72 characters
- Reference issue numbers where applicable: "Fix date parsing (#12)"

### Branch Naming

- Features: `feature/<short-description>` (e.g., `feature/portfolio-analysis`)
- Bug fixes: `fix/<short-description>` (e.g., `fix/date-parsing`)
- Chores/housekeeping: `chore/<short-description>`
- AI-assisted branches follow the pattern: `claude/<session-id>`

### Code Style

- Follow the conventions established by the project linter/formatter once configured.
- For Python: prefer `black` + `ruff`; for JS/TS: prefer `prettier` + `eslint`.

### Data Handling

- **Never commit real financial data, API keys, or credentials** to the repository.
- Use environment variables or a secrets manager for API keys.
- Add a `.gitignore` entry for any `.env` files and data directories containing real data.
- Use anonymised or synthetic fixtures in the test suite.

### Documentation

- Keep this CLAUDE.md updated whenever project structure, tooling, or workflow changes occur.
- Add a `README.md` once there is something meaningful to document for end users.

---

## Git Workflow

1. **Create a branch** from `master` for every change.
2. **Commit early and often** with descriptive messages.
3. **Push** to the remote branch and open a pull request for review.
4. **Never force-push** to `master`.

### AI-Assisted Development Branch

When Claude Code operates on this repository it targets the branch:
`claude/claude-md-mmnes6xq6ekojh50-Kjcpt`

All Claude-generated changes should be committed and pushed to that branch before a PR is opened against `master`.

---

## Notes for AI Assistants

- **No existing code exists.** Do not assume or invent a tech stack — ask the user first.
- **Update CLAUDE.md** whenever significant changes to structure, tooling, or workflow are introduced.
- **Security first:** never include real API keys, credentials, or personally identifiable financial data.
- **Keep changes focused:** avoid introducing unnecessary dependencies or over-engineering solutions.
- **Financial domain awareness:** be mindful of precision requirements (use `Decimal` not `float` for monetary values in Python), timezone handling for market hours, and the difference between price data and return data.
- When adding dependencies for the first time, document them here and explain why they were chosen.
- If you discover that CLAUDE.md is out of date with the actual codebase, update it as part of your task.
