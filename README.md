# Mubashir Hussain

**Senior Full-Stack Engineer | AI Applications & Backend Systems**

I have 5+ years of professional experience building SaaS applications, APIs, integrations, and backend workflows. My foundation is full-stack/backend engineering, data modeling, and reliable delivery; AI applications are an expanding specialization. I favor correctness, explicit system boundaries, tested failure paths, and clear engineering decisions that make working software easier to ship and maintain.

[Portfolio](https://mubashirhussain.dev) · [Résumé](https://mubashirhussain.dev/resume)

## Featured Engineering

### [PRISM — AI PR Review Agent](https://github.com/mubidotjs/ai-pr-review-agent)

Reviews public GitHub PRs against pinned source evidence and produces suggestions for human approval.

- The backend prepares bounded evidence for one native Gemma inference. Node independently validates supported findings against exact added-line coordinates and the pinned head SHA.
- Vercel Node Functions and a private Workers AI relay enforce authentication and shared admission/quota controls. Human approval unlocks manual-copy Markdown; nothing automatically publishes to GitHub.

**Stack:** React, TypeScript, Node.js, Cloudflare Workers AI, Vercel.

**Status:** Production LIVE; real AI acceptance PASS. Authenticated approval and clipboard PASS used a labeled synthetic replay. Public demo available; live ingestion and real AI require private owner authentication. Coverage is limited to three supported risk categories.

[Live application](https://prism.mubashirhussain.dev) · [Architecture](https://github.com/mubidotjs/ai-pr-review-agent/blob/main/docs/ARCHITECTURE.md) · [Production verification](https://github.com/mubidotjs/ai-pr-review-agent/blob/main/docs/PRODUCTION.md) · [Evidence](https://github.com/mubidotjs/ai-pr-review-agent/blob/main/docs/production-live-result.json)

### [AI Release Notes Generator](https://github.com/mubidotjs/ai-release-notes-generator)

Turns public GitHub comparisons into categorized release notes with inspectable source evidence.

- A Cloudflare Worker ingests public GitHub comparisons and calls native Workers AI/Gemma. Coverage warnings disclose omitted commits; request, prompt, output, and time limits bound inference.
- Strict schemas, retrieved-SHA checks, and exact evidence excerpts reject malformed output and fabricated references. Validated notes export as Markdown; failures surface without automatic retries or paid fallback.

**Stack:** React, TypeScript, Vite, Cloudflare Workers AI, Zod.

**Status:** Production deployed; one real AI generation verified. Sources are commit messages; mechanical grounding does not establish semantic correctness or general model quality.

[Live demo](https://release-notes.mubashirhussain.dev) · [Architecture](https://github.com/mubidotjs/ai-release-notes-generator/blob/main/docs/ARCHITECTURE.md) · [Evaluation](https://github.com/mubidotjs/ai-release-notes-generator/blob/main/docs/EVALUATION.md)

### [Reliable Webhook Platform](https://github.com/mubidotjs/reliable-webhook-platform)

Makes webhook acceptance durable and failed delivery recoverable, with an operations UI for investigation and replay.

- Events, deliveries, and transactional outbox work commit before acknowledgment. Leased workers and stale-worker fencing support recovery with at-least-once delivery.
- Idempotent ingestion, bounded retries, HMAC signing, and tenant isolation protect delivery boundaries. Operational inspection and replay preserve immutable attempt history.

**Stack:** TypeScript, Next.js, PostgreSQL, Prisma, QStash.

**Status:** Implemented and locally verified. Hosted application available; complete hosted OAuth, QStash, and recovery acceptance remains pending.

[Hosted application](https://webhooks.mubashirhussain.dev) · [Architecture](https://github.com/mubidotjs/reliable-webhook-platform/blob/main/docs/architecture.md) · [Verification](https://github.com/mubidotjs/reliable-webhook-platform/blob/main/docs/reviews/m4-v1-hardening.md)

### [Ledger Lens — Invoice & Receipt Processor](https://github.com/mubidotjs/ai-invoice-receipt-processor)

Processes invoices and receipts through working OCR/PDF extraction, manual document review, and structured exports.

- Real PDF text extraction and Tesseract OCR run in browser memory with bundled assets, keeping documents local. File, page, and processing limits bound resource use.
- Decimal-safe arithmetic checks and schema validation guard JSON/CSV exports. Edits reset review; unresolved warnings require acknowledgment, and CSV text is protected against spreadsheet formulas.

**Stack:** React, TypeScript, PDF.js, Tesseract.js, Zod.

**Status:** Public OCR/document-processing demo verified. Live AI extraction remains disabled; no accepted live-AI workflow is claimed.

[Public demo](https://invoice.mubashirhussain.dev) · [Architecture](https://github.com/mubidotjs/ai-invoice-receipt-processor/blob/main/docs/ARCHITECTURE.md) · [Deployment status](https://github.com/mubidotjs/ai-invoice-receipt-processor/blob/main/docs/DEPLOYMENT.md) · [Acceptance evidence](https://github.com/mubidotjs/ai-invoice-receipt-processor/blob/main/docs/EVIDENCE-COMPLETENESS.md)

## Engineering Focus

- **Backend & Distributed Systems:** explicit delivery guarantees, asynchronous workflows, and recovery from uncertain outcomes.
- **Full-Stack Product Engineering:** usable React/Next.js interfaces, API contracts, data models, and third-party integrations.
- **Production Reliability & Security:** tested failure paths, authorization boundaries, maintainable architecture, and deployment checks.
- **AI Application Engineering:** model integration with inspectable evidence, structured validation, and explicit verification boundaries.

## Technology Stack

- **Languages & UI:** JavaScript, TypeScript, React, Next.js.
- **Backend & APIs:** Node.js, Express, NestJS, REST APIs.
- **Data:** PostgreSQL, MongoDB.
- **Infrastructure:** AWS, Docker, Cloudflare Workers, Vercel.
- **AI Applications:** native Workers AI, model integration, structured validation, source grounding, bounded workflows.
- **Testing & Delivery:** Vitest, Playwright, GitHub Actions, CI/CD.

## Current Exploration

I’m exploring RAG and retrieval evaluation, secure AI agents and tool calling, MCP integrations, AI application security, and production-oriented LLM systems.

## Contact

[Portfolio](https://mubashirhussain.dev) · [Résumé](https://mubashirhussain.dev/resume) · [LinkedIn](https://www.linkedin.com/in/mubashir-leo/) · [mubashir@mubashirhussain.dev](mailto:mubashir@mubashirhussain.dev)
