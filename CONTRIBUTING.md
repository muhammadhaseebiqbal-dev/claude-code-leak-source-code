# Contributing

Thanks for your interest in contributing to this repository!

## What This Is

This repo archives a source snapshot of Anthropic's Claude Code CLI together with documentation and exploration tooling. Contributions here are about **documentation, tooling, and exploration aids** rather than editing the archived snapshot itself.

## What You Can Contribute

- **Documentation** — Improve or expand the [docs/](docs/) directory
- **MCP Server** — Enhance the exploration MCP server in [mcp-server/](mcp-server/)
- **Analysis** — Write-ups, architecture diagrams, or annotated walkthroughs
- **Tooling** — Scripts or tools that aid in studying the source code
- **Bug fixes** — Fix issues in the MCP server or supporting infrastructure

## What Not to Change

- **`src/` directory** — This is the archived source snapshot and should generally remain unchanged.
- The [`backup` branch](https://github.com/muhammadhaseebiqbal-dev/claude-code-leak-source-code/tree/backup) contains the raw imported snapshot.

## Getting Started

### Prerequisites

- **Node.js** 18+ (for the MCP server)
- **Git**

### Setup

```bash
git clone https://github.com/muhammadhaseebiqbal-dev/claude-code-leak-source-code.git
cd claude-code-source-code
```

### MCP Server Development

```bash
cd mcp-server
npm install
npm run dev    # Run with tsx (no build step)
npm run build  # Compile to dist/
```

### Linting & Type Checking

```bash
# From the repo root — checks the archived snapshot
npm run lint        # Biome lint
npm run typecheck   # TypeScript type check
```

## Code Style

For any new code (MCP server, tooling, scripts):

- TypeScript with strict mode
- ES modules
- 2-space indentation (tabs for `src/` to match Biome config)
- Descriptive variable names, minimal comments

## Submitting Changes

1. Fork the repository
2. Create a feature branch (`git checkout -b my-feature`)
3. Make your changes
4. Commit with a clear message
5. Push and open a pull request

Please keep pull requests scoped to docs, MCP tooling, scripts, or repository metadata unless a maintainer explicitly asks for changes to the archived snapshot.

## Questions?

Open an issue or reach out to [nichxbt](https://www.x.com/nichxbt).
