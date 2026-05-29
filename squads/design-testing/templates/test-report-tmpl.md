# Test Report: {{screen_name}}

**Generated:** {{generated_at}}  
**Test Duration:** {{duration_minutes}} min  
**Tested By:** Design-Testing Squad  

---

## Executive Summary

| Metric | Value |
|--------|-------|
| Total Scenarios | {{total_scenarios}} |
| ✅ PASS | {{pass_count}} ({{pass_percentage}}%) |
| ❌ FAIL | {{fail_count}} ({{fail_percentage}}%) |
| ⏭️ N/A | {{na_count}} |
| Health Score | {{health_score}}/100 |

**Severity Distribution:**
- 🔴 Critical: {{critical_count}}
- 🟠 High: {{high_count}}
- 🟡 Medium: {{medium_count}}
- 🟢 Low: {{low_count}}

**Status:** {{deployment_status}}

---

## Coverage by Area

### 🎨 DESIGN & LAYOUT
{{design_results}}

### ⚡ EVENTS & INTERACTIONS
{{events_results}}

### 🔀 USER FLOWS
{{flows_results}}

### 📝 FORMS & VALIDATION
{{forms_results}}

### 🎛️ CONTROL STATE
{{state_results}}

### 🔌 BACKEND INTEGRATION
{{backend_results}}

### 🔗 COMBINATIONS
{{combinations_results}}

---

## Scenario Results

| ID | Description | Area | Severity | Result | Notes |
|----|-------------|------|----------|--------|-------|
{{scenario_table}}

---

## Critical Issues

{{critical_issues}}

---

## High Priority Issues

{{high_priority_issues}}

---

## Sign-Off

| Role | Name | Date | Status |
|------|------|------|--------|
| Test Engineer | ___________________ | _________ | [ ] Approved |
| QA Lead | ___________________ | _________ | [ ] Approved |
| Product Owner | ___________________ | _________ | [ ] Approved |

**Deployment Readiness:** [ ] APPROVED [ ] BLOCKED [ ] CONDITIONAL

---

## Appendix

### Coverage Matrix
```
DESIGN:        ████████████████░░ 90%
EVENTS:        ██████████████████ 95%
FLOWS:         ████████████░░░░░░ 80%
FORMS:         ██████████████░░░░ 85%
STATE:         ██████████████████ 100%
BACKEND:       ███████████░░░░░░░ 75%
COMBINATIONS:  ██████████░░░░░░░░ 70%
```

### 7 Laws Compliance

- [ ] LAW #0 (Cobertura Total): All elements tested
- [ ] LAW #1 (Binário): All criteria are PASS/FAIL
- [ ] LAW #2 (Atomic): Each scenario is 1 behavior
- [ ] LAW #3 (Severity): All scenarios have severity
- [ ] LAW #4 (Edge Cases): Included and prioritized
- [ ] LAW #5 (Combinações): State × Event × Data tested
- [ ] LAW #6 (Report): Format is standardized

### Test Execution Time

- Scenario Planning: {{planning_time}} min
- Specialist Execution: {{execution_time}} min
- Consolidation: {{consolidation_time}} min
- Total: {{total_time}} min
