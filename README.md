# React Router v6 Nested Route Issue with Wildcard Parent Route

This repository demonstrates a bug in React Router v6 where nested routes fail to render correctly when a parent route uses a wildcard path (`/*`). The wildcard route incorrectly intercepts all other routes, even nested ones. 

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Navigate to `/about`.

You'll observe that the `/about` route doesn't render; instead, the wildcard route (`/*`) is displayed.

## Solution

The solution involves restructuring the routes to avoid the conflict with the wildcard route. See `AppSolution.js` for a working example.