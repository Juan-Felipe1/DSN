# Story: Test Dispatch Squad Execution

**ID:** TEST-001  
**Status:** 🔄 In Progress  
**Created:** 2026-05-29  

---

## Objective

Test the dispatch squad with a simple multi-task story to verify:
- Story decomposition into atomic tasks
- Wave optimization (parallelism)
- Correct model selection (Haiku/Sonnet)
- Quality gates
- Cost tracking

---

## Acceptance Criteria

- [ ] Dispatch decomposes into 3-5 atomic tasks
- [ ] Tasks organized into 2+ parallel waves
- [ ] Quality gate (pre-execution) validates all tasks
- [ ] Execution completes without errors
- [ ] Post-execution report shows cost and health score

---

## What to do

Create a simple technical document with:
1. **Summary section** - 2 paragraphs explaining dispatch squad (Haiku task)
2. **Installation guide** - Step-by-step setup instructions (Haiku task)
3. **Usage examples** - 3 code examples with explanations (Haiku task)
4. **Troubleshooting** - 5 common issues and fixes (Sonnet task - needs judgment)

---

## Output Format

Markdown document with structure:
```
# Dispatch Squad User Guide

## Summary
[2 paragraphs]

## Installation
[Step-by-step]

## Usage Examples
[3 examples]

## Troubleshooting
[5 issues + fixes]
```

---

## Notes

- This is a TEST story to verify dispatch functionality
- Expected cost: ~$0.03 (will see actual in report)
- Expected time: 2-3 minutes total
- Should execute in 2 waves:
  - Wave 1: Summary + Installation + Examples (3 Haiku tasks in parallel)
  - Wave 2: Troubleshooting (1 Sonnet task)

---

## Files

- Input: This story
- Output: `docs/dispatch/dispatch-user-guide.md` (created by dispatch)
