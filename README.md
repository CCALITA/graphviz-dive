# Graphviz Deep Dive Skill

A skill for creating professional "ByteByteGo-style" system architecture diagrams using Graphviz DOT format with Excalidraw aesthetics.

## Version

2.0.0 - Exhaustive analysis with 8+ aspects

## What This Skill Does

This skill produces **exhaustive, expert-grade visualizations** of any codebase. It generates complete analysis across all architectural aspects without requiring user interaction or selection.

**Target:** A new-grad should produce diagrams as if they'd written the system from scratch.

## Core Principle

**Generate ALL aspects by default.** No selection, no minimal. Every diagram an expert would need to fully understand the system.

## Installation

```bash
npx skills add CCALITA/graphviz-dive
```

## Aspects Generated (8+)

| Aspect | File Suffix | Focus |
|--------|-------------|-------|
| Context | `_context` | External users, systems, boundaries |
| Components | `_components` | Modules, services, boundaries |
| Types | `_types` | Classes, interfaces, domain model |
| Flow | `_flow` | Request pipeline, data journey |
| Concurrency | `_concurrency` | Threads, async, events |
| Storage | `_storage` | Databases, caches, schemas |
| Security | `_security` | Auth, trust boundaries |
| Deployment | `_deployment` | Infrastructure, containers |

Plus optional: `_memory`, `_state`

## Style Requirements

All diagrams follow the "ByteByteGo" aesthetic:

- **Orthogonal edges** (`splines="ortho"`) for right-angle connections
- **Virgil font** for hand-drawn look
- **Rounded rectangle nodes** with thick borders
- **Clustered subgraphs** with dashed borders
- **xlabel** (not label) for edge annotations
- **Left-to-right flow** (`rankdir="LR"`)

## Usage

When asked to visualize a codebase:

1. The skill explores the codebase structure
2. Generates all 8+ DOT files for different aspects
3. Uses proper ByteByteGo styling
4. Includes expert annotations

## Examples

### Monolith
- `examples/monolith/` - Full 8-aspect for monolithic architecture

### Microservices
- `examples/microservice/` - Full 8-aspect for microservices

### Event-Driven
- `examples/event_driven/` - Full 8-aspect for event-driven architecture

### DDD
- `examples/ddd/` - Full 8-aspect for Domain-Driven Design

### Faiss (Original)
- `examples/faiss_types.dot` - Type hierarchy example

## Templates

Reusable templates available in `template/`:
- `template.dot` - Full standard template
- `template_context.dot` - Context diagram template
- `template_components.dot` - Components template
- `template_types.dot` - Types template
- `template_flow.dot` - Flow template
- `template_concurrency.dot` - Concurrency template
- `template_storage.dot` - Storage template
- `template_security.dot` - Security template
- `template_deployment.dot` - Deployment template
- `template_memory.dot` - Memory template
- `template_state.dot` - State machine template

## Rendering

Paste DOT code into:

- [Edotor.net](https://edotor.net)
- [GraphvizOnline](https://dreampuf.github.io/GraphvizOnline)

For Excalidraw style, convert to SVG and import.

## License

MIT
