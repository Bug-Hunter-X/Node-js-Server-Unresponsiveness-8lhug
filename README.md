# Node.js Server Unresponsiveness Bug

This repository demonstrates a bug where a Node.js HTTP server becomes unresponsive after handling a certain number of requests.  The server appears to hang, and subsequent requests are not processed.

## Bug Description

A simple HTTP server is created using Node.js's `http` module. Under normal circumstances, it should continue to respond to incoming requests indefinitely. However, after a period of time or a certain number of requests, the server stops responding.

## Bug Reproduction

1. Clone this repository.
2. Run `node server.js`.
3. Send multiple requests to `http://localhost:8080` using tools like `curl` or a web browser.
4. Observe that after a certain point, requests are no longer processed.

## Solution

The provided `server-fixed.js` file demonstrates how to mitigate the issue. It includes fixes to address the potential problem.

## Technologies Used

* Node.js