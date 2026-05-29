# Design-Testing Squad

**Version:** 1.0.0  
**Purpose:** Comprehensive UI/UX testing for screens and components  
**Scope:** Design, events, flows, clicks, forms, state, backend integration  

## Quick Start

```
@design-chief

Please test the [Screen Name].
It has [brief description].
Cover: design, events, flows, forms, state, backend.
```

## What This Squad Does

Takes a screen/component and generates **60+ test scenarios** covering:

| Area | Tests |
|------|-------|
| **Design** | Layout, spacing, colors, typography, responsive |
| **Events** | Clicks, hovers, focus, keydown, drag-drop, combinations |
| **Flows** | Navigation, wizard, modals, tabs, completeness |
| **Forms** | Fields, validation, required, messages, masks, limits |
| **State** | Enabled/disabled, visible/hidden, loading, error |
| **Backend** | API responses in UI, loading states, error handling |
| **Combinations** | State × Event × Data = real-world coverage |

**Output:** Structured test document with:
- ✅ PASS/FAIL/N/A results
- 🎯 Severity badges (Critical, High, Medium, Low)
- 📋 Scenario details (preconditions, steps, expected)
- 🖼️ Screenshots of failures
- ✍️ Sign-off table (test engineer, QA, product owner)

## 7 Immutable Laws

1. **COBERTURA TOTAL** — Every element has a scenario
2. **BINÁRIO** — All criteria are PASS/FAIL only
3. **ATOMIC** — 1 scenario = 1 behavior
4. **SEVERITY** — Every scenario has a severity level
5. **EDGE CASES FIRST** — Empty, limit, special chars prioritized
6. **COMBINAÇÕES** — Test State × Event × Data combinations
7. **REPORT PADRONIZADO** — Consistent output format

## Agents

| Agent | Role |
|-------|------|
| design-chief | Orchestrator |
| test-gate | Scope validation |
| scenario-planner | Scenario decomposition (BDD) |
| test-router | Specialist routing |
| visual-validator | Design/Layout testing |
| event-tester | Interaction testing |
| flow-mapper | User flow validation |
| form-validator | Form testing |
| state-inspector | State verification |
| api-probe | Backend integration (light) |

## File Structure

```
squads/design-testing/
├── config.yaml                 (Full configuration)
├── README.md                   (This file)
├── requirements.txt            (Python dependencies)
├── agents/                     (10 agent definitions)
├── checklists/                 (5 quality gates)
├── data/                       (Event registry, patterns, etc.)
├── templates/                  (Test report, plan templates)
├── tasks/                      (Executable tasks)
└── workflows/                  (BDD workflows)
```

## Testing Workflow

```
1. Input Screen
    ↓
2. test-gate validates scope (QG-SCOPE)
    ↓
3. scenario-planner generates 60+ scenarios (BDD)
    ↓
4. test-router routes to 6 specialists
    ↓
5. Specialists execute in parallel (DESIGN, EVENTS, FLOWS, FORMS, STATE, BACKEND)
    ↓
6. design-chief consolidates results
    ↓
7. Output: Test report (PASS/FAIL/N/A) with sign-off
    ↓
8. QG-EXECUTION validates completeness
```

## Output Example

```
TEST REPORT: FrmTarefaDepositoLayoutSepara
Generated: 2026-05-29
Total Scenarios: 67
Results: 63 PASS, 2 FAIL, 2 N/A
Overall Health Score: 94/100

COVERAGE BY AREA:
- DESIGN: 10/10 PASS
- EVENTS: 18/18 PASS
- FLOWS: 12/12 PASS
- FORMS: 15/16 PASS (1 FAIL: validation message missing)
- STATE: 8/8 PASS
- BACKEND: 3/3 PASS
- COMBINATIONS: 2/2 N/A (not applicable)

CRITICAL ISSUES:
None

HIGH PRIORITY:
- Form validation error message missing on required field

SIGN-OFF:
[ ] Test Engineer: Juan Silva [2026-05-29]
[ ] QA Lead: Maria Gomez [2026-05-29]
[ ] Product Owner: Carlos Mendez [PENDING]
```

## When to Use

✅ Preparing for QA sign-off  
✅ Pre-release validation  
✅ Regression testing after changes  
✅ New feature testing  
✅ Component library validation  
✅ Finding gaps before users do  

## Collaboration with Dispatch

This squad works great with **dispatch squad** for:
- Parallelizing specialist execution
- Economizing tokens (Haiku for simple scenarios, Sonnet for judgment)
- Cost tracking per test run
- Wave optimization

## References

- **AIOX Core:** `.aiox-core/` (framework)
- **Dispatch Squad:** `squads/dispatch/` (execution engine)
- **Related:** `docs/dispatch/` (test examples)
