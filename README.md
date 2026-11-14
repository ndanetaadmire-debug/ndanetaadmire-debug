<div align="center">

# Admire T. Ndaneta

### Full-Stack Engineer | AI & Agentic Systems Engineer

**AI agents · Scalable SaaS · Real revenue**
6+ years owning production products end to end across healthcare, energy, financial services and e-commerce. Remote, South Africa.

[![Portfolio](https://img.shields.io/badge/Portfolio-admire--portfolio.vercel.app-111827?style=for-the-badge&logo=vercel&logoColor=white)](https://admire-portfolio.vercel.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Admire_Ndaneta-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/admire-ndaneta-a3272711a)
[![Email](https://img.shields.io/badge/Email-ndanetaadmire%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ndanetaadmire@gmail.com)
[![Talk to Victor](https://img.shields.io/badge/Talk_to_my_AI_agent-Victor-7C3AED?style=for-the-badge&logo=probot&logoColor=white)](https://admire-portfolio.vercel.app)

</div>

---

## 👨🏽‍💻 About me

I'm a **Senior Full-Stack Engineer, Product Owner and Tech Lead** at **Gerko**, where I lead the product and architecture of a multi-tenant healthcare practice-management SaaS, report to the CTO and lead a team of three developers. I co-architected **Scribe**, the platform's AI clinical co-pilot.

I design **agentic AI systems that run in production**: stateful LangGraph agents with typed tools, deterministic guardrails, human-in-the-loop checkpoints and streaming UIs. I also own the SaaS around them: data models, APIs, performance, CI/CD and the people who ship it.

<table>
<tr>
<td align="center"><h3>6+</h3>years shipping production code</td>
<td align="center"><h3>4</h3>AI & agentic systems live in production</td>
<td align="center"><h3>99.9%</h3>uptime delivered</td>
<td align="center"><h3>35%</h3>faster page loads at Gerko</td>
</tr>
<tr>
<td align="center"><h3>20%</h3>gain in dev velocity</td>
<td align="center"><h3>15%</h3>fewer regressions</td>
<td align="center"><h3>3</h3>developers led and mentored</td>
<td align="center"><h3>18</h3>projects shipped</td>
</tr>
</table>

---

## 🤖 Agentic AI systems in production

### Victor: autonomous AI representative · [live on my portfolio](https://admire-portfolio.vercel.app) · [case study](https://admire-portfolio.vercel.app/projects/victor) · [code](https://github.com/ndanetaadmire-debug/victor-ai-agent)
A 24/7 agent that represents me to recruiters and clients. It reasons over my career, maps job specs to evidence, scopes client builds, demos live code in the chat and books interviews.
- **LangGraph.js state graph:** a deterministic security gate (blocks prompt injection and jailbreaks before any tokens are spent) → reasoning planner → bounded multi-tool loop → sanitised SSE streaming with a visible step trace
- **7 Zod-typed tools:** profile, experience, project search, JD-fit analysis, scope estimation, CV delivery and booking
- **Hard booking guardrails:** contact details are verified against the conversation, and false "you're booked" claims are intercepted and corrected mid-stream
- **Generative UI:** whitelisted markers render live React demos, case-study cards and a booking form inside the chat
- **Model-agnostic setup:** recovers from malformed tool calls and is tested offline against the real graph with a scripted model

`TypeScript` `LangGraph.js` `LangChain.js` `Next.js 16` `React 19` `Groq · GPT-OSS` `Zod` `SSE` `Web Speech API` `Tailwind v4` `Resend` `Vercel Fluid Compute` `Playwright`

### Scribe: AI clinical guide & co-pilot (Gerko) · [case study](https://admire-portfolio.vercel.app/projects/scribe) · [how it works: open demo](https://github.com/ndanetaadmire-debug/realtime-clinical-notes-demo)
Gerko's flagship AI feature. It analyses clinician speech in real time, produces structured clinical observations and cuts consultation documentation time.
`Node.js` `Fastify` `Redis` `WebSockets`

### Lwazi Hair: AI e-commerce operations agent · [case study](https://admire-portfolio.vercel.app/projects/lwazi-hair-agent) · [code](https://github.com/ndanetaadmire-debug/commerce-ops-agent)
A customer-operations agent for a live retailer. It checks stock, tracks orders, estimates delivery and routes refund escalations to a human.
`TypeScript` `LangGraph.js` `Groq · Llama 3.3` `Webhooks` `Shopify`

### Finance & accounting workflow engine · [case study](https://admire-portfolio.vercel.app/projects/finance-workflow-engine) · [code](https://github.com/ndanetaadmire-debug/finance-workflow-engine)
Automates invoice ingestion, OCR parsing, field-extraction validation, reconciliation and exception handling, with a human in the loop for anything uncertain.
`Python` `C# / .NET Core` `Fastify` `Redis` `PostgreSQL`

### 🧰 AI engineering toolkit (open source)

The infrastructure that makes agents trustworthy in production: guardrails, evaluation, retrieval, tool protocols and orchestration.

| Repo | What it is |
|---|---|
| [llm-guardrails-kit](https://github.com/ndanetaadmire-debug/llm-guardrails-kit) | Prompt-injection scoring, reversible PII redaction with checksums, tool-call policy, ledger-checked claims. CI gates recall and precision on a labelled attack corpus |
| [agent-eval-harness](https://github.com/ndanetaadmire-debug/agent-eval-harness) | Regression testing for agents: tool-trajectory, grounded-number and PII-leak scorers, repeated runs to expose flakiness, baseline gate in CI |
| [rag-knowledge-agent](https://github.com/ndanetaadmire-debug/rag-knowledge-agent-) | Permission-aware RAG: hybrid BM25 + dense retrieval with RRF and MMR, cited answers, grounding verifier, refuses when evidence is weak |
| [mcp-commerce-server](https://github.com/ndanetaadmire-debug/mcp-commerce-server-) | Model Context Protocol server with scoped keys, PII masking and HMAC-bound preview-then-confirm for every write |
| [multi-agent-research-crew](https://github.com/ndanetaadmire-debug/multi-agent-research-crew) | LangGraph planner → parallel researchers → critic → writer, with every citation verified in code and token budgets |
| [voice-booking-agent](https://github.com/ndanetaadmire-debug/voice-booking-agent) | Phone receptionist on Twilio: spoken date/time parsing, low-confidence recovery, keypad fallback, human handoff |
| [ai-invoice-extractor](https://github.com/ndanetaadmire-debug/ai-invoice-extractor) | LLM extraction with evidence spans checked against the document, repair loop, model fallback and a field-accuracy gate |
| [resilient-http-client](https://github.com/ndanetaadmire-debug/axios) | Typed HTTP client on native fetch for calling flaky APIs: jittered retries that respect Retry-After and idempotency, per-host circuit breakers, stale-if-error caching. Zero dependencies |

---

## 🏥 Production SaaS & commerce

| Product | What it is | Stack | Links |
|---|---|---|---|
| **Gerko** | All-in-one practice management for health practitioners: scheduling, patient records, billing, reviews and an AI medical scribe | React · TypeScript · Node.js · Fastify · PostgreSQL · Redis | [app.gerko.io](https://app.gerko.io) · [case study](https://admire-portfolio.vercel.app/projects/gerko) |
| **Lwazi Hair** | Live Shopify store with a custom wig and bundle builder, live pricing and real orders | Shopify · Liquid · JavaScript · Yoco Payments | [lwazihair.co.za](https://lwazihair.co.za) · [case study](https://admire-portfolio.vercel.app/projects/lwazi-hair) |
| **Respectful** *(MVP in active development)* | Privacy-first dating, marriage and family platform: transparent two-sided matching, Row Level Security on every table, couples and family journeys on the roadmap | Next.js 16 · Supabase · PostgreSQL RLS · Vitest · Storybook | [case study](https://github.com/ndanetaadmire-debug/respectful-platform-case-study) · app repo private |

### 🌍 Client websites: redesign & build

| Client | Sector | Live site |
|---|---|---|
| **Girteka** | Asset-based logistics, Europe | [girteka.eu](https://www.girteka.eu/) |
| **Corteva Agriscience Canada** | Agriculture, Canada | [corteva.com/ca-en](https://www.corteva.com/ca-en/) |
| **NUST** | Higher education, Pakistan | [nust.edu.pk](https://nust.edu.pk/) |
| **Focus Grid** | Tech talent & digital products | [focusgrid.net](https://www.focusgrid.net/) |

### 🧩 Full-stack product builds

| Project | Domain | Highlights | Code |
|---|---|---|---|
| **FinanceFlow** | Fintech | Double-entry ledger in Go: optimistic concurrency, idempotent transfers, immutable history, race- and property-tested | [repo](https://github.com/ndanetaadmire-debug/financeflow) |
| **ShopSphere** | E-commerce | Checkout backend: VAT-correct pricing, oversell-proof reservations, payment saga with compensations, transactional outbox | [repo](https://github.com/ndanetaadmire-debug/shopsphere) |
| **FleetFlow** | Logistics & field ops | Real-time dispatch: regret-2 assignment, event-sourced jobs, geofenced arrivals, resumable WebSocket streams | [repo](https://github.com/ndanetaadmire-debug/fleetflow) |
| **LearnHub** | EdTech | Accessible React 19 course player: SM-2 spaced repetition, partial-credit grading, keyboard-only tested | [repo](https://github.com/ndanetaadmire-debug/learnhub) |
| **PropManage** | PropTech | Leases with proration and escalation, payment allocation, arrears ageing, SLA-tracked maintenance | [repo](https://github.com/ndanetaadmire-debug/propmanage) |
| **TalentHub** | HR / People Ops | Fair, POPIA-compliant hiring in Go: blind screening, structured scorecards, four-fifths monitoring, retention and erasure | [repo](https://github.com/ndanetaadmire-debug/talenthub) |
| **Knights-Nestlé MS** | Retail execution | Merchandiser visit planning (tiers, spacing, 2-opt routing), geofenced check-ins, on-shelf availability | [engine](https://github.com/ndanetaadmire-debug/retail-merch-scheduler) |
| **VibeCheck** | Content / social | Mood-based blogging with a custom Markdown renderer that is XSS-safe by construction | [repo](https://github.com/ndanetaadmire-debug/vibecheck) |
| **Restaurant Ops** | Hospitality | Ordering and kitchen display: server-side pricing, a state machine enforced in code and in Postgres, session-authorised realtime | [repo](https://github.com/ndanetaadmire-debug/Full-stack-restaurant-app) |
| **Investment calculator** | Personal finance | SA savings planner: monthly compounding in cents, fees, inflation, TFSA limits, cent-exact goal solver | [repo](https://github.com/ndanetaadmire-debug/investment-calculator) |
| **Read along** | Accessibility | Text-to-speech reader that highlights each word as it is spoken, with click-to-seek and a timing fallback | [repo](https://github.com/ndanetaadmire-debug/speechify-assessment) |
| **Engineering notes** | Content | Next.js App Router blog: validated Markdown, sanitized rendering, RSS, sitemap, JSON-LD | [repo](https://github.com/ndanetaadmire-debug/nextjsp1) |

### 🔬 Engineering showcase: what each repo proves

Every repo below ships with an architecture write-up, CI, and tests that prove the guarantees it claims, not just the happy path.

| Repo | Stack | What the tests prove |
|---|---|---|
| [victor-ai-agent](https://github.com/ndanetaadmire-debug/victor-ai-agent) | TypeScript · LangGraph.js · Fastify | Jailbreaks are blocked before the model runs; false "you're booked" claims are caught; contact details are never guessed |
| [commerce-ops-agent](https://github.com/ndanetaadmire-debug/commerce-ops-agent) | TypeScript · LangGraph.js · Shopify GraphQL | Refunds can't be promised without approval; orders can't be enumerated; HMAC-verified, idempotent webhooks |
| [finance-workflow-engine](https://github.com/ndanetaadmire-debug/finance-workflow-engine) | Python · FastAPI · PostgreSQL | Bank-detail fraud, duplicates and 3-way-match failures go to a human; audit-log tampering is detectable |
| [financeflow](https://github.com/ndanetaadmire-debug/financeflow) | Go (stdlib only) · PostgreSQL | 200 concurrent spends never overdraw; 2,000 random transfers always net to zero; the DB rejects unbalanced entries |
| [shopsphere](https://github.com/ndanetaadmire-debug/shopsphere) | TypeScript · Fastify | The last unit goes to exactly one buyer; discounts never lose a cent; late payments are re-reserved or auto-refunded |
| [fleetflow](https://github.com/ndanetaadmire-debug/fleetflow) | TypeScript · WebSockets · event sourcing | Regret assignment beats greedy; the projection equals a replay of events; tenants never see each other's streams |
| [propmanage](https://github.com/ndanetaadmire-debug/propmanage) | Python · SQLAlchemy 2.0 | A unit can't be double-let; rent prorates and escalates correctly; billing is idempotent at the DB level |
| [learnhub](https://github.com/ndanetaadmire-debug/learnhub) | React 19 · TypeScript · Vite | The quiz works with the keyboard alone; corrupt saved state can't crash the player; "select all" scores zero |
| [llm-guardrails-kit](https://github.com/ndanetaadmire-debug/llm-guardrails-kit) | TypeScript · Zod | 20/20 obfuscated attacks caught (homoglyphs, zero-width, base64) with 0 false positives; unbacked claims are corrected |
| [agent-eval-harness](https://github.com/ndanetaadmire-debug/agent-eval-harness) | Python (stdlib) | Flaky agents fail; invented numbers and PII leaks are caught; a regressed agent fails the build |
| [rag-knowledge-agent](https://github.com/ndanetaadmire-debug/rag-knowledge-agent-) | Python · FastAPI | Recall@4 100%; restricted documents never reach unauthorised users; a hallucinating generator is refused |
| [mcp-commerce-server](https://github.com/ndanetaadmire-debug/mcp-commerce-server-) | TypeScript · MCP SDK | A write can't skip its preview, swap its arguments or replay an approval; PII is masked without the right scope |
| [multi-agent-research-crew](https://github.com/ndanetaadmire-debug/multi-agent-research-crew) | TypeScript · LangGraph.js | Invented URLs and numbers are dropped and disclosed; the revision loop and token budget are bounded |
| [voice-booking-agent](https://github.com/ndanetaadmire-debug/voice-booking-agent) | TypeScript · Twilio | 38 tests on how people really say dates and times; races and webhook retries can't double-book |
| [ai-invoice-extractor](https://github.com/ndanetaadmire-debug/ai-invoice-extractor) | Python · Pydantic | A hallucinated total is caught by the evidence check; nothing unverified is auto-approved |
| [talenthub](https://github.com/ndanetaadmire-debug/talenthub) | Go (stdlib only) | Reviewers can't see identity at screening; offers need two evidenced scorecards; POPIA retention runs on time |
| [retail-merch-scheduler](https://github.com/ndanetaadmire-debug/retail-merch-scheduler) | Python | Tier frequencies met with no back-to-back visits; stock data comes only from geofenced, photo-verified visits |
| [vibecheck](https://github.com/ndanetaadmire-debug/vibecheck) | React 19 · TypeScript | A table of real XSS payloads renders as harmless text |
| [realtime-clinical-notes-demo](https://github.com/ndanetaadmire-debug/realtime-clinical-notes-demo) | TypeScript · WebSockets | Every note line cites its transcript; a penicillin–amoxicillin conflict blocks sign-off; logs are PHI-free |
| [respectful-platform-case-study](https://github.com/ndanetaadmire-debug/respectful-platform-case-study) | SQL · PGlite · TypeScript | RLS policies withstand cross-user attacks against real Postgres; matching is two-sided and explainable |
| [restaurant-ops-platform](https://github.com/ndanetaadmire-debug/Full-stack-restaurant-app) | TypeScript · Express 5 · Socket.IO · PostgreSQL | Client prices are ignored; a Postgres trigger blocks illegal status jumps; customers never receive each other's order events |
| [resilient-http-client](https://github.com/ndanetaadmire-debug/axios) | TypeScript · native fetch | A dead upstream trips the breaker and stops being called; a POST is never retried without an idempotency key |
| [investment-calculator](https://github.com/ndanetaadmire-debug/investment-calculator) | React 19 · TypeScript · fast-check | Totals reconcile to the cent on thousands of random plans; TFSA limits are never exceeded |
| [read-along](https://github.com/ndanetaadmire-debug/speechify-assessment) | React 19 · Web Speech API | Stale events from cancelled speech never skip ahead; highlighting survives voices without word boundaries |
| [nextjs-engineering-blog](https://github.com/ndanetaadmire-debug/nextjsp1) | Next.js 16 · TypeScript | Hostile Markdown is sanitized; a malformed post fails the build; unknown slugs are 404s, never file reads |


---

## 🛠️ Tech stack

**AI & agents**
![LangGraph](https://img.shields.io/badge/LangGraph.js-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain.js-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square)
![Llama](https://img.shields.io/badge/Llama_3.3-0467DF?style=flat-square&logo=meta&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-336791?style=flat-square&logo=postgresql&logoColor=white)
![Zod](https://img.shields.io/badge/Zod-3E67B1?style=flat-square&logo=zod&logoColor=white)

**Front end**
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Webpack](https://img.shields.io/badge/Webpack-8DD6F9?style=flat-square&logo=webpack&logoColor=black)

**Back end & data**
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=flat-square&logo=fastify&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![.NET](https://img.shields.io/badge/C%23_/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=flat-square&logo=socketdotio&logoColor=white)

**Cloud, quality & delivery**
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![Shopify](https://img.shields.io/badge/Shopify-7AB55C?style=flat-square&logo=shopify&logoColor=white)

---

## 🧭 How I build

- **Agents are software, not prompts.** I use typed tool contracts, deterministic guardrails before the model, bounded loops, offline tests against the real graph and human-in-the-loop checkpoints wherever money or health is involved.
- **Security and privacy first.** Row Level Security on every table, nonce-based CSP, rate limits, no secrets in code and no personal data in analytics.
- **Built to scale from day one.** Keyset pagination, idempotent writes, partition-ready hot tables and stateless services, without premature infrastructure.
- **Ownership end to end.** From discovery and architecture to CI/CD, observability and mentoring the team that ships it.

---

## 📈 Activity

<div align="center">

![GitHub stats](https://github-readme-stats.vercel.app/api?username=ndanetaadmire-debug&show_icons=true&count_private=true&include_all_commits=true&hide_border=true&theme=transparent)
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=ndanetaadmire-debug&layout=compact&hide_border=true&theme=transparent)

![Streak](https://streak-stats.demolab.com?user=ndanetaadmire-debug&hide_border=true&theme=transparent)

</div>

---

<div align="center">

**Open to senior full-stack and AI/agentic engineering roles, and to client builds.**
The fastest way to check fit: [ask Victor](https://admire-portfolio.vercel.app). He has read my whole career.

</div>
