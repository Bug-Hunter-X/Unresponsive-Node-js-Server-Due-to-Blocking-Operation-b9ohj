# Node.js Unresponsive Server

This repository demonstrates a common issue in Node.js where a long-running synchronous operation blocks the event loop, causing the server to become unresponsive.

## Problem

The `blockingServer.js` file contains a simple HTTP server that performs a 5-second synchronous operation in the request handler. This operation prevents the server from handling other requests during that time, leading to unresponsiveness.

## Solution

The `nonblockingServer.js` file shows how to resolve this issue using asynchronous operations and promises.  This allows the server to remain responsive while the long-running task completes.