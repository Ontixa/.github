# Ontixa

Ontixa is an open-source organization building tools for agentic software
work — a systems programming language, an AI-native project engine, and
execution-safety and control surfaces for terminal coding agents.

## Projects

| Project | Description |
| --- | --- |
| [ontixa](https://github.com/Ontixa/ontixa) | Experimental semantic-first systems programming language and compiler pipeline for human and autonomous machine programmers — multi-module workspaces, inferred ownership contracts, semantic rename and patch transactions, `ontixa fmt`, strings, arrays, and `for` loops; programs run in a reference interpreter (no native codegen yet). |
| [worldos](https://github.com/Ontixa/worldos) | AI-native project engine: a governed, schema-versioned universal project graph behind a portable `.worldos` file, driven by CLI, JSON-RPC, MCP, SDK, and desktop surfaces — with an opt-in CAD workflow (`geometry.measure`, `geometry.import`, `geometry.export`, artifact export), a bounded observe–act–verify agent loop, and a hosted plugin runtime. |
| [agent-loop-runtime](https://github.com/Ontixa/agent-loop-runtime) | Headless runtime that runs coding agents (Codex, Claude Code, Devin, Gemini CLI, Qwen Code, OpenCode, Aider, custom CLIs) as bounded, resumable missions with worktree isolation, scope-expansion approvals, fair scheduling with resource-aware admission, chaos-tested recovery, live mission-event streaming, and a loopback daemon control API plus MCP server. |
| [ai-cli-editor](https://github.com/Ontixa/ai-cli-editor) | Desktop control plane for terminal coding agents — agent sessions cockpit, live token and cost telemetry, worktree isolation with merge-readiness probes, checkpoints, session export receipts, deterministic review classification, and diff review. Built with Tauri 2, React, and Rust. |
| [veyra](https://github.com/Ontixa/veyra) | Local, embeddable execution kernel (v0.1.0 released) that turns agent side effects into versioned transactions with least-authority capabilities, exact approvals, verified rollback, and a versioned journal-migration contract. |

## Where to start

- Interested in the language and its machine-readable semantics? Start with
  [ontixa](https://github.com/Ontixa/ontixa).
- Want to run coding agents under explicit policy and recovery? See
  [agent-loop-runtime](https://github.com/Ontixa/agent-loop-runtime).
  For a desktop workspace around terminal coding sessions, explore
  [ai-cli-editor](https://github.com/Ontixa/ai-cli-editor).
- Care about authorization, provenance, and rollback for agent side effects?
  Read [veyra](https://github.com/Ontixa/veyra).
- For the broader governed project model behind one portable file, explore
  [worldos](https://github.com/Ontixa/worldos).

## First run: agent-loop-runtime

Requires Git and Node.js (24.14.1 verified locally; Node 20, 22 and 24 tested in CI).

```bash
git clone https://github.com/Ontixa/agent-loop-runtime.git
cd agent-loop-runtime
npm ci
npm run build
node scripts/demo-mission.mjs
```

This runs a real bounded mission with a deterministic local Node fixture agent,
not an AI model. No AI account is needed. It creates a temporary repository and
isolated worktree, checks exact output with an independent validation command,
and prints the retained receipt and evidence paths. It does not use your project
as the mission repository or publish changes.

Run `node scripts/demo-mission.mjs --fail-validation` to see incorrect output
rejected even when the agent process succeeds; this deliberately exits 1.
See the [demo and its limits](https://github.com/Ontixa/agent-loop-runtime#try-a-mission-without-an-ai-account)
for cleanup and verification details. Running a model-backed mission additionally
requires a configured, authenticated, supported agent CLI, its sandbox/workspace
trust setup, and real validation commands for the intended task.

## Contributing

Each repository keeps its own contributing guide:
[ontixa](https://github.com/Ontixa/ontixa/blob/main/CONTRIBUTING.md) ·
[worldos](https://github.com/Ontixa/worldos/blob/main/CONTRIBUTING.md) ·
[agent-loop-runtime](https://github.com/Ontixa/agent-loop-runtime/blob/main/CONTRIBUTING.md) ·
[ai-cli-editor](https://github.com/Ontixa/ai-cli-editor/blob/main/CONTRIBUTING.md) ·
[veyra](https://github.com/Ontixa/veyra/blob/main/CONTRIBUTING.md)

Looking for somewhere to help? Browse
[open issues across the Ontixa org](https://github.com/search?q=org%3AOntixa+is%3Aissue+is%3Aopen&type=issues).

## Maintainer

Founded and maintained by [Tang Vu (@tang-vu)](https://github.com/tang-vu).
