### Hi, I'm Ratthapol

Full-stack engineer and tech lead in Thailand. I build and run production systems for government, healthcare, finance and manufacturing clients, mostly on .NET and TypeScript.

Most of my work is the groundwork other developers build on: the stack, shared code, code review and AI tooling. I have reviewed over a thousand pull requests and made over 4,000 contributions in the past year, mostly in private client repositories.

### Stack

- **Back end:** C# / .NET, ASP.NET Core, EF Core, Wolverine, OpenIddict. Rust in my own projects.
- **Front end:** TypeScript, React, Next.js, Vite, Mantine, TanStack.
- **Data:** PostgreSQL, SQL Server, Redis, Qdrant.
- **Delivery and testing:** Docker, GitHub Actions, Playwright, k6, Trivy.

### How I work

- TypeScript in full strict mode with no `any`. Data from outside is validated before use.
- Business rules don't depend on the database or the web framework, so they can be tested alone.
- Layering, naming and security rules are checked by lint and tests, so a broken rule fails the build.
- I write specs, estimates, decision records, runbooks and handover guides in Thai and English, and plan my own work in **my-helm**, a plain-text workspace.
- I often work remotely from a home lab over Tailscale. I'm slowly turning it into a small self-hosted cloud.

### Foundations for my team

- I set the front-end and back-end stack and conventions for the company's development team.
- I wrote most of the UI library and starter that new front-end projects begin from, and co-built a generator for first-draft screens.
- I maintain parts of the company's back-end packages, including sign-in.
- I built a small reference system with the same structure as production, for new developers to read before they start on a real one.

### Testing and quality

- End-to-end tests in four layers: use cases, the actors who perform them, the screens they use, and drivers for the API and the mailbox. Lint keeps the layers apart.
- A test fails on any console error, failed request or error response, even if its assertions pass.
- The list of use cases, with Thai descriptions for non-developers, is generated from the test titles. The build fails if it goes out of date.
- Permission tests read the real roles from the system and check that each role can open only its own pages.
- Load tests that find where a system starts to slow down and where it fails.

### Some of my work

- Procurement portals, a ministry website and a local government data platform, with public sites, officer back offices and single sign-on.
- A GIS map editor for government data.
- A nightly import from Thailand's national e-procurement system, and APIs for outside agencies.
- A hospital laboratory service platform and a healthcare web platform.
- Manufacturing systems for change control, risk evaluation, budgets and approvals.
- Fintech and legal case-management platforms, mostly as the main reviewer.
- A survey platform that connects researchers with participants.
- Cloud servers, deployments and CI/CD pipelines. A DevOps team runs most of this now.

### AI engineering

- RAG chatbots on a vector database, one of them for a large telecom company. They cite sources, keep per-user history and can switch LLM providers.
- OCR and data extraction from documents with LLMs, and an AI pull-request reviewer.
- I wrote most of the company's agent skills: reusable instructions and scripts that guide an agent through intake, estimates, specs, pull-request review, release and documentation.
- **Harness engineering**
  - Steps that must give the same result every time run as scripts.
  - Model output has a fixed shape, checked by a validator.
  - Skills have evals.
  - Hooks and permission guards let long runs go unattended.
- **Loop engineering**
  - Each loop states what one round does, when it stops and who judges it.
  - Cheaper models do the work and a stronger model reviews it. Nothing merges until tests and review pass.
- A dashboard that shows each agent session's task tree, conversation and output.

### Security and data protection

- On a government platform, I found and fixed queries that let one organization read another's data.
- I wrote the company's tools for masking personal data in documents, screenshots and databases, checking that masked databases don't leak, and checking websites against Thailand's national website security standard.
- PDPA Data Protection Officer (DPO) workshop, 18 hours, 2025.
- ISO/IEC 27001 information security management course, five days (40 hours), 2026.

### Education

- B.Sc. in Computer Science, Khon Kaen University, Thailand (2018)
