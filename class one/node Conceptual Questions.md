# Conceptual Questions

**1. What is NPM and what role does it play in Node.js development?**

- NPM (Node Package Manager) is the default package manager for Node.js. It plays a key role in development by:

- Managing Packages: Easily install, update, and share reusable libraries and tools from a vast online registry.

- Handling Dependencies: Automatically tracks and installs all the packages your project needs to run smoothly across environments.

- Running Scripts: Lets you define and execute custom commands for tasks like testing, building, or deploying your app.

**2. Why is Node.js considered cross-platform, and what are the benefits of this feature?**

- Node.js is cross-platform because it runs seamlessly on major operating systems like Windows, macOS, and Linux without needing code changes. This is made possible by its use of the V8 engine and abstraction of system-level operations.

Benefits:

- Wider Reach: Build once and run anywhere, making apps accessible across platforms.

- Simplified Development: One codebase for all environments reduces time and effort.

- Flexible Deployment: Easily deploy to various server setups with no compatibility issues.

- Cost-Effective: No need for separate teams or infrastructure for different platforms.

**3. What are built-in modules in Node.js, and why are they important?**

- Built-in modules are core features included with Node.js—no installation needed. You simply use require() to load them. Examples include:

fs – file system operations

http – create HTTP servers and clients

path – handle file paths

os – interact with the operating system

- Why They Matter:
  These modules provide essential low-level tools for server-side development, enabling tasks like file access, networking, and system interactions. They form the foundation on which more complex apps and external packages are built.
