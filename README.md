# David Song

**Product Developer** · End-to-End Problem Solving · Agentic AI · Workflow Automation · Service Operations

As a product engineer driven by solving business challenges, I founded both an AX venture and a postpartum care franchise, building an integrated business operations platform that unifies customer management with internal AI agents for headquarters workflow automation. Leading end-to-end development, I directed everything from problem definition to UI, API, and database design, as well as AWS deployment, monitoring, and automated disaster recovery. I established a highly maintainable architecture through NestJS layered design while leveraging Next.js and Supabase for agile implementation and continuous maintenance. Furthermore, I developed a custom "Agent Workflow Harness" to operate an agent-driven development pipeline, standardizing agents.md, skill.md, hooks, and agent SDKs to prevent context drift and maximize token efficiency.

## Experience

### Covenant Labs — Founder · Product Developer

**Dec 2025 – Present**

Postpartum care operations platform, internal AI agents and business systems

- Product strategy and delivery: Founded Covenant Labs and translated client operations into product requirements. Defined roadmaps, operating procedures, AI usage guidelines and engineering standards; owned delivery across frontend, backend, databases, deployment and operations.
- Operations platform: Built BabyJamJam for postpartum care providers, connecting consultations, client registration, caregiver assignments, contracts, schedules, service records and notifications. Implemented branch-specific workflows and data access in a web admin and mobile PWA.
- AI consultation automation: Used n8n and Gemini to process consultation recordings into structured summaries, client details, requests and supporting evidence. Generated reviewable client drafts and connected staff approval to registration, scheduling, notifications and electronic contracts.
- Internal agents: Designed marketing agents using Notion reference documents and external research, and product QA agents reviewing PRDs, code, tests and operational evidence. Applied human approval to key actions and recorded findings with severity, evidence and follow-up steps.
- Workflow orchestration: Separated Hermes request intake and task execution, n8n scheduling, integrations and retries, and LLM reasoning and structured outputs. Unified consultation, marketing, product QA and technical review workflows with approvals, status tracking and recovery.
- Infrastructure and recovery: Configured AWS operations and a local server fallback path so AI workflows could continue in either environment. Managed execution-state synchronization, monitoring and recovery procedures.
- Quality and operational safety: Connected Playwright E2E tests against live databases and APIs, authentication and branch-isolation tests, and migration checks to CI. Enforced shared UI rules with Glint component specifications and ESLint; applied feature flags and rollback procedures.

### Imirae Incheon — Full-Stack Developer · Contract

**Mar 2024 – Present**

- Operations improvement: Integrated client, caregiver, scheduling and electronic-document management, reducing processing time per case by 67% and doubling monthly processing capacity.
- Electronic contracts and data synchronization: Integrated the eFormSign API for contract issuance, signatures and webhook status updates. Used database transactions and duplicate-event protection to keep external document states consistent with internal client data.

### Bridge — Frontend Developer Intern

**Aug 2023 – Dec 2023**

- User experience and maintainability: Improved information architecture and responsive navigation on core screens, increasing customer retention by 23%. Built reusable UI components, reducing customer inquiries by 35%.

## Selected projects

### Internal AI Agent Platform — Automation and AgentOps

**2026 – Present**

- Agent architecture: Separated Hermes intake and task execution, n8n scheduling, integrations and retries, and LLM reasoning and structured outputs. Managed approvals, processing states and recovery through shared workflows; supplied relevant knowledge through section-based document retrieval and a local cache.
- Sentry issue response: Built a Grok Bot workflow to detect all incoming Sentry issues and report problems and proposed solutions to the responsible developer. Assigned fixes to Claude Code and automated code changes, review, QA and pull request creation.
- Marketing and product QA: Generated strategy, campaign and content plans from Notion references and external research, with approval gates for publishing, ad spend, pricing and contracts. Reviewed PRDs, code, tests and operational evidence to record missing features, regression risks, severity and follow-up actions.
- Multi-agent technical review: Used the OpenAI Agents SDK for independent architecture, operational safety and technical suitability reviews, with cross-checks and counterarguments. Validated decisions, confidence and risk with Zod; withheld conclusions below the confidence threshold and restricted inputs by role.

### [BabyJamJam Admin — Postpartum Care Platform](https://github.com/jaino-song/babyjamjam-admin)

**Dec 2025 – Present**

- Product architecture: Built a pnpm monorepo with a Next.js web admin and mobile PWA, NestJS APIs, and PostgreSQL/Prisma. Shared types, schemas and UI packages; connected consultations, assignments, contracts and service records in one operational workflow.
- Authorization and data integrity: Separated domain rules from data access with Clean Architecture and DDD. Validated selected branches, roles and active memberships; scoped client-draft access and confirmation by branch. Used idempotency, terminal-state protection and snapshots to handle duplicate or delayed webhooks.
- Quality and UI validation: Built Playwright E2E tests using PostgreSQL, Valkey, Mailpit and NestJS, plus authentication and branch-isolation integration tests. Added migration and database-patch checks to GitHub Actions, and shared UI-rule checks using Glint specifications and ESLint.

### Agent Harnesses — Rules and Skills · Configuration

**Dec 2025 – Present**

Custom Agent Workflow Harness: shared rules, skills, tool adapters, and development orchestration.

- Shared rules and tool adapters: Organized engineering rules for Claude Code, Codex, OpenCode and Antigravity into a shared Core, domain guidance and tool-specific adapters. Guided each task to load the relevant rules and skills.
- Skill catalog validation: Automated catalog generation and checks for missing references and stale entries. Connected shared rules and reusable skills to tool-specific configuration and execution lifecycles to maintain consistent engineering practices.
- Configuration and recovery: Separated preview, apply and rollback, checking file changes before recovery to preserve later edits. Published architecture documentation, a Python reference demo and unit tests demonstrating selective loading, catalog validation and configuration recovery.
- Dev Guru development orchestration: Coordinated implementation, independent review and verification in isolated worktrees. Scoped tools and QA per task, validating results and execution evidence against the same candidate.

Public references (architecture and runnable demos with synthetic inputs; the implementations are private):

- [Agent Harnesses](https://github.com/jaino-song/agent-harnesses) — [architecture](https://github.com/jaino-song/agent-harnesses/blob/main/docs/architecture.md) · [public reference demo](https://github.com/jaino-song/agent-harnesses#run-the-public-reference-demo)
- [Covenant Labs Factory showcase](https://github.com/jaino-song/covenant-factory-showcase) — [architecture](https://github.com/jaino-song/covenant-factory-showcase/blob/main/docs/architecture.md) · [evidence-checking demo](https://github.com/jaino-song/covenant-factory-showcase#run-the-evidence-checking-demo)

### [Fiterview — AI Mock Interview Service · Team Project](https://github.com/jaino-song/Fiterview)

**Jul 2025 – Aug 2025** · [fiterview.com](https://fiterview.com/)

- AI product workflow: Built a mock interview service that analyzes resumes and job postings to identify role requirements, generate tailored questions, evaluate answers and provide actionable feedback.
- Performance and recognition: Improved LLM API orchestration and application layers in Next.js, TypeScript and Prisma, reducing response time by 30%. Won the top project award at the LIKELION frontend bootcamp.

## Technical skills

- **Product development:** TypeScript, JavaScript, React, Next.js, NestJS, Node.js, PostgreSQL, Prisma, Supabase, REST API, SSE, TanStack Query, Zustand
- **AI systems:** Hermes, n8n, Grok Bot, OpenAI Agents SDK, Claude Code, Codex, Gemini API, tool calling, structured outputs, retrieval, approvals, agent evaluation
- **Infrastructure and AgentOps:** AWS, local servers, fallback and recovery, GitHub Actions, Vercel, Railway, SQLite FTS5, Sentry, PostHog
- **Architecture and quality:** Clean Architecture, DDD, multitenancy, Jest, React Testing Library, Playwright, custom ESLint, CI validation, comparative runs, rollback

## Education

- **Georgia Institute of Technology** — M.S. Computer Science · Machine Learning Specialization · In Progress
- **New York University** — B.S. Information Systems Management · 2025 · GPA 3.73/4.00 · Dean's List

Korean · English

## Connect

[LinkedIn](https://www.linkedin.com/in/jaino-dev/) · [Email](mailto:david.jh.song@gmail.com)
