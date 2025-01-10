# Missing Error Handling in Express.js Route Handler

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input and resource not found scenarios.  The `bug.js` file shows the flawed code, while `bugSolution.js` provides the corrected version.

## Bug
The original code lacks error handling for cases where:

1. The `userId` parameter is not a valid number.
2. A user with the given ID is not found.

This can lead to unexpected behavior or crashes in the application.

## Solution
The solution includes explicit checks for these error conditions and returns appropriate HTTP status codes (400 for bad request and 404 for not found) along with informative error messages.