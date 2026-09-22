# Varad Ganjoo

**AI Systems & Software Engineer** | Texas, United States  
[LinkedIn](https://www.linkedin.com/in/varad-ganjoo-3137631b2/) · [Email](mailto:varadganjoo@gmail.com)

I build reliable, deterministic AI systems with durable state machines, AST-enforced security guards, and human-in-the-loop workflows. My focus is on making generative AI dependable in enterprise environments where hallucinations and unconstrained execution are unacceptable.

---

## Featured Projects

### 🧠 [Baby LLM](https://github.com/varadganjoo/baby-llm)
An experimental language model and continuous learning platform built from scratch in PyTorch.
- **Incremental Learning Architecture**: Explores continuous language acquisition through dynamic n-gram memory, adaptive token embeddings, and a PyTorch GRU with multi-head attention.
- **Interactive CLI & Training Harness**: Supports incremental ingestion from text corpora and web crawls, human feedback loops, replay buffers, and GPU execution controls.

### 🏥 [CareFlow Clinical Agent](https://github.com/varadganjoo/careflow-clinical-agent)
Clinical decision support and EHR documentation platform built on a durable LangGraph state machine.
- **Deterministic Pharmacological Safety Engine**: Code-level invariants running before LLM generation that block contraindicated medication combinations (e.g., dual RAS blockade) and flag critical lab thresholds (hyperkalemia, severe CKD).
- **Clinical Practice Guidelines**: Formalized ACC/AHA hypertension and ADA diabetes standards with verbatim citation verification.
- **Human-in-the-Loop Review Gate**: Uses LangGraph `interrupt()` to enforce mandatory physician sign-off before committing clinical notes to the EHR.

### 📈 [Apex-Alpha](https://github.com/varadganjoo/apex-alpha)
Quantitative forecasting and multi-agent investment committee platform with streaming consensus debate.
- **Adversarial Multi-Agent Debate**: Bull Equity Analyst and Bear Risk Officer agents debate asset allocations grounded in SEC disclosures.
- **Quantitative Engine**: 10,000-path Monte Carlo price path simulations with Kelly criterion position sizing and parametric Value at Risk (VaR).
- **Portfolio Manager Review Gate**: Stateful LangGraph workflow with deterministic circuit breakers pausing high-volatility allocations for human sign-off.

### 🛡️ [Aegis SRE](https://github.com/varadganjoo/aegis-sre)
Autonomous site reliability engineering agent with isolated skill synthesis and blast-radius safety gates.
- **Isolated Subprocess Execution**: Synthesizes and tests remediation scripts in isolated subprocesses with scrubbed environment variables and strict timeouts.
- **Dual-Critic Reflexion Engine**: Safety Critic and SRE Reviewer validate proposed actions against immutable blast-radius constraints.

### ⚙️ [Enterprise AI Systems Engineering Suite](https://github.com/varadganjoo/enterprise-ai-systems)
A suite of 9 independent AI architectures demonstrating deterministic guardrails, state-machine orchestration, and evals-as-code:
- **01 Cited Knowledge Agent**: Verifiable grounding with character-level span offsets and temporal policy supersession.
- **02 Document Extraction**: Accounting reconciler verifying line-item math and routing low-confidence scans to human triage.
- **03 Operator Agent**: Stateful operator with tool allowlists, PII/credential guardrails, and supervisor approval queues.
- **04 Analytics Copilot**: Read-only SQL copilot enforcing AST validation via `sqlglot` (SELECT-only, table allowlist, row limits).
- **05 Model Router**: Multi-tiered semantic router triaging simple queries to lightweight models and complex reasoning to frontier models.
- **06 Memory Service**: Entity slot memory with deterministic supersession tracking and bidirectional PII redaction token vault.
- **07 Claim Auditor**: Atomic proposition fact-checking computing evidence-based verdicts against governing documents.
- **08 Case Workflow**: Event-sourced refund state machine with idempotent processing and hard financial category caps.
- **09 Multi-Hop Brief**: DAG-based multi-document reasoning that gates final conclusions if intermediate hops lack citations.

---

## Technical Stack

- **Core Languages**: Python, TypeScript, SQL
- **AI & Orchestration**: LangGraph, LangChain, Pydantic, Model Context Protocol (MCP), Gemini SDK, PyTorch
- **Backend & Data**: FastAPI, SQLite, PostgreSQL, `sqlglot`
- **Frontend & Visualization**: Modern HTML5/Tailwind CSS, React, Chart.js
- **Engineering Rigor**: Unit testing (`pytest`), evals-as-code, AST analysis, CI/CD with GitHub Actions

