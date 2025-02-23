# Node.js Port Already in Use Error

This repository demonstrates a common error in Node.js: the `EADDRINUSE` error, which occurs when a server tries to bind to a port that's already in use.

## Bug
The `bug.js` file contains a simple HTTP server that attempts to listen on port 8080. If another application is already using this port, the server will throw an error.

## Solution
The `bugSolution.js` file provides a solution that handles the `EADDRINUSE` error gracefully.  It attempts to start the server, and if the port is unavailable, it waits for a short period before retrying.