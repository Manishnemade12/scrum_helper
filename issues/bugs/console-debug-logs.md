# Bug: Console debug logs left in production code

## Description
There are several `console.log` and `console.error` statements in the production code (e.g., `src/scripts/scrumHelper.js`, `src/scripts/main.js`). These should be removed or guarded by a debug flag to avoid leaking debug information in production.

## Steps to Reproduce
1. Use the extension in production mode.
2. Open the browser console.
3. Notice debug logs from the extension.

## Expected Behavior
No debug logs should appear in the console unless a debug mode is enabled.

## Suggested Fix
- Remove or guard all debug logging with a `DEBUG` flag.
- Audit all scripts for stray `console.log`/`console.error`.

**Estimated change:** 10-30 lines

---

**Labels:** bug, cleanup, good first issue