# Ontixa

Ontixa is an open-source organization building tools for agentic software
work — a systems programming language, an AI-native project engine, and
execution-safety and control surfaces for terminal coding agents.

## Projects

| Project | Description |
| --- | --- |
| [ontixa](https://github.com/Ontixa/ontixa) | Semantic-first systems programming language and compiler pipeline, designed for human and autonomous machine programmers. |
| [worldos](https://github.com/Ontixa/worldos) | AI-native project engine: a governed, schema-versioned universal project graph behind a portable `.worldos` file, driven by CLI, JSON-RPC, MCP, SDK, and desktop surfaces. |
| [agent-loop-runtime](https://github.com/Ontixa/agent-loop-runtime) | Headless runtime that runs coding agents (Codex, Claude Code, Devin, Qwen Code, OpenCode, Aider, custom CLIs) as bounded, resumable missions with worktree isolation and human approval gates. |
| [ai-cli-editor](https://github.com/Ontixa/ai-cli-editor) | Desktop control plane for terminal coding agents — project tabs, live session telemetry, worktree isolation, and diff review. Built with Tauri 2, React, and Rust. |
| [veyra](https://github.com/Ontixa/veyra) | Local, embeddable execution kernel that turns agent side effects into versioned transactions with least-authority capabilities, exact approvals, and verified rollback. |

## Where to start

- Interested in the language and its machine-readable semantics? Start with
  [ontixa](https://github.com/Ontixa/ontixa).
- Want to run coding agents under explicit policy and recovery? See
  [agent-loop-runtime](https://github.com/Ontixa/agent-loop-runtime), then pair it with
  [ai-cli-editor](https://github.com/Ontixa/ai-cli-editor), the desktop cockpit that
  consumes its mission status and events.
- Care about authorization, provenance, and rollback for agent side effects?
  Read [veyra](https://github.com/Ontixa/veyra).
- For the broader governed project model behind one portable file, explore
  [worldos](https://github.com/Ontixa/worldos).

## Contributing

Each repository keeps its own contributing guide:
[ontixa](https://github.com/Ontixa/ontixa/blob/main/CONTRIBUTING.md) ·
[worldos](https://github.com/Ontixa/worldos/blob/main/CONTRIBUTING.md) ·
[agent-loop-runtime](https://github.com/Ontixa/agent-loop-runtime/blob/main/CONTRIBUTING.md) ·
[ai-cli-editor](https://github.com/Ontixa/ai-cli-editor/blob/main/CONTRIBUTING.md) ·
[veyra](https://github.com/Ontixa/veyra/blob/main/CONTRIBUTING.md)

## Maintainer

Founded and maintained by [Tang Vu (@tang-vu)](https://github.com/tang-vu).
