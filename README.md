# React Router v6 Catch-all Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router v6.  The catch-all route incorrectly triggers even when other routes should match.

## Problem
The provided `App.js` file shows a basic React Router setup.  Despite having specific routes defined (`/` and `/about`), the catch-all route (`/*`) is always activated, resulting in the "404 Not Found" component being displayed, regardless of the URL.

## Solution
The solution is provided in `AppSolution.js`.  The issue is resolved by moving the catch-all route to be the last route defined in the Routes component.  This ensures that more specific routes are checked first before the catch all route is considered.