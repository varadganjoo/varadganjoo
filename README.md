# Varad Ganjoo

**AI Systems & Software Engineer**

I build developer tools and stateful AI applications, with a focus on agent memory, tool execution, and human approval.

[LinkedIn](https://www.linkedin.com/in/varad-ganjoo-3137631b2/) | [Email](mailto:varadganjoo@gmail.com)

## Featured Projects

### [MemKernel](https://github.com/varadganjoo/MemKernel)

Shared local memory for coding agents. Persistent decisions, investigation branches, memory rollback, and token-budgeted snapshots built on an append-only SQLite event log.

Local agents coordinate through leases and notices. Separate machines can exchange signed notices through a synced folder; direct memory sync is still in development.

[Python package](https://pypi.org/project/memkernel-mcp/) | [Design and benchmarks](https://github.com/varadganjoo/MemKernel/blob/main/docs/whitepaper.md)

### [AutoTool](https://github.com/varadganjoo/Autotool)

An MCP tool layer that lets agents create and reuse Python tools as they work. It verifies tools in separate processes, loads them without restarting the server, and keeps them available across agent clients.

Credential access uses per-tool declarations and consent, with host allowlists and output redaction.

[Python package](https://pypi.org/project/autotool-mcp/) | [Design and evaluation](https://github.com/varadganjoo/Autotool/blob/main/paper/autotool.md)

### [WebAgent Protocol](https://github.com/varadganjoo/WebAgent-Protocol)

A Python SDK and proposed MCP extension for discovering tools published by websites. Signed manifests and responses let clients verify what a site returned.

Includes a FastAPI server, MCP bridge, confirmation hooks for side effects, rate limits, replay protection, and bounded multi-turn interactions.

[Python package](https://pypi.org/project/webagent-protocol/) | [MCP extension proposal](https://github.com/varadganjoo/WebAgent-Protocol/blob/main/docs/mcp_extension.md)

## Applied AI Systems

| Project | Engineering focus |
| --- | --- |
| [CareFlow Clinical Agent](https://github.com/varadganjoo/careflow-clinical-agent) ([demo](https://careflow-clinical-agent.vercel.app)) | Clinical documentation demo with de-identification, code-level safety checks, and physician sign-off. Uses fictional patients; not clinically validated. |
| [Apex-Alpha](https://github.com/varadganjoo/apex-alpha) ([demo](https://apex-alpha-tan.vercel.app)) | Research terminal combining market data, Monte Carlo simulations, filing-grounded agent debate, and human review of staged orders. |
| [Aegis SRE](https://github.com/varadganjoo/aegis-sre) | Incident-response simulation with validated actions, blast-radius checks, and operator feedback recorded as reusable rules. |
| [Enterprise AI Systems](https://github.com/varadganjoo/enterprise-ai-systems) | Nine runnable reference applications covering cited retrieval, document extraction, read-only SQL, event-sourced workflows, and evaluation. |

<details>
<summary>See the CareFlow documentation workflow</summary>

![CareFlow demo showing an editable SOAP note for a fictional patient](https://raw.githubusercontent.com/varadganjoo/careflow-clinical-agent/main/docs/images/03_scribe.png)

</details>

I also maintain [Baby LLM](https://github.com/varadganjoo/baby-llm), a learning experiment combining incremental n-gram memory, adaptive embeddings, and a PyTorch GRU with attention.

## Technical Stack

**Languages:** Python, TypeScript, SQL  
**Agent systems:** MCP, LangGraph, LangChain, Pydantic, PyTorch  
**Backend and data:** FastAPI, SQLite, PostgreSQL, Redis  
**Interfaces:** React, Tailwind CSS, Chart.js  
**Delivery:** pytest, reproducible evaluations, package releases, GitHub Actions

My approach is to keep state explicit, validate model proposals in code, and test the failure paths as well as the successful ones.
