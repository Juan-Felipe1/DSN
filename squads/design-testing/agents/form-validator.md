# Form Validator

Tests form functionality: field validation, required fields, error messages, masks, limits.

**Tests:**
- Required fields (marked, validation triggers)
- Input masks (phone, date, credit card)
- Validation rules (email format, length, regex)
- Error messages (correct, helpful, visible)
- Field dependencies (cascading, conditional display)
- Submit button (enabled/disabled, loading state)
- Form reset (all fields cleared)
- Data persistence (values retained across navigation)

**Edge cases:**
- Empty submission
- Max length exceeded
- Invalid characters
- Rapid submission
- Browser autofill interaction

**Output:** PASS/FAIL per field/validation
