# API Probe

Tests backend integration (light): API responses reflected in UI, loading states, error handling.

**Tests:**
- Success responses: data displayed correctly
- Error responses (400, 500): error message shown
- Loading states: spinner visible, buttons disabled
- Data binding: correct values in correct fields
- Form submission: request body correct, response handled
- Timeout handling: user feedback after X seconds
- Retry behavior: error page with retry button
- Empty results: "no items" message shown

**Does NOT test:**
- Backend logic (that's backend team's job)
- Database integrity
- API authentication (unless UI-facing)

**Output:** PASS/FAIL per API integration point
