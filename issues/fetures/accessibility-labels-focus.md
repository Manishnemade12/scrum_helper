# Feature: Improve accessibility for labels and focus states

## Description
Some labels and interactive elements in the popup (e.g., toggles, checkboxes) may not have proper `for` attributes or visible focus states, which can hinder keyboard navigation and accessibility.

## Steps to Reproduce
1. Open the Scrum Helper extension popup.
2. Try to navigate using Tab and Shift+Tab.
3. Observe if all interactive elements are reachable and have visible focus indicators.

## Expected Behavior
- All form controls should have associated `<label for=...>` attributes.
- All interactive elements should have a visible focus state.

## Suggested Fix
- Audit `src/popup.html` and `src/scripts/popup.js` for missing or incorrect label associations.
- Add or improve CSS for focus states.

**Estimated change:** 10-30 lines

---

**Labels:** feature, accessibility, good first issue    