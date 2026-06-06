# Learning Journal — Week 1, Day 3

**Date:** 2026-06-03
**Focus:** Module 5 (Test Levels) — Component, Component Integration, System, System Integration, Acceptance
**Time spent:** ~3h (tutor session, test-levels exercise, journal)

---

## What I learned today

- Learned about the five levels of testing from the single component to how multiple systems interact and acceptance testing, where we verify the needs and wants of stakeholders and users
- Found out that ISTQB syllabus does not formally define smoke and sanity testing
- E2E is a scenario scope, not a test level — it describes how much of a flow you exercise, not which level you're at

<!-- Prompts to draw from:
- The five test levels and their scope: component (isolated function), component integration
  (two of our modules exchanging data, below the UI), system (whole assembled app through the UI,
  our code), system integration (our system crossing to an external system — Stripe, SEPA, etc.),
  acceptance (stakeholder sign-off against business requirements).
- The two traps: "E2E" is a scenario scope, not a level; system vs system-integration is the
  our-boundary line, not distance or complexity.
- Change-related testing: smoke (new build, broad/shallow, go/no-go gate), sanity (after a change,
  narrow/focused, does the change work and is nearby functionality intact), confirmation/retest
  (same test cases, one fixed defect), regression (previously passing tests, confirms the change
  didn't break anything).
- ISTQB v4.0 formally defines only confirmation and regression (section 2.2.3); smoke and sanity
  are study-guide/industry terms, not syllabus body terms — worth flagging in an interview.
- The teaching-style correction: teach-first for new material, Socratic only after the concept
  has been explained. Updated roadmap and project instructions to reflect this.
-->

## What's still fuzzy

- Need to remember that component integration and component testing in general live bellow UI - code level, not browser
- Make sure to repeat the difference between sanity and retest.

<!-- Honest candidates:
- Component integration — still have to consciously remind myself it lives below the UI.
  The "two things interacting" reflex wants to fire on UI-level observations.
- Smoke vs sanity line — now clean, but worth one more active recall before Day 4.
-->

## What's tomorrow

- Week 1, Day 4 — Module 6 (Static Testing & Reviews): static analysis, review types
  (informal, walkthrough, technical review, inspection), shift-left testing, checklists
- New material — teach-first session, then requirements doc exercise

---

## Deliverables shipped today

- [x] Test-levels deliverable committed (`manual-testing/test-levels/test-levels-saucedemo.md`)
- [x] This journal entry
