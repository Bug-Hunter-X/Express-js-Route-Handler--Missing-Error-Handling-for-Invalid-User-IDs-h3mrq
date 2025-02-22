# Express.js Route Handler: Missing Error Handling for Invalid User IDs

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input, specifically focusing on user IDs.

The `bug.js` file shows the problematic code, where an attempt is made to parse a user ID as an integer without any validation. This can lead to unexpected errors if the ID is not a valid integer.

The `bugSolution.js` file provides a corrected version with robust error handling, preventing crashes and providing appropriate responses to clients.

## How to Reproduce

1. Clone the repository.
2. Navigate to the project directory.
3. Run `node bug.js` and make requests to `/users/:id` with both valid and invalid IDs.  Observe the behavior.
4. Run `node bugSolution.js` and make the same requests. Note the improved error handling.