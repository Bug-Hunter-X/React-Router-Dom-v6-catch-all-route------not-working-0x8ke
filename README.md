# React Router Dom v6 Catch-All Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router Dom v6.  The issue is that the catch-all route isn't working correctly, failing to match any unmatched routes. Other routes within the same `Routes` component function properly. 

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Navigate to a route that doesn't match any of the defined routes (e.g., `/nonexistent`).

You'll observe that the `NotFound` component (which should be rendered by the catch-all route) is not displayed.  Instead, nothing is rendered.

## Solution

The solution involves reordering the routes, ensuring the catch-all route is placed at the end.  See `bugSolution.js` for the corrected code.