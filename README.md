# Express.js Route Handler Missing Error Handling

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input.  Specifically, the code attempts to access a user by ID, but fails to handle cases where the ID is not a valid number.

## Bug

The `bug.js` file contains the buggy code.  It fetches a user based on the ID passed in the request parameters. If the ID is not a number or if no user with that ID exists, it does not handle this correctly.

## Solution

The `bugSolution.js` file provides a corrected version. It adds error handling to gracefully manage cases where the ID is invalid or the user is not found.

## How to Run

1. Clone this repository.
2. Navigate to the repository directory.
3. Run `npm install` to install the necessary dependencies.
4. Run `node bug.js` to see the original buggy code in action.
5. Run `node bugSolution.js` to observe how the issue is resolved.