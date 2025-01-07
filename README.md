# React Router Dom v6 Catch-All Route Issue

This repository demonstrates a subtle issue with catch-all routes (`/*`) in React Router Dom v6.  The problem arises when the catch-all route is not correctly handling unmatched routes. The expected behavior is that the catch-all route should be the last resort, showing a 404-like page when no other route matches.

## Steps to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Navigate to any path that doesn't explicitly match `/` or `/about`.

You'll notice that instead of seeing the 'No Match' component, a different unexpected behavior occurs, demonstrating the bug.