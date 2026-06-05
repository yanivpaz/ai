# AI Glossary

A practical glossary for AI development, coding agents, prompting, and the everyday language that grows around using these systems.

## Table of Contents

- [Core AI Concepts](#core-ai-concepts)
- [Prompting and Context](#prompting-and-context)
- [Agents and Orchestration](#agents-and-orchestration)
- [Developer AI](#developer-ai)
- [Observability and Evaluation](#observability-and-evaluation)
- [Culture and Workflow Slang](#culture-and-workflow-slang)

## Core AI Concepts

### AI / Artificial Intelligence

Software systems that perform tasks associated with human intelligence, such as reasoning, language understanding, planning, perception, and code generation.

### Machine Learning

A field of AI where systems learn patterns from data instead of being programmed only with explicit rules.

### Deep Learning

Machine learning based on neural networks with many layers, commonly used in modern language, vision, and speech systems.

### Foundation Model

A large model trained on broad data that can be adapted to many downstream tasks.

### LLM / Large Language Model

A model trained to understand and generate text, code, and sometimes multimodal content by predicting likely token sequences.

### Token

A unit of text processed by a language model. Tokens may be words, word fragments, punctuation, or code fragments.

### Context Window

The maximum amount of input and output a model can consider in a single interaction, measured in tokens.

### AST

Abstract Syntax Tree. A structured representation of source code used by compilers, linters, code analyzers, and AI coding tools to understand or transform code more safely.

## Prompting and Context

### Prompt

The instruction, question, context, or task given to an AI model.

### System Prompt

High-priority instructions that define the model's role, behavior, constraints, and available tools.

### Prompt Engineering

The practice of designing prompts to produce more useful, reliable, or controllable model outputs.

### Silent Prompt Decay

The gradual loss of important instructions, constraints, or intent as a conversation grows longer, often without the user noticing until output quality drifts.

### Token Maxxing

Aggressively filling the context window with as much background, examples, files, or instructions as possible. It can improve grounding, but can also create noise and bloated context.

### Bloated Context

A context window overloaded with irrelevant, stale, duplicated, or low-value information, making the model slower, more expensive, and sometimes less accurate.

### Prompt Injection

An attack or failure mode where untrusted text tries to override instructions, leak data, or manipulate an AI system's behavior.

## Agents and Orchestration

### AI Agent

An AI system that can plan, use tools, observe results, and continue working across multiple steps toward a goal.

### Agentic Harness

The surrounding system that lets an AI model act like an agent: tools, permissions, memory, planning loops, execution environment, logging, and safety checks.

### Deterministic Orchestration

Designing AI workflows so routing, tool use, state transitions, and outputs are controlled by explicit logic rather than relying entirely on model improvisation.

### Tool Calling

The ability for a model to request structured calls to external tools, APIs, scripts, databases, or applications.

### Function Calling

A structured form of tool calling where the model emits function names and arguments that a host application can execute.

### MCP / Model Context Protocol

A protocol for connecting AI applications to external tools, data sources, prompts, and context providers through a standard interface.

### ACP / Agent Client Protocol

An open protocol pattern for communication between coding agents and clients such as editors or IDEs. The acronym ACP is overloaded in AI, so check the specific project or vendor context.

## Developer AI

### Copilot

An AI coding assistant, commonly referring to GitHub Copilot, that helps write, explain, review, and modify code.

### Claude

Anthropic's family of AI assistants and models, often used for coding, writing, reasoning, and long-context analysis.

### ChatGPT

OpenAI's conversational AI product, used for writing, coding, analysis, brainstorming, and tool-assisted workflows.

### Code Assistant

An AI tool that helps developers write, edit, explain, debug, test, or review software.

### Pair Programming with AI

Working with an AI assistant as a coding collaborator: asking for suggestions, reviews, implementation help, and explanations while the human keeps direction and judgment.

### Code Review with AI

Using AI to inspect code for bugs, regressions, maintainability risks, missing tests, and unclear behavior.

### LLM Wiki

A knowledge base maintained for or by LLM-powered workflows, often used to store project context, decisions, reusable prompts, terminology, or operational notes.

## Observability and Evaluation

### Evals / AI Evaluation

Tests and measurements used to judge whether an AI system behaves correctly, reliably, safely, and usefully.

### Benchmark

A standardized task or dataset used to compare models, prompts, tools, or systems.

### OTEL Observability

Using OpenTelemetry traces, metrics, and logs to understand AI systems, including agent steps, tool calls, latency, token usage, failures, and cost.

### Latency

The time it takes for an AI system to respond or complete a workflow.

### Cost per Token

The price associated with model input and output usage, usually calculated by token volume.

### Guardrails

Rules, checks, filters, or system designs that reduce unsafe, incorrect, or unwanted model behavior.

## Culture and Workflow Slang

### YOLO Mode

Running an AI agent with broad permissions and minimal human confirmation, usually allowing it to edit files, run commands, or make decisions autonomously. Useful for speed, risky when the task is ambiguous or destructive.

### Ralph Loops

Repeated cycles where an AI agent keeps trying variations of the same flawed approach instead of stepping back, re-planning, or asking for clarification.

### AI Slop

Low-quality AI-generated content that looks plausible but is generic, shallow, inaccurate, or unedited.

### AI FOMO

The anxiety that one is falling behind because new AI tools, models, workflows, and capabilities are appearing faster than they can be evaluated or adopted.

### Vibe Coding

An informal style of AI-assisted programming where the developer steers by intent, feedback, and iteration rather than manually writing every detail.
