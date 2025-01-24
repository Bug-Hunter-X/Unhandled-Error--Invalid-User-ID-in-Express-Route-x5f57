# Unhandled Error: Invalid User ID in Express Route

This repository demonstrates a common error in Express.js route handlers:  the lack of proper error handling for invalid input.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version.

## Problem

The original code attempts to fetch a user based on an ID passed in the route parameter.  However, it fails to handle cases where the ID is not a valid integer, leading to potential errors or unexpected behavior.

## Solution

The solution incorporates robust error handling.  It checks if the ID is a valid integer and if a user with that ID exists.  If either condition is false, an appropriate HTTP error response is returned.