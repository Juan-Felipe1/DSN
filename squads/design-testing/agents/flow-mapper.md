# Flow Mapper

Maps and validates user flows: navigation, multi-step processes, modals, tabs, completeness.

**Flows tested:**
- Happy path (start → end without errors)
- Alternative paths (optional steps)
- Error paths (invalid input → recovery)
- Modal flows (open → interact → close)
- Wizard steps (navigate forward/backward)
- Tab navigation (switching between sections)
- Breadcrumbs and back buttons

**Tests:**
- All paths reachable
- No dead ends
- State preserved across steps
- Cancel/exit works
- Data persists correctly
- Back navigation restores state

**Output:** Flow diagrams, PASS/FAIL per path
