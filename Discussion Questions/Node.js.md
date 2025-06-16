# Node.js

**1. How does Node.js's single-threaded nature affect its performance and scalability?**

Node.js runs all JavaScript code in one main thread — meaning one task at a time in the event loop. But thanks to non-blocking (asynchronous) I/O, it can handle many things at once without waiting.

$$
Performance   Impact:
$$

$$
Pros:
$$

Great for handling many concurrent connections (e.g., APIs, chats, real-time apps).

Super efficient for I/O-heavy tasks like reading files, databases, or making API calls.

$$
Cons:
$$

Not ideal for CPU-heavy tasks (like image processing or complex calculations), because one long-running task can block everything else.

$$
 Scalability:
$$

Scales well using clusters or worker threads — you can run multiple Node.js instances to take advantage of multi-core CPUs.

Also easily scaled horizontally (across servers) for high-traffic applications.

**2. What are the advantages and disadvantages of using an event-driven architecture?**

$$
 Advantages:
$$

Scalable – Components are loosely connected, making it easier to scale parts of the system.

Responsive – Great for real-time apps (e.g., chats, notifications).

Flexible – Easy to plug in or change parts without affecting everything.

Decoupled – Services don’t need to know about each other directly.

$$
Disadvantages:
$$

Harder to Debug – Events may come from anywhere, making issues harder to trace.

Complex Flow – It’s not always clear what happens next or in what order.

Error Handling – More difficult across multiple event-driven components.

Testing is Tricky – Because events happen asynchronously and across systems.

**3. How does Node.js's non-blocking I/O model benefit web applications?**

Node.js uses non-blocking I/O, meaning it can handle other tasks while waiting for things like file reads, database calls, or API responses.
