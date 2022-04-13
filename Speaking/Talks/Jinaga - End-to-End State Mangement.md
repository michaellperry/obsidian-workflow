# Abstract

State management libraries like Redux make it easier to coordinate changes in all parts of your web applications. But they stop at the browser. You are still responsible for developing the API and back-end data store.

Jinaga is an end-to-end state management solution. No custom API. No app-specific database. You write your model, and Jinaga takes it from there:

-   Local storage for offline-first web apps and PWAs
-   Reliable communication with delivery guarantees
-   Application-agnostic persistence for low-friction data evolution
-   Server-sent events for real-time collaboration

What makes this work is a completely different approach to data management. You won't find stores, actions, and reducers. Instead, Jinaga is based on Immutable Architecture. Store the user's decisions as immutable facts. Share those decisions with other clients who express interest. And then interpret those decisions as UI updates.

This does require a shift to your mental model. It won't be easy. But if you apply immutability end-to-end, you might find that many of the hard problems of collaborative web apps are no longer hard problems.

Please allow me to introduce you to Jinaga.

# Short Abstract

Jinaga manages state in React applications. Rather than reducers, actions, and selectors, you write immutable facts. Record each input as a fact, and project it back onto the user interface. Because facts are immutable, apps can detect and resolve conflicts. Save them in a central database with no API. You can even store them in Indexed DB for an offline PWA.

# Key Takeaways

- Model application data using immutable facts
- Simulate mutable properties
- Detect and resolve conflicts
- Store data in Indexed DB for offline PWAs

# Qualifications

I created Jinaga to build on the immutability of ReactJS. Immutability is the key to predictable architectures, including web apps, mobile apps, and microservices. I wrote about this in The Art of immutable Architecture. I'm excited to build a community around the tools and practices of applying immutability to difficult development problems.

# Demos

- Create a fact on Jinaga.com
- Query for facts on Jinaga.com
- Write a specification in Jinaga React application
- Map the specification to a React component
- Write a specification for a collection
- Map the collection into a container
- Subscribe to a query

# Slides

- React Redux app architecture
- Jinaga app architecture
- Demos
- Back-end API and message bus integration