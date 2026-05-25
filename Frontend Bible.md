<img width="1002" height="973" alt="εικόνα" src="https://github.com/user-attachments/assets/a9603b32-2878-4055-9331-081af7b7b2f8" />


# Browser
- Javascript Runtime
  - Event Loop
  - Microtask
  - Macrotask
- JS Engine (V8)
  - Call Stack
  - Heap Memory 
  - Parser
  - Interpreter
  - Compiler
- Web APIs
  - Fetch API
  - Storage API
  - Events API
  - DOM API
- Network Application Layer
  - HTTPS
  - DNS
  - WebSocket
- Rendering Engine (Blink)
  - HTML Parser
  - CSS Parser
  - Layout
  - Paint
- Memory
  - localStorage
  - sessionStorage
  - Cache (Cache API)
  - IndexedDB
  - Cookies
- Trees
  - DOM tree
  - CSSOM tree
  - Render tree
  - Accessibility tree
  - Layer tree
  - BOM tree

# Javascript

## Runtime & JS Engine Concepts
- Agent execution model
  - Realms
  - Scheduler
    - Event Loop
    - Microtask Queue
    - Macrotask Queue
  - JS Engine
    - Heap Memory
    - Call Stack (Stack of execution contexts)
      - Execution Context
        - Global EC
        - Function EC
- JIT Compilation
- Prototype Chain
- Garbage Collection

## Fundamentals

- Data types
  - Primitive values
  - Objects (reference)    
    - Built-in primitive wrapper objects
    - Built-in Constructor objects
    - Built-in Utility objects    
- Scope & Hoisting
- Statements
  - Variables
  - Control flow
  - Functions
  - Classes
  - Iterations
- Expressions
  - Primary
  - Left-hand-side
- Data structures
  - Indexed collections
  - Keyed collections
  - Structured data
- Functions
  - Global Built-ins functions
  - Arrow Functions
  - Default parameters
  - Rest parameters
  - Arguments
  - Callbacks
- Classes
  - Constructor
  - Instance Properties
  - Instance Methods
  - Static Methods
  - Static Properties
  - Getters
  - Setters
  - Private Fields
  - Inheritance (extends)
- Errors
- Promises
- async / await

## Browser Apis
- Events
- Networking
  - Fetch
  - WebSockets
  - WebRTC
  - Server-Sent Events
- Parallelism
  - Web Workers
  - Service Workers
- Storage
  - LocalStorage
  - SessionStorage
  - Cache
  - IndexedDB




---



# React Internals

## Architecture
- React Fiber architecture
- Scheduler / prioritization
- Concurrent rendering (React 18+)

### Rendering Model
- Component render / Mount / Update / Unmount
- Re-renders (on state/props change)
- Virtual DOM
- Reconciliation (diffing algorithm)

### Events System
- Synthetic events
- Event handlers (onClick etc.)
- Cleanup functions


https://medium.com/@canpolat.dev/deep-dive-into-reacts-internal-architecture-from-virtual-dom-to-fiber-08dcf66b309d

# Framework
- Routing
- Data Fetching
- Error Handling
- Forms
- Rendering strategies
- Bundling
