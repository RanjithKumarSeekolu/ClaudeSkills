# Fact bank: Ranjith Kumar (living document, edit when facts change)

Rules for this section: only use what is listed here or newly confirmed in chat. When the user corrects something, update it and use the new version everywhere.

### Profile

- **Name:** Ranjith Kumar. **Location:** Hyderabad, India. **Phone:** +919182176879. **Default email:** ranjithkumarseekolu@gmail.com.
- **Education:** B.Tech CSE, IIIT RGUKT RK Valley (shown as "IIIT, RGUKT"), Sep 2019 to May 2023, CGPA 8.87.
- **Links:** LinkedIn linkedin.com/in/ranjithkumarseekolu, GitHub github.com/RanjithKumarSeekolu, LeetCode leetcode.com/Ranjith998, portfolio ranjithkumarseekolu.vercel.app, X x.com/ranjithseekolu.
- **Status:** serving notice period, last working day **10 December 2026**. Spoken languages: English, Telugu, Hindi. Strong knowledge of DSA mostly in Java.Strong Knowledge in Agentic AI. Strong knowledge in System Desing (HLD/LLD). Strong knowledge of Core CS

### WaveMaker India Pvt Ltd, Associate Development Engineer, May 2024 to present, on-site Hyderabad

**Employer context (researched from WaveMaker's site, press releases and coverage; the user should confirm).**

- **What it is:** WaveMaker, Inc. is a private enterprise software company founded in 2003. It sells a Java-based low-code platform that generates real, editable code (Angular for web, React Native for mobile, Spring on the back end) with no lock-in, licensed per developer seat. Customers are enterprise teams and software vendors building many web and mobile apps, and the company now adds AI-assisted code generation.
- **Who the user's users are:** the developers who build apps in WaveMaker Studio. Behind them are the end users of the apps those developers ship, such as bank customers and retail staff.
- **Product pitch:** React Native Studio lets web developers build native iOS and Android apps from one codebase, produce the app files (IPA and APK), export the code and keep working outside WaveMaker, with Expo supported out of the box. The pitch is faster delivery of enterprise mobile apps.
- **Where the user's work sits:** the React Native runtime and component layer that generated apps run on, the Studio preview flow, the build pipeline and tools that turn projects into app files (the CLI and AppChef), parts of the Angular Studio, and customer-facing support. When the user says "the platform", they mean this low-code platform, specifically its React Native runtime or code-generation side.
- **How the company works:** a product company with a Professional Services team that builds apps for customers on the platform, an in-house engineering team, and internal tools such as Sprintly.
- **Framing rule:** in each bullet, say what became faster, safer or easier for the developers building apps on the platform, and what that meant for the enterprise apps running on it.

- **App preview service (Studio):** replaced a per-user Expo dev server with a multi-tenant Node.js service on AWS that builds an app once and serves static bundles. Handles **1,000+ previews a day**. Split bundling made builds about **50 percent faster** and previews about **2x faster** (the user once also said 70 percent for the redesigned architecture, so confirm before using it). Symlinked shared dependencies lowered infrastructure cost (do not say it let containers serve more users). Web preview first, then Expo Go native preview via QR code with static iOS and Android bundles.
- **AWS Lambda proxy:** adds the Expo headers to manifest files so Expo Go opens previews. Three options were weighed (backend team adds headers, DevOps adds headers in the gateway, or a Lambda proxy). The proxy won because it shipped fast and touched nothing else. Only the manifest goes through it. The DevOps team manages the AWS infrastructure, so do not name specific AWS services beyond Lambda.
- **Java endpoints:** Developed and maintained scalable backend services and REST APIs using Java, Spring Boot, and Hibernate ORM for enterprise web applications. Implemented custom business logic, third-party API integrations, and role-based security using Spring Security, JWT, and OpenAPI/Swagger. Improved API speed and code reliability by optimizing MySQL persistence using Spring Data JPA / Hibernate and writing automated unit tests with JUnit and Mockito.
- **wm-reactnative-cli (Node.js):** developer workflow tool for building apps and syncing Studio with local projects, with WebSockets, polling and logging. Major improvements, 5+ commands.
- **AppChef:** build automation for Android (APK/AAB) and iOS (IPA), with build queues, load balancing, a web UI and builds in about 3 to 10 minutes.
- **React Native platform:** components and runtime features, native capabilities (push notifications, Sentry, WebSockets), unit tests. Apps delivered for PNB Retail, FIS banking apps, Blue Yonder retail store and MerchantOps (confirm the spelling of the last name).
- **Critical fixes and support:** a hardware Enter-key bug that broke barcode scanning on retail devices, an esbuild and Flow transform failure that blocked the Expo 54 and React Native 0.81 upgrade, and constant support for customers and WaveMaker's Professional Services team.
- **Angular Studio:** an ESLint configuration UI so users set up linting without editing files (ESLint is a feature here, not a tool the user uses), and a redesign of the whole preview screens for developer experience.
- **Monitoring dashboard:** Dashboard that show previews status for all the users across different environments with logs and alerts triggering if there are critical build failures, WebSockets and polling, with structured logging used to debug incidents.
- **Sprintly:** internal sprint management tool (sprints, releases, team work). The user contributed and uses it. AI agents pick up JIRA tickets and use tailored Claude skills for bug fixes, code review, feature work and React Native QA, and report progress through APIs. Use "contributed to".
- **AI tools:** uses Claude Code and Cursor daily, validating output through tests and peer review.
- All kids of react or react native concepts and optimizations were applied at WaveMaker and Codecrux.

### Worked examples: XYZ bullets framed inside WaveMaker

Use these as patterns. Keep the facts, change the framing for each target company.

- **Preview service:** "Cut app build time by about 50 percent and preview load time by about 2x for developers building apps in WaveMaker Studio, at 1,000+ previews a day, by replacing a dev server per user with a build-once service that serves static web and native bundles on AWS."
- **Phone previews:** "Let developers test their apps on a real iPhone or Android phone by scanning a QR code, without running a server of their own, by extending the preview service to serve native bundles to Expo Go through a small AWS Lambda proxy."
- **Build tools:** "Shortened the path from an app project to store-ready files (APK, AAB, IPA) to about 3 to 10 minutes for teams building on the platform, by adding build queues and load balancing to AppChef and improving the CLI that builds and syncs projects locally."
- **Runtime and customer fixes:** "Kept enterprise apps for banks and retailers (PNB Retail, FIS, Blue Yonder, MerchantOps) running by fixing critical customer-raised bugs in the React Native runtime, such as a hardware Enter-key bug that broke barcode scanning on retail devices and a build failure that blocked the Expo 54 upgrade, and supported the Professional Services team that builds with the platform."

### Codecrux, Associate Software Engineer, Nov 2023 to Apr 2024, remote

**Employer context (researched from the company's own site; the user should confirm).** CodeCrux Web Technologies Pvt Ltd is a Hyderabad software company based at T-Hub, offering web and mobile app design and development, REST API services, and apps for e-commerce, healthcare and real estate, including real estate CRM and property management software. It works like a client-delivery firm: the user built features and APIs for a client's real estate platform, so the users are that client's agents or tenants and the buyer is the client. Frame bullets around what shipped for the client and how fast and reliably.

- 10+ features on a real estate platform, React, 20+ REST APIs documented in Swagger, JWT authentication, input validation, PostgreSQL data model.
- **Back-end stack conflict:** the user has said Node.js and Express, Python with FastAPI, and once mentioned Django and Spring Boot versions. **Confirm one answer and use it everywhere.** If unsure, leave the framework unnamed.

### SkillRazr, SDE Intern, Apr 2023 to Sep 2023 (six months), remote

**Employer context:** no reliable public information was found about SkillRazr, so do not guess. Ask the user what it sells, who used it (students, instructors, institutes) and how large it was. What is known from the user: a live-classes and learning platform with ClassCast, flashcards, quizzes and courses. The user's public ClassCast front-end repo describes live classes built with React, Tailwind and WebSockets.

- React, Redux, TypeScript and Tailwind pages in an Agile team, contributing to a 20 percent rise in unique visitors. ClassCast live classes with WebSockets and a Node.js back end, a collaborative Monaco code editor, flashcards and quizzes.

### Projects (only these exist)

- **Dejank:** open-source MCP server on npm (github.com/RanjithKumarSeekolu/dejank, npmjs.com/package/dejank) that lets AI agents inspect, profile and drive React Native apps on real devices.
- **Lumina:** Play Store app (play.google.com/store/apps/details?id=com.luminablocker, github.com/RanjithKumarSeekolu/luminablocker) with a Kotlin native module using the Expo Modules API, and an LLM API (OpenRouter) with schema-constrained prompts and validated structured JSON.
- **RentNHost:** car rental platform (github.com/RanjithKumarSeekolu/Car-Rental, car-rental-3a89c.web.app). React front end, FastAPI back end, OAuth2, Google Maps, Firebase. The back end was also ported to Java 17 and Spring Boot 3 with Firebase Auth verification, admin role guards, Razorpay payments, global exception handling and JUnit tests.
- **Planned, not built:** an Amazon Connect call-flow demo. Do not list it until it is pushed to GitHub.

### Stated hands-on experience (the user says they have worked on these at their companies)

The user has said, in chat, that they know these from real work, not only from study. Treat them as claimed experience, never as gaps. Write them from the Employer Context by default. Ask for a concrete example only on large doubt, and record any example the user gives here.

- **React Native in depth:** components and component design, state management and stores, performance, native modules and runtime features. Infer from the runtime and component layer of the low-code platform. Ask only if a specific store, library or number is needed.
- **Backend (Node.js and Python):** services, APIs, data models, auth. Infer from the preview service, CLI and AppChef (Node.js) and the dashboard and Sprintly services (Python).
- **System design (HLD and LLD):** the preview service is the main example (multi-tenant service, proxy choice, scale). Earlier the user also said they learned HLD and LLD from lectures. Both are true if the lectures taught the vocabulary and the work gave the practice. Use the build queue and load balancing in AppChef as a second design example.
- **AWS services:** the user has said they used AWS services extensively in WaveMaker. Earlier they said the DevOps team manages the infrastructure and they were not sure which services. Name only services the user has mentioned (Lambda for the manifest proxy). Describe the rest as "AWS" without naming services, and ask only if a job needs a specific service name.

Do not turn "I know everything about X" into the words "expert" or "everything" on a resume. Show the depth with specific examples, and let the interview prove the rest.

### Knowledge but no work experience

DynamoDB, Playwright (light use), Next.js, RabbitMQ (Used in Certiflow (https://github.com/RanjithKumarSeekolu/certiflow_backend, https://github.com/RanjithKumarSeekolu/certiflow_frontend)). List these in skills when useful, never in experience bullets.
