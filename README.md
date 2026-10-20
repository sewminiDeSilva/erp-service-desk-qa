# ERP IT Support & Service Desk: QA Portfolio Project

A learning project to build an IT Support & ERP Service Desk system while practising professional QA engineering: requirements analysis, test design, API and UI automation, CI/CD, and evidence-based release decisions.

> **Status: Phase 1 complete (environment and repository foundations). No application code yet.**

## Goal
ERP users report software, hardware, access and other IT problems through a ticket portal. IT support triages, assigns and resolves them, with a controlled QA stage for software fixes.

## Planned stack (not all installed yet)
React + TypeScript, Node.js + Express, PostgreSQL, Vitest, Playwright, GitHub Actions.

## What exists today
- Repository with branch and commit conventions: [CONTRIBUTING.md](CONTRIBUTING.md)
- Pull request template with a test-evidence checklist
- `main` protected by a ruleset (changes require a pull request)
- First test case: [TC-001](docs/qa/test-cases/TC-001-main-branch-protection.md), **Pass**

## Repository layout
| Folder | Purpose |
|---|---|
| `docs/requirements` | Requirements, user stories, acceptance criteria |
| `docs/design` | Architecture, ER diagram, API design |
| `docs/qa` | Test strategy, plan, risk register, traceability |
| `docs/qa/test-cases` | Test scenarios and cases |
| `docs/qa/defects` | Defect reports with evidence |
| `docs/reports` | Execution, regression, release-readiness reports |

## Roadmap
Phase 2 (requirements and design) is next. Later phases add the application, API and UI tests, CI/CD, and a release-readiness report.

## Known limitations
- Solo project: pull request approvals are set to 0.
- Only fake test data is used. No real company data belongs in this repository.

## Licence
MIT