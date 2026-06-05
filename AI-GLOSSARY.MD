# AI Glossary

A focused glossary for AI development, coding agents, prompting, and the everyday language that grows around using these systems.

## Table of Contents

- [Prompting and Context](#prompting-and-context)
  - [Silent Prompt Decay](#silent-prompt-decay)
  - [Token Maxxing](#token-maxxing)
  - [Bloated Context](#bloated-context)
- [Agents and Orchestration](#agents-and-orchestration)
  - [Agentic Harness](#agentic-harness)
  - [Deterministic Orchestration](#deterministic-orchestration)
  - [ACP Protocol](#acp-protocol)
- [Developer AI](#developer-ai)
  - [LLM Wiki](#llm-wiki)
  - [LSP / Language Server Protocol](#lsp--language-server-protocol)
  - [Knowledge Graph](#knowledge-graph)
  - [Spec Driven Development](#spec-driven-development)
- [Skill Review](#skill-review)
  - [GSD / Get Shit Done](#gsd--get-shit-done)
  - [Superpowers](#superpowers)
  - [Waza](#waza)
  - [vscode-chat-customizations-evaluation](#vscode-chat-customizations-evaluation)
- [Evaluation](#evaluation)
  - [Terminal Bench](#terminal-bench)
  - [SWE-bench](#swe-bench)
  - [DeepSWE](#deepswe)
  - [OTEL Observability](#otel-observability)
- [Culture and Workflow Slang](#culture-and-workflow-slang)
  - [YOLO Mode](#yolo-mode)
  - [Ralph Loops](#ralph-loops)
  - [AI Slop](#ai-slop)
  - [AI FOMO](#ai-fomo)

## Prompting and Context

### Silent Prompt Decay

The gradual loss of important instructions, constraints, or intent as a conversation grows longer, often without the user noticing until output quality drifts.

In practice, this happens when earlier guidance gets pushed out of the effective working context by newer messages, tool outputs, long files, or repeated retries. 

Reference:
- [YouTube clip](https://youtu.be/WnBx1Vi7M6w?t=835)

### Token Maxxing

The idea of maximizing token consumption as a signal of how deeply someone is embracing AI tools. The term borrows from internet slang where "-maxxing" means pushing something to its absolute limit.

It took hold in early 2026, when stories circulated about large companies such as Meta and Amazon ranking employees by token usage on internal leaderboards.

### Bloated Context

A context window overloaded with irrelevant, stale, duplicated, or low-value information, making the model slower, more expensive, and sometimes less accurate.

## Agents and Orchestration

### Agentic Harness

The surrounding system that lets an AI model act like an agent: tools, permissions, memory, planning loops, execution environment, logging, and safety checks.

### Deterministic Orchestration

Designing AI workflows so routing, tool use, state transitions, and outputs are controlled by explicit logic rather than relying entirely on model improvisation.

### ACP Protocol

An open protocol pattern for communication between coding agents and clients such as editors or IDEs. The acronym ACP is overloaded in AI, so check the specific project or vendor context.

## Developer AI

### LLM Wiki

A knowledge base maintained for or by LLM-powered workflows, often used to store project context, decisions, reusable prompts, terminology, or operational notes.

### LSP / Language Server Protocol

A standard protocol that lets editors, IDEs, and coding agents communicate with language-specific tools for features such as autocomplete, go-to-definition, rename, diagnostics, formatting, and code navigation. See [LSP.MD](./LSP.MD) for a longer explanation.

Example:
- [Serena](https://github.com/oraios/serena), which uses language-server-backed semantic tools to give coding agents more IDE-like retrieval and editing capabilities.

### Knowledge Graph

A structured graph representation of a codebase or project where files, symbols, APIs, schemas, docs, and relationships can be queried more directly than raw text alone.

Examples:
- [Graphify](https://github.com/safishamsi/graphify), which turns a codebase into a queryable knowledge graph that can help an agent work from a structured map instead of raw file sprawl.
- [GitNexus](https://github.com/nxpatterns/gitnexus), which builds a repository knowledge graph and Graph RAG workflow to support structured exploration before implementation.

### Spec Driven Development

Writing a clear specification before implementation, then using that spec to guide AI-assisted coding, tests, reviews, and acceptance criteria.

Example:
- [GitHub Spec Kit](https://github.com/github/spec-kit), a toolkit for Spec-Driven Development that structures work as spec -> plan -> tasks -> implement and integrates with multiple AI coding agents.

## Skill Review

### GSD / Get Shit Done

A spec-driven workflow system for coding agents that emphasizes milestones, structured handoffs, and keeping work moving through explicit project phases instead of loose chat history.

Repo: [gsd-build/get-shit-done](https://github.com/gsd-build/get-shit-done)

### Superpowers

An agentic skills framework and software development methodology that gives coding agents staged habits such as planning, research, verification, and review so they produce more engineering-grade work.

Repo: [obra/superpowers](https://github.com/obra/superpowers)

### Waza

Microsoft's CLI and evaluation framework for agent skills, used to create, test, benchmark, and improve skill quality across workflows and models.

Repo: [microsoft/waza](https://github.com/microsoft/waza)

### vscode-chat-customizations-evaluation

An extension for analyzing and improving AI prompt files. Works with .prompt.md, .agent.md, SKILL.md, and .instructions.md files — providing LLM-powered semantic analysis directly in VS Code.  

Repo: [microsoft/vscode-chat-customizations-evaluation](https://github.com/microsoft/vscode-chat-customizations-evaluation)


## Evaluation

### Terminal Bench

A benchmark for evaluating AI agents on realistic terminal-based tasks, where the model has to work through shell commands and environment constraints instead of only generating code in the abstract.

Repo: [laude-institute/terminal-bench](https://github.com/laude-institute/terminal-bench)

### SWE-bench

A benchmark that measures whether language models and coding agents can resolve real GitHub software issues by producing fixes that pass repository-specific tests.

Repo: [SWE-bench/SWE-bench](https://github.com/SWE-bench/SWE-bench)

### DeepSWE

A benchmark for frontier coding agents focused on original, long-horizon software engineering tasks across active open-source repositories, designed to reduce contamination from previously published fixes.

Repo: [datacurve-ai/deep-swe](https://github.com/datacurve-ai/deep-swe)

### OTEL Observability

Using OpenTelemetry traces, metrics, and logs to understand AI systems, including agent steps, tool calls, latency, token usage, failures, and cost.

## Culture and Workflow Slang

### YOLO Mode

Running an AI agent with broad permissions and minimal human confirmation, usually allowing it to edit files, run commands, or make decisions autonomously. Useful for speed, risky when the task is ambiguous or destructive.

### Ralph Loops

Repeated cycles where an AI agent keeps trying variations of the same flawed approach instead of stepping back, re-planning, or asking for clarification.

### AI Slop

Low-quality AI-generated content that looks plausible but is generic, shallow, inaccurate, or unedited.

### AI FOMO

The anxiety that one is falling behind because new AI tools, models, workflows, and capabilities are appearing faster than they can be evaluated or adopted.
