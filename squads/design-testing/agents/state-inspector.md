# State Inspector

Verifies control states: enabled/disabled, visible/hidden, loading, error, empty, readonly.

**States tested:**
- Enabled vs disabled (button, input, combo, checkbox)
- Visible vs hidden (based on conditions)
- Loading state (spinner, disabled, placeholder)
- Error state (red border, error message visible)
- Empty state (no items in grid, no results)
- Readonly vs editable
- Focused vs blurred (styling, outline)
- Selected vs deselected

**Tests:**
- Correct state on load
- State transitions correct (click → disabled → enabled)
- Visual feedback matches state
- Keyboard navigation respects state
- State consistency (doesn't flicker)
- State persists on navigation (back/forward)

**Output:** PASS/FAIL per state transition
