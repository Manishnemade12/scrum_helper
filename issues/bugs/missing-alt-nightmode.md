# Bug: Missing alt text for night mode icon in popup.html

## Description
The night mode icon in the popup does not have a descriptive `alt` attribute. This can cause accessibility issues for users relying on screen readers.

## Steps to Reproduce
1. Open the Scrum Helper extension popup.
2. Inspect the night mode icon (`<img src="icons/night-mode.png" ...>`).
3. Notice the `alt` attribute is set to "Night Mode" but does not describe the function or state.

## Expected Behavior
The `alt` attribute should describe the button's function, e.g., "Toggle night mode".

## Suggested Fix
Update the `alt` attribute in `src/popup.html` to a more descriptive value.

**Estimated change:** ~1 line

---

**Labels:** accessibility, bug, good first issue