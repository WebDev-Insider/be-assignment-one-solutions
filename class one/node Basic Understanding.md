# Basic Understanding

**1. What is Node.js and how does it differ from traditional server-side technologies?**

**What is Node.js?**
Node.js allows JavaScript to run outside the browser, mainly on servers. It uses Chrome’s high-speed V8 engine, enabling JavaScript to handle files, databases, and network tasks server-side.

**How It Differs from Traditional Tech:**
Unlike traditional server technologies (like PHP or Java) that create a new thread per request, Node.js uses a single-threaded, non-blocking event loop. This lets it handle many requests at once without waiting for one to finish—making it ideal for I/O-heavy and real-time applications.

**2. Explain the relationship between Node.js and the V8 JavaScript engine.**

**Relationship Between Node.js and the V8 Engine:**

**V8** is Google’s fast JavaScript engine (built in C++) that powers Chrome. It compiles JavaScript into machine code for high performance.

**Node.js** is a runtime that uses V8 to run JavaScript outside the browser, adding features like file access and networking.

**The Relationship:** V8 executes the code; Node.js builds on top of it to enable server-side JavaScript development.

**3. What are the key features that make Node.js suitable for modern web applications?**

**Non-blocking I/O:** Handles multiple requests efficiently using an event-driven model—perfect for real-time apps like chats and live dashboards.

**JavaScript Everywhere:** Enables full-stack development with one language, simplifying code sharing and team workflows.

**High Performance:** Powered by Chrome’s V8 engine for fast execution.

**Vast Ecosystem:** NPM offers thousands of ready-to-use packages to speed up development.

**Scalable Architecture:** Ideal for building scalable systems and microservices.
