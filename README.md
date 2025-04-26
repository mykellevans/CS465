# CS465
Project Architecture and Frontend Approaches

Building the full stack project felt a lot like constructing a living organism, where different parts handled different vital functions. For the public side, Express HTML was the foundation. It offered basic page structure quickly rendered from the server, ideal for visitors seeking immediate content without heavy interactions. JavaScript acted almost like the nervous system, layering dynamic responses onto that structure, giving buttons, forms, and pages an intelligent edge. In contrast, the administrator's side evolved into a Single Page Application (SPA) built in Angular, where content updates fluidly inside the same window. There were no jarring page loads, just a smooth, app-like environment ideal for complex content management.

On the server side, MongoDB was a necessity. The project demanded flexible data models, and MongoDB’s document-oriented design handled evolving schemas better than any rigid SQL alternative. Whenever trip packages changed or new fields were needed, MongoDB allowed fast adaptation without forcing a painful database migration. That agility kept development momentum steady.

Bridging Frontend and Backend with JSON

While JavaScript gives pages thinking power, JSON serves a quieter, but critical role. JSON is a data format, not a language. It does not compute or make decisions. Instead, it organizes information cleanly, acting like a translator between the frontend’s needs and the backend’s resources. Throughout the project, every time the SPA requested updates or new information, the data traveled as JSON payloads. These structured packets moved back and forth between Angular components and Express routes, creating a rhythm that kept both halves of the project in sync.

Refactoring became a habit rather than an afterthought. Early on, form designs in the admin portal duplicated too much code, creating maintenance headaches. I broke those apart into modular, reusable components that dramatically reduced repetition. Backend optimization followed a similar trend, as inefficient queries were restructured to leverage MongoDB indexing, transforming sluggish retrievals into rapid responses. These refinements saved not just loading time but also made future updates much easier.

Testing Layers, Methods, and the Challenge of Security

In full stack development, testing is not a one-size-fits-all effort. Each request type demands a slightly different approach. GET methods required validation to make sure the right information returned under varying conditions, while POST and PUT operations had to be tested both for success and graceful failure. DELETE methods demanded special caution, ensuring only authorized actions could remove critical data.

Security complicated things further. With authentication layered into the project, endpoint testing had to include token validation, login expiry handling, and access permission checks. It was not enough to see a 200 OK; I had to simulate various edge cases, like expired tokens or corrupted payloads, and confirm the system’s ability to defend itself without crashing.

Personal Growth and Professional Impact

If I look back on what this course shifted in my trajectory, it comes down to gaining command over the flow of data, security, and interface design. I learned how to weave together backend APIs and frontend applications into a seamless system, rather than thinking of them as disconnected efforts. I also developed an appreciation for security’s role in every API and user flow, not just as an afterthought but as a design principle. I had a lot of growth during this class that I can be proud of!

Skills like RESTful API construction, NoSQL database management, reusable UI component architecture, and authentication protocol integration are no longer theoretical ideas to me. They are tangible, practiced skills. Every piece of this learning journey builds my marketability, not just by stacking technical knowledge but by showing that I can build real, secure, scalable applications that solve real problems.

Thank you for a great class!
