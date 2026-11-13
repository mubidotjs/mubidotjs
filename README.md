# Mubashir Hussain

**Senior Full-Stack Engineer | AI Applications & Backend Systems**

I have 5+ years of experience building SaaS products, APIs, integrations, and backend workflows that connect usable interfaces with dependable services. My foundation is full-stack and backend engineering, from data modeling and transactional behavior to operational tooling. I apply the same priorities to AI applications: correctness, reliability, maintainability, and software that works under real-world constraints.

[Portfolio](https://mubashirhussain.dev) · [Résumé](https://mubashirhussain.dev/resume)

## Featured Engineering

### [AI Release Notes Generator](https://github.com/mubidotjs/ai-release-notes-generator)

GitHub comparisons become categorized, structured release notes, with source evidence exposed for human review rather than untraceable generated summaries. The application supports a clearly labeled synthetic demo alongside its separate live generation path.

- Validates model output with Zod, retrieved commit SHAs, and exact excerpts from the supplied commit messages; rejects unsupported references.
- Bounds input, inference, and response handling, with explicit rate limits, timeout paths, and error states rather than silent fallbacks. Markdown export is generated from validated data.

**Stack:** React, TypeScript, Vite, Cloudflare Workers AI, Zod.\
**Links:** [Live demo](https://release-notes.mubashirhussain.dev) · [Architecture](https://github.com/mubidotjs/ai-release-notes-generator/blob/main/docs/ARCHITECTURE.md) · [Evaluation](https://github.com/mubidotjs/ai-release-notes-generator/blob/main/docs/EVALUATION.md).\
**Status:** Live AI integration was demonstrated on one documented example. Grounding uses commit messages, not code semantics; semantic correctness and general model quality remain unproven.

### [Reliable Webhook Platform](https://github.com/mubidotjs/reliable-webhook-platform)

Webhook delivery must survive interrupted publication and worker failures without acknowledging events that have not been durably accepted.

- Commits events and outbox work before acknowledgment; uses idempotency, leased recovery, bounded retries, and immutable delivery-attempt history. Replay preserves prior attempts for auditability.
- Protects outgoing deliveries with HMAC signing and scopes application access and persisted records to authenticated tenants.

**Stack:** TypeScript, Next.js, PostgreSQL, Prisma, QStash.\
**Links:** [Hosted app](https://webhooks.mubashirhussain.dev) · [Architecture](https://github.com/mubidotjs/reliable-webhook-platform/blob/main/docs/architecture.md) · [Release verification](https://github.com/mubidotjs/reliable-webhook-platform/blob/main/docs/reviews/m4-v1-hardening.md).\
**Status:** Implementation is locally verified; complete hosted OAuth, QStash, and recovery acceptance remains pending.

### [Ledger Lens — Invoice & Receipt Processor](https://github.com/mubidotjs/ai-invoice-receipt-processor)

Document extraction is only useful when uncertain financial fields can be inspected, corrected, and exported safely.

- Extracts native PDF text or runs browser-local OCR, preserving document previews and a manual structured-review workflow. Raw uploaded documents stay in browser memory.
- Applies decimal-safe arithmetic checks, revision-aware review gates, and spreadsheet-safe CSV export with corrected-field provenance.

**Stack:** React, TypeScript, PDF.js, Tesseract.js, Zod.\
**Links:** [Public demo](https://invoice.mubashirhussain.dev) · [Architecture](https://github.com/mubidotjs/ai-invoice-receipt-processor/blob/main/docs/ARCHITECTURE.md) · [Acceptance evidence](https://github.com/mubidotjs/ai-invoice-receipt-processor/blob/main/docs/EVIDENCE-COMPLETENESS.md).\
**Status:** Live AI is disabled after unsuccessful model acceptance; OCR, manual review, and exports work.

## Engineering Focus

- **AI Application Engineering:** grounded model outputs, strict schemas, source-evidence validation, bounded inference, and documented evaluation limits rather than unsupported accuracy claims.
- **Backend & Distributed Systems:** durable asynchronous processing, transactional boundaries, idempotency, retries, and recoverable background work under interruption and partial failures.
- **Full-Stack Product Engineering:** accessible React interfaces, REST APIs, database modeling, workflow design, and integration-focused SaaS features shaped around operator and end-user needs.
- **Production Reliability & Security:** authentication, tenant isolation, signed requests, failure-path testing, CI, release verification, and cautious deployment gates with clearly recorded acceptance boundaries.

## Technology Stack

Tools used across professional work and the linked projects, selected for clear contracts, testability, and maintainable delivery.

- **Languages & UI:** JavaScript, TypeScript, React, Next.js.
- **Backend & APIs:** Node.js, Express, NestJS, REST APIs.
- **Databases & Infrastructure:** PostgreSQL, MongoDB, AWS, Docker, Cloudflare Workers.
- **AI & Evaluation:** Workers AI, Zod, synthetic fixtures, source-evidence checks.
- **Testing & Delivery:** Vitest, Playwright, GitHub Actions, CI/CD.

## Current Exploration

Exploring RAG and retrieval evaluation, secure agents and tool calling, MCP integrations, AI application security, and production LLM systems. These are active learning and build directions, not claims of shipped agent or retrieval platforms. Future work will be promoted here only with implementation and verification evidence.

## Contact

[Portfolio](https://mubashirhussain.dev) · [Résumé](https://mubashirhussain.dev/resume) · [LinkedIn](https://www.linkedin.com/in/mubashir-leo/) · [Email](mailto:mubashir@mubashirhussain.dev)
