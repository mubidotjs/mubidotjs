# Mubashir Hussain

**Senior Full-Stack Engineer | AI Applications & Backend Systems**

I build full-stack applications, SaaS products, APIs, and integrations, with 5+ years of professional experience connecting product interfaces to backend workflows. My foundation is JavaScript/TypeScript engineering, data modeling, and reliable delivery; I’m extending that work through practical AI applications. I favor explicit system boundaries, tested failure paths, and architecture that makes usable software easier to ship and maintain.

[Portfolio](https://mubashirhussain.dev) · [Résumé](https://mubashirhussain.dev/resume)

## Featured Engineering

### [AI Release Notes Generator](https://github.com/mubidotjs/ai-release-notes-generator)

Turns public GitHub comparisons into categorized release notes with inspectable source evidence.

- A Cloudflare Worker retrieves bounded commit context and calls Workers AI. Coverage warnings disclose omitted commits; request, prompt, output, and time limits constrain resource consumption.
- Strict schemas, retrieved-SHA checks, and exact evidence excerpts reject malformed output and fabricated references. Provider failures surface explicitly, without automatic retries or paid fallback.

**Stack:** React, TypeScript, Vite, Cloudflare Workers AI, Zod.

**Status:** Deployed live integration verified on one documented generation. Sources are commit messages; mechanical grounding does not establish semantic correctness or general model quality.

[Live demo](https://release-notes.mubashirhussain.dev) · [Architecture](https://github.com/mubidotjs/ai-release-notes-generator/blob/main/docs/ARCHITECTURE.md) · [Evaluation](https://github.com/mubidotjs/ai-release-notes-generator/blob/main/docs/EVALUATION.md)

### [Reliable Webhook Platform](https://github.com/mubidotjs/reliable-webhook-platform)

Makes webhook acceptance durable and failed delivery recoverable, with an operations UI for investigation and replay.

- Events, deliveries, and outbox work commit together before acknowledgment. Leased processing and stale-worker fencing support recovery while preserving at-least-once delivery semantics.
- Idempotent ingestion, bounded retries, HMAC signing, and tenant-scoped access protect delivery boundaries. Failure-path tests exercise recovery and replay while preserving immutable attempt history.

**Stack:** TypeScript, Next.js, PostgreSQL, Prisma, QStash.

**Status:** Implemented and locally verified. Hosted application available; complete hosted OAuth, QStash, and recovery acceptance remains pending.

[Hosted application](https://webhooks.mubashirhussain.dev) · [Architecture](https://github.com/mubidotjs/reliable-webhook-platform/blob/main/docs/architecture.md) · [Verification](https://github.com/mubidotjs/reliable-webhook-platform/blob/main/docs/reviews/m4-v1-hardening.md)

### [Ledger Lens](https://github.com/mubidotjs/ai-invoice-receipt-processor)

Processes invoices and receipts through working OCR/PDF extraction, manual document review, and structured exports.

- PDF.js and Tesseract.js process documents in browser memory with bundled assets, avoiding document uploads in the local workflow. File, page, and processing limits bound resource use.
- Decimal-safe arithmetic checks and schema validation guard JSON/CSV exports. Edits reset review; unresolved warnings require acknowledgment, and CSV text is protected against spreadsheet formulas.

**Stack:** React, TypeScript, PDF.js, Tesseract.js, Zod.

**Status:** Public OCR/review/export demo verified. Latest AI acceptance stopped at provider invocation, before output validation; live AI remains disabled with no accepted live-AI workflow.

[Public demo](https://invoice.mubashirhussain.dev) · [Architecture](https://github.com/mubidotjs/ai-invoice-receipt-processor/blob/main/docs/ARCHITECTURE.md) · [Acceptance evidence](https://github.com/mubidotjs/ai-invoice-receipt-processor/blob/main/docs/EVIDENCE-COMPLETENESS.md)

## Engineering Focus

- **AI Application Engineering:** model-backed workflows, structured output validation, source grounding, and evaluation with explicit verification boundaries.
- **Backend & Distributed Systems:** asynchronous jobs, transactional outboxes, idempotency, retry semantics, and recovery from uncertain outcomes.
- **Full-Stack Product Engineering:** usable React/Next.js interfaces, API contracts, data models, and third-party integrations.
- **Production Reliability & Security:** authentication, tenant isolation, bounded resource consumption, automated testing, and deployment checks.

## Technology Stack

- **Languages & UI:** JavaScript, TypeScript, React, Next.js.
- **Backend & APIs:** Node.js, Express, NestJS, REST APIs.
- **Databases & Infrastructure:** PostgreSQL, MongoDB, AWS, Docker, Cloudflare Workers.
- **AI & Evaluation:** Workers AI, Zod, synthetic fixtures, source-evidence checks.
- **Testing & Delivery:** Vitest, Playwright, GitHub Actions, CI/CD.

## Current Exploration

I’m exploring RAG and retrieval evaluation, secure AI agents and tool calling, MCP integrations, AI application security, and production-oriented LLM systems.

## Contact

[Portfolio](https://mubashirhussain.dev) · [Résumé](https://mubashirhussain.dev/resume) · [LinkedIn](https://www.linkedin.com/in/mubashir-leo/) · [mubashir@mubashirhussain.dev](mailto:mubashir@mubashirhussain.dev)
