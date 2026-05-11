# Obsidian Vault Manager - Claude Code Plugin

A Claude Code plugin that provides two powerful skills for knowledge management and technical documentation:

1. **Obsidian Manager (Obi)** - An intelligent Obsidian vault manager for organizing, creating, and optimizing notes with PKM best practices
2. **Mermaid Diagrams** - A comprehensive guide for creating professional software diagrams using Mermaid syntax

## Installation

```bash
# Step 1: Add the marketplace
claude plugin marketplace add git@github.com:GeniusGogoing/obsidian-vault-manager-claude-plugin.git

# Step 2: Install the plugin
claude plugin install obsidian-vault-manager@obsidian-vault-manager-claude-plugin
```

## Skills

### Obsidian Manager

An intelligent note manager called "Obi" that helps you:

- **Organize Inbox** - Categorize and file notes from your inbox
- **Create Notes** - Generate well-structured notes using templates
- **Explain & Record** - Learn concepts and save them as knowledge notes
- **Manage Tags & Links** - Maintain note relationships and metadata
- **MOC Management** - Build and maintain Maps of Content

Supports multiple backends: Obsidian MCP (preferred), Obsidian CLI, and local file tools.

#### Vault Structure

```
00-Inbox/      - Temporary unsorted notes
01-MOC/        - Map of Content notes (knowledge network hubs)
02-Concepts/   - Concept-related notes
03-Problems/   - Problem-solving notes
04-Notes/      - Personal notes
05-Work/       - Work-related notes
```

### Mermaid Diagrams

A comprehensive diagramming guide supporting 9 diagram types:

1. **Class Diagrams** - Domain modeling, OOP design
2. **Sequence Diagrams** - API flows, temporal interactions
3. **Flowcharts** - Processes, algorithms, decision trees
4. **ERD** - Database schemas, table relationships
5. **C4 Architecture** - System context, containers, components
6. **State Diagrams** - State machines, lifecycle states
7. **Git Graphs** - Branching strategies
8. **Gantt Charts** - Project timelines
9. **Pie/Bar Charts** - Data visualization

Includes detailed reference guides for each diagram type with syntax, examples, and best practices.

## Requirements

- Claude Code CLI
- Node.js (for Obsidian MCP server via npx)

## MCP Server

This plugin bundles the [mcpvault](https://www.npmjs.com/package/@bitbonsai/mcpvault) Obsidian MCP server, which provides direct vault access (read, write, search, tags, frontmatter, etc.) through the Model Context Protocol. The MCP server is automatically configured when the plugin is installed.

## License

[MIT](LICENSE)

## Author

[GeniusGogoing](https://github.com/GeniusGogoing)
