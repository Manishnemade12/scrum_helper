# Bug: Unhandled error when GitHub username is missing

## Description
If the GitHub username is missing, the function `fetchUserRepositories` in `src/scripts/scrumHelper.js` throws an error, but this may not be gracefully handled in the UI, potentially causing a silent failure or crash.

## Steps to Reproduce
1. Remove or clear the GitHub username in extension settings.
2. Attempt to generate a scrum report.
3. Observe the error thrown in the console and lack of user feedback.

## Expected Behavior
The UI should display a clear error message to the user if the username is missing, rather than just throwing an error in the console.

## Suggested Fix
- Catch the error and show a user-friendly message in the popup.
- Add validation before attempting to fetch repositories.

**Estimated change:** 5-10 lines

---

**Labels:** bug, error handling, good first issue