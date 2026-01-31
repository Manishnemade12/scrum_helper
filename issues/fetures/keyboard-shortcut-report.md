# Feature: Add keyboard navigation for report generation

## Description
Currently, users must use the mouse to generate a scrum report in the popup. Adding keyboard shortcuts (e.g., Enter or Ctrl+Enter) to trigger report generation would improve accessibility and user experience.

## Steps to Reproduce
1. Open the Scrum Helper extension popup.
2. Try to generate a report using only the keyboard (Tab, Enter, etc.).
3. Notice there is no keyboard shortcut for the main action.

## Expected Behavior
Users should be able to generate a report using a keyboard shortcut.

## Suggested Fix
- Add a keyboard event listener in `src/scripts/popup.js` to trigger report generation.
- Document the shortcut in the UI or tooltip.

**Estimated change:** 10-20 lines

---

**Labels:** feature, accessibility, good first issue