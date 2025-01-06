# Node.js Server: listen EADDRINUSE error

This repository demonstrates a common error encountered when running a Node.js HTTP server: the `listen EADDRINUSE` error.  This occurs when the server attempts to bind to a port that is already in use by another process.

The `bug.js` file contains the problematic code. The `bugSolution.js` file provides a solution to handle this scenario gracefully.

## Setup

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `npm install` (not necessary in this case but good practice).

## Running the Code

1. Run `node bug.js`. You'll see the error `listen EADDRINUSE` because port 8080 is already in use by another process (most likely by the server itself if you try to run multiple times without stopping it).
2. Run `node bugSolution.js`. This will attempt to start the server and handle the error if the port is already in use, providing more informative feedback.