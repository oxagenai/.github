<div align="center">

<img src="https://oxagen.ai/logos/oxagen-logo-adaptive.svg" alt="Oxagen" width="200" />

# Context Infrastructure for AI Agents

**Persistent memory. Queryable knowledge. One API.**

[![Website](https://img.shields.io/badge/oxagen.ai-7182FF?style=for-the-badge&labelColor=0F172A)](https://oxagen.ai)
[![Docs](https://img.shields.io/badge/Docs-3CFF52?style=for-the-badge&labelColor=0F172A&logoColor=black)](https://docs.oxagen.ai)
[![X](https://img.shields.io/badge/Follow-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/oxagenai)
[![License](https://img.shields.io/badge/License-Apache_2.0-7182FF?style=for-the-badge&labelColor=0F172A)](LICENSE)

</div>

---

## What Oxagen builds

Oxagen is the first ontology-as-a-service platform: a managed knowledge graph that gives AI agents durable memory and structured reasoning context. Connect once over MCP and your agent gains a mind that persists across sessions, tools, and runs.

We are creating the **Context Infrastructure** category. Stop stuffing prompts — start querying a mind.

## The problem

Agents forget. Vector stores match keywords without understanding them. Context windows blow up, decay, and lose the thread. Every workflow restarts from zero.

The missing layer is not a better model. It is persistent, structured knowledge that agents can actually reason over.

## What Oxagen ships

- **Ontology engine.** Entities, relationships, provenance, and semantics, modeled as a queryable graph on Postgres.
- **MCP server.** Drop-in connection for any agent runtime: Claude, Cursor, Copilot, custom stacks.
- **Multi-tenant API.** Tenants, workspaces, and projects with RBAC, supporting single-user and team configurations.
- **Hybrid retrieval.** Qdrant for semantic recall, PuppyGraph for graph traversal, joined under one query plane.
- **Schema authoring.** Design ontologies in code or in the studio, then version them like data.

## Stack

Running in production on Next.js 15, FastAPI, PostgreSQL (Citus on Crunchy Bridge), Qdrant, PuppyGraph, Anthropic, and Vercel.

## Quick start

```bash
pip install oxagen
```

```python
from oxagen import Workspace

ws = Workspace.connect(api_key="ox_...")

ws.remember("Acme signed a 3-year contract worth $1.2M starting Q3 2026")
ws.query("What is Acme's current commitment?")
```

```bash
# Or wire it straight into an MCP-compatible agent
npx @oxagen/mcp --workspace acme-prod
```

## Repositories

| Repo | What it does |
|------|--------------|
| [`oxagen`](https://github.com/oxagenai/oxagen) | Core platform monorepo: API, web app, ontology engine |
| [`oxagen-py`](https://github.com/oxagenai/oxagen-py) | Python SDK |
| [`oxagen-ts`](https://github.com/oxagenai/oxagen-ts) | TypeScript SDK |
| [`oxagen-mcp`](https://github.com/oxagenai/oxagen-mcp) | MCP server reference implementation |
| [`docs`](https://github.com/oxagenai/docs) | Public documentation |
| [`examples`](https://github.com/oxagenai/examples) | Reference agents and integration recipes |

## Hiring

Oxagen is hiring its Founding Member of Technical Staff. AI-workflow-first, cross-functional, shipping fast. Mail [mac@oxagen.ai](mailto:mac@oxagen.ai) with whatever best represents your work.

## Connect

- Web: [oxagen.ai](https://oxagen.ai)
- Docs: [docs.oxagen.ai](https://docs.oxagen.ai)
- Contact: [hello@oxagen.ai](mailto:hello@oxagen.ai)
- Founder: [Mac Anderson](https://linkedin.com/in/macanderson)

<div align="center">

<sub>Built by operators. Backed by Meta Ventures.</sub>

</div>
