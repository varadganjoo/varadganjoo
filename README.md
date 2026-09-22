# Varad Ganjoo

**AI Systems & Software Engineer** | Melbourne, Australia  
[LinkedIn](https://www.linkedin.com/in/varad-ganjoo-3137631b2/) · [Email](mailto:varadganjoo@gmail.com)

I build reliable, deterministic AI systems with durable state machines, AST-enforced security guards, and human-in-the-loop workflows. My focus is on making generative AI dependable in production environments where hallucinations and unconstrained execution are unacceptable.

---

## Featured Projects

### 🏥 [CareFlow Clinical Agent](https://github.com/varadganjoo/careflow-clinical-agent)
Enterprise clinical decision support and EHR documentation platform built on a durable LangGraph state machine.
- **Deterministic Pharmacological Safety Engine**: Code-level invariants running before LLM generation that block contraindicated medication combinations (e.g., dual RAS blockade) and flag critical lab thresholds (hyperkalemia, severe CKD).
- **Clinical Practice Guidelines**: Formalized ACC/AHA 2024 hypertension and ADA 2025/2026 diabetes standards.
- **Human-in-the-Loop Review Gate**: Uses LangGraph `interrupt()` to enforce mandatory physician sign-off before committing clinical notes to the EHR.

### ⚙️ [Enterprise AI Systems Engineering Suite](https://github.com/varadganjoo/enterprise-ai-systems)
A suite of 9 independent, production-grade AI systems with deterministic guardrails, state-machine orchestration, and evals-as-code:
- **01 Cited Knowledge Agent**: Verifiable grounding with character-level span offsets and temporal policy supersession.
- **02 Document Extraction**: Accounting reconciler verifying line-item math and routing low-confidence scans to human triage.
- **03 Operator Agent**: Stateful operator with tool allowlists, PII/credential guardrails, and supervisor approval queues.
- **04 Analytics Copilot**: Read-only SQL copilot enforcing AST validation via `sqlglot` (SELECT-only, table allowlist, row limits).
- **05 Model Router**: Multi-tiered semantic router triaging simple queries to lightweight models and complex reasoning to frontier models.
- **06 Memory Service**: Entity slot memory with deterministic supersession tracking and bidirectional PII redaction token vault.
- **07 Claim Auditor**: Atomic proposition fact-checking computing evidence-based verdicts against governing documents.
- **08 Case Workflow**: Event-sourced refund state machine with idempotent processing and hard financial category caps.
- **09 Multi-Hop Brief**: DAG-based multi-document reasoning that gates final conclusions if intermediate hops lack citations.

### 🎙️ [Real-Time Voice & Vision Assistant](https://github.com/varadganjoo/realtime-voice-and-vision-assistant)
A low-latency desktop voice assistant for Windows integrating real-time speech transcription, Groq Vision AI, system automation tools, and text-to-speech feedback.

### 📝 [Real-Time Speech Transcription](https://github.com/varadganjoo/Real-Time-Speech-Transcription)
Streaming audio transcription pipeline that utilizes generative AI to correct grammar in real time and fill missing words without hallucinating context.

---

## Technical Stack

- **Core Languages**: Python, TypeScript, SQL
- **AI & Orchestration**: LangGraph, LangChain, Pydantic, Model Context Protocol (MCP), Gemini SDK
- **Backend & Data**: FastAPI, SQLite, PostgreSQL, `sqlglot`
- **Frontend & Visualization**: Modern HTML5/Tailwind CSS, React, Chart.js
- **Engineering Rigor**: Unit testing (`pytest`), evals-as-code, AST analysis, CI/CD with GitHub Actions
