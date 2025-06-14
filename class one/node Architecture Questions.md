# Architecture Questions

**1. How does Node.js handle multiple concurrent connections despite being single-threaded?**

- How Node.js Handles Many Connections Efficiently-Node.js uses a single-threaded event loop with non-blocking I/O. When it encounters tasks like file reads or database queries, it offloads them to the system and keeps processing other requests. Once the I/O is done, a callback is triggered and handled by the event loop. This lets Node.js manage thousands of concurrent connections without blocking the main thread.

**2. Explain the concept of non-blocking I/O in Node.js and provide an example of when it's beneficial.**

- Non-blocking I/O means Node.js doesn't pause program execution to wait for tasks like file reads or network requests to finish. Instead, it starts the operation and immediately moves on to handle other tasks. Once the I/O is complete, a callback function is triggered to handle the result.

- Real-World Benefit:
  Imagine a web server querying a slow database. With non-blocking I/O, it can request data for User A, instantly begin processing User B’s request, and then respond to each user as their data becomes available. This keeps the server responsive and prevents it from freezing under heavy load.

**3. What is the event-driven architecture in Node.js and how does it contribute to its efficiency?**

- Node.js follows an event-driven model, meaning it reacts to events rather than executing code in a strict sequence. When an async operation (like reading a file or making a network request) completes, it emits an event. A predefined callback function listens for that event and runs when it’s triggered. This approach keeps the event loop—Node.js’s single main thread—constantly active without waiting. It efficiently handles many concurrent operations with low overhead, making Node.js ideal for I/O-heavy tasks.
