# Unhandled Errors in Node.js HTTP Server

This repository demonstrates a common error in Node.js applications: the lack of robust error handling in HTTP servers. The `bug.js` file showcases a server without proper error handling, while `bugSolution.js` provides an improved version with comprehensive error management.

## Bug

The original server (`bug.js`) doesn't handle potential errors during request processing or server operation. This can lead to the server crashing unexpectedly without providing any information about the error.

## Solution

The solution (`bugSolution.js`) adds comprehensive error handling using `try...catch` blocks and appropriate logging.  It also includes an event listener for `'error'` events emitted by the server object, ensuring that critical errors are caught and handled gracefully.

## Running the Code

1. Clone the repository.
2. Navigate to the project directory.
3. Run `node bug.js` to see the unhandled error scenario.
4. Run `node bugSolution.js` to observe the improved error handling.