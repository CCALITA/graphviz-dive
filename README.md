# Graphviz Deep Dive Skill

A skill for creating professional "ByteByteGo-style" system architecture diagrams using Graphviz DOT format with Excalidraw aesthetics.

## Installation

```bash
npx skills add CCALITA/graphviz-dive
```

## What This Skill Does

This skill provides a structured workflow for visualizing complex software systems through multiple architectural perspectives:

1. **System Architecture** - High-level modules, subsystems, and boundaries
2. **Type System & Relationships** - Class hierarchies, inheritance, and composition
3. **Data Flow Pipeline** - Request lifecycle and data movement
4. **Memory Model** - Low-level storage mechanics and physical layout
5. **Data Structure Internals** - Implementation details of core components
6. **State Machines** - Resource management and lifecycle transitions

## Style Requirements

All diagrams follow the "ByteByteGo" aesthetic:

- **Orthogonal edges** (`splines="ortho"`) for right-angle connections
- **Virgil font** for hand-drawn look
- **Rounded rectangle nodes** with thick borders
- **Clustered subgraphs** with dashed borders
- **xlabel** (not label) for edge annotations
- **Left-to-right flow** (`rankdir="LR"`)

## Usage

When asked to visualize a codebase or system:

1. The skill will explore the codebase structure
2. Generate 3-4 separate DOT files for different aspects
3. Use proper ByteByteGo styling

## Example Output Files

- `faiss_architecture.dot` - System overview
- `faiss_types.dot` - Class hierarchy
- `faiss_flow.dot` - Data flow
- `faiss_memory.dot` - Memory layout

## Rendering

Paste DOT code into:

- [Edotor.net](https://edotor.net)
- [GraphvizOnline](https://dreampuf.github.io/GraphvizOnline)

For Excalidraw style, convert to SVG and import.

## License

MIT
