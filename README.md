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

### 🏥 [CareFlow Clinical Agent](https://github.com/varadganjoo/careflow-clinical-agent) · [Live demo](https://careflow-clinical-agent.vercel.app)
Clinical decision support and SOAP-note scribe built on a LangGraph state machine with a physician sign-off gate.
- **Deterministic Safety Checks**: Code-level rules run before the model is called and flag contraindicated combinations (e.g., dual RAS blockade, metformin with low eGFR) and critical labs (hyperkalemia).
- **De-identified Ambient Scribe**: The encounter transcript and patient record pass through a PHI token vault (names, MRNs, contact details) before Gemini, with Groq as a backup, drafts a structured SOAP note with ICD-10 and CPT codes.
- **Human-in-the-Loop Sign-off**: LangGraph `interrupt()` holds every draft until a physician approves, edits, or rejects it; only signed notes reach the writeback step.

### 📈 [Apex-Alpha](https://github.com/varadganjoo/apex-alpha) · [Live demo](https://apex-alpha-tan.vercel.app)
Quant research terminal on live market data: Monte Carlo forecasts, an adversarial LLM investment committee, and a portfolio manager sign-off gate.
- **Live Data**: Prices from Yahoo Finance, fundamentals and filing excerpts from SEC EDGAR, and the risk-free rate from the U.S. Treasury, each cached with a labeled fallback.
- **Grounded Multi-Agent Debate**: Bull and Bear agents argue from the latest 10-Q or 10-K, and every citation is checked word for word against the filing.
- **Backtested Quant Engine**: Jump-diffusion Monte Carlo with fractional-Kelly sizing and VaR limits, scored walk-forward on 15 years of real prices (held-out rank IC +0.07).
- **Portfolio Manager Gate**: LangGraph `interrupt()` pauses every staged order for approval, with overrides capped at the 15% position limit.

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
- **AI & Orchestration**: LangGraph, LangChain, Pydantic, Model Context Protocol (MCP), Gemini SDK, Groq, PyTorch
- **Backend & Data**: FastAPI, SQLite, PostgreSQL, `sqlglot`, SEC EDGAR XBRL, yfinance
- **Frontend & Visualization**: Modern HTML5/Tailwind CSS, React, Chart.js
- **Engineering Rigor**: Unit testing (`pytest`), evals-as-code, AST analysis, CI/CD with GitHub Actions

