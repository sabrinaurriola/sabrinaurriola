# Sabrina Urriola Vergara

### AI & Automation Consultant | Business Process Improvement | AI Solution Integration

Food Engineer based in Île-de-France, with eight years of industrial experience in product and process development, quality, and project coordination. I am extending that background into AI consulting and automation: analysing operational problems, identifying where AI or automation is appropriate, designing solutions, building and evaluating prototypes, and working with technical teams on implementation.

Languages: Spanish, English, French. Open to on-site or hybrid roles in France, or remote roles.

[LinkedIn](https://www.linkedin.com/in/sabrina-urriola-vergara/) · [GitHub](https://github.com/sabrinaurriola)

## From business analysis to technical delivery

- **Frame the problem.** Start from the process, the users, and the constraints before choosing a technology.
- **Place AI deliberately.** Keep calculations, state changes, and business rules deterministic; use AI for retrieval, drafting, and interpretation, with human review where decisions matter.
- **Build and test incrementally.** Prototype with Python, n8n, Make, and Airtable; validate with tests; document what works, what is planned, and what is not yet proven.
- **Collaborate across disciplines.** Translate between business stakeholders and technical specialists, as I did for years between commercial teams, R&D, production, and quality.

## Experience

**AI and automation projects (portfolio, 2026).** Four self-directed projects built during my transition, summarised below. They are prototypes and case studies, not paid client engagements, production deployments, or measured business results.

**Career transition, Aug 2025 – present.** Training in AI consulting: AI Consulting Bootcamp, Ironhack (in progress, until December 2026); Product Builder No-Code, RNCP 39108 BC03 (Make, Airtable, 2026); Google Data Analytics Professional Certificate (2026).

**Previous professional experience: Symrise AG, 2016 – 2025 (8 yrs 8 mos).** Progression through product and process roles, mainly in aquaculture feed, then fruit and vegetable ingredients:

- R&D Product Development Project Manager, Naturals – Fruits & Vegetables (Rennes, 2025): turned commercial requirements into development plans and defined scope for pilot and industrial trials.
- Product and Process Development Manager, Aqua Feed (2021 – 2025): turned business needs into technical specifications and assessed industrial feasibility.
- Quality Manager, Aqua Feed (2020 – 2021): led root-cause analysis of non-conformities and coordinated quality control and supplier audits.
- Product and Process Engineer, Aqua Feed (2016 – 2020): led product development and industrialisation from pilot trials to scale-up.

**Education.** Master's in Production Management & Process Improvement, OBS Business School (2021); Lean Six Sigma Green Belt, ESPOL (2020); Engineer's degree in Food Technology and Processing, ESPOL (2016).

## Portfolio projects

### 1. Procurement Risk & Mitigation Agent

**Problem.** A procurement manager must connect market news to the company's own contracts and forecasts to judge exposure to commodity price moves. Doing this by hand across news, price data, contracts, and policies is slow and error-prone.

**Solution.** A LangGraph agent researches market signals, retrieves internal policies (RAG), calculates exposure deterministically in Python, and drafts an evidence-backed risk and mitigation report. Claims without a supporting source are removed visibly. n8n archives completed reports in Notion and e-mails the PDF on request.

**Demonstrates.** Agent workflow design, RAG, deterministic calculations, evidence validation, human oversight, integration with business tools.

**Status.** Working PoC for one raw material (sunflower oil); other commodities are placeholders. The company, contracts, and forecasts are fictional; market data is real. Offline tests pass with mocked services, and live runs were executed in November 2026 (most ended "partial" because validation removed unsupported items, as intended). It is decision support only. No accuracy, time-saving, or user-validation results exist.


[README](https://github.com/sabrinaurriola/procurement-risk-and-mitigation-ai-agent/blob/main/README.md) ·  [Repository](https://github.com/sabrinaurriola/procurement-risk-and-mitigation-ai-agent) · [Loom walkthrough](https://www.loom.com/share/3f1675d6e96b41f098145668226c3a26) 

### 2. AI-Powered IT Service Desk

**Problem.** In a simulated company of 150 employees, a three-person IT team handles requests through Slack and e-mail, logs them by hand, and answers recurring questions repeatedly. Volumes and pain points are case-study assumptions.

**Solution.** A Slack, n8n, and Airtable workflow that registers each request, creates traceable tickets, and is designed to offer a RAG-based answer from approved documentation, with escalation to a technician. Ticketing is deterministic and idempotent; the AI never changes state or creates tickets.

**Demonstrates.** Scoping an MVP, data-model and workflow design, idempotency and failure handling, clear boundaries for AI use, and evaluation criteria defined before building.

**Status: work in progress.** *Built and tested:* Airtable data model, Slack intake (tested end to end on a live webhook), and ticket creation (tested standalone with controlled inputs). *Designed, not built:* button interactions, the RAG answer path, document ingestion, timeouts, and offline RAG evaluation. Slack signature verification and concurrent execution are unverified. No service-desk outcomes are claimed.

[Repository](https://github.com/sabrinaurriola/ai-powered-it-service-desk)  [README](https://github.com/sabrinaurriola/ai-powered-it-service-desk/blob/main/README.md)

### 3. FutureTech Marketing Intelligence Platform (Campaign OS)

**Problem.** Marketing managers and executives need decisions, not only dashboards, from campaign data that is inconsistent and slow to turn into weekly reporting.

**Solution.** A Python platform that cleans campaign data, computes KPIs in a deterministic analytics engine, and passes validated facts to a provider-agnostic AI layer (Mock for development and CI, Anthropic Claude validated end to end) that writes the executive narrative. Outputs feed a Power BI report, an executive e-mail sent through n8n, and a full Markdown report.

**Demonstrates.** Stable data contracts between layers, an LLM that interprets but never calculates, provider abstraction, BI reporting, and automation through n8n.

**Status.** MVP (v1.0.0) runs end to end on simulated data (32,800 rows), on demand through an n8n form trigger. A real SMTP send was validated. Scheduled execution is not implemented. Retry/backoff and cost monitoring are planned for later sprints, and cost and latency have not been benchmarked at scale. Results do not reflect real client impact.

[Repository](https://github.com/sabrinaurriola/futuretech-marketing-intelligence-platform) · 📄 [Case study](https://github.com/sabrinaurriola/futuretech-marketing-intelligence-platform/blob/main/case-study/FutureTech_Marketing_Intelligence_Platform_Case_Study.pdf)

### 4. NeoBâti Operations System

**Problem.** A construction company (Atelier NéoBâti, a fictional case-study client) needed one shared way to manage the path from customer request and quote through delivery, field reporting, purchases, incidents, and invoicing.

**Solution.** A no-code/low-code operations system: a relational Airtable data model, 12 Airtable automations, five Make scenarios, four role-specific interfaces (Administration, Sales, Management, Field Artisan), and operational and financial dashboards. AI drafts visit summaries and reminders within business rules; invoice reminders require explicit human confirmation.

**Demonstrates.** Business discovery and process analysis, solution and data-model design, no-code/low-code implementation, workflow automation, error handling, and human oversight of AI.

**Status: completed** as a designed, implemented, and tested solution, documented in a final written dossier. 

[Repository](https://github.com/sabrinaurriola/NEOBATI-Operations-System) ·  [README](https://github.com/sabrinaurriola/NEOBATI-Operations-System/blob/main/README.md)

## Toolkit

**AI and orchestration:** Python, LLM APIs (OpenAI, Anthropic), LangChain, LangGraph, RAG, n8n, Make  
**Data and integration:** PostgreSQL / Supabase, Airtable, Slack, REST APIs and webhooks, Notion  
**Analytics and reporting:** pandas, Power BI  
**Practice:** process analysis, workflow design, model evaluation and testing, human-in-the-loop controls, error handling, technical documentation
