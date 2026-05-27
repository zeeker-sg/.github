# Zeeker

Curated Singapore legal and regulatory datasets, designed for AI agents.

## What we do

Zeeker collects, structures, and serves primary-source Singapore legal data so that LLM-based legal research workflows are **citation-ready, scope-bounded, and safe to feed back into an agent loop**.

Our datasets include:

- **Court judgments** — Singapore High Court, Court of Appeal, and State Courts decisions
- **PDPC enforcement decisions** — Personal Data Protection Commission enforcement actions and voluntary undertakings
- **Government newsroom releases** — Regulatory announcements and policy updates from Singapore ministries and agencies
- **Legal commentaries** — Summaries and analysis from Singapore legal publications

## How to access the data

### MCP Server (for Claude and other MCP clients)

Connect to `https://mcp.zeeker.sg/mcp` using the Model Context Protocol. The server exposes read-only tools for search, table query, and document retrieval against `data.zeeker.sg`.

[→ MCP connector repository](https://github.com/zeeker-sg/mcp)

### Datasette (for humans and API clients)

Browse and query the data interactively at `https://data.zeeker.sg`. The Datasette interface supports full-text search, faceted filtering, and JSON API export.

[→ Datasette deployment repository](https://github.com/zeeker-sg/datasette)

### CLI (for developers)

Build, update, and deploy Zeeker databases locally with the `zeeker` CLI.

[→ CLI repository](https://github.com/zeeker-sg/cli)

## Repositories

| Repository | Purpose |
|---|---|
| [`mcp`](https://github.com/zeeker-sg/mcp) | MCP server connector — exposes datasets to Claude and other MCP clients |
| [`datasette`](https://github.com/zeeker-sg/datasette) | Branded Datasette deployment — the web UI and API at `data.zeeker.sg` |
| [`cli`](https://github.com/zeeker-sg/cli) | Core CLI for building and deploying Zeeker database projects |
| [`judgements`](https://github.com/zeeker-sg/judgements) | Court judgment data pipeline |
| [`pdpc`](https://github.com/zeeker-sg/pdpc) | PDPC enforcement decision data pipeline |
| [`sg-gov-newsrooms`](https://github.com/zeeker-sg/sg-gov-newsrooms) | Singapore government newsroom release data pipeline |
| [`sglawwatch`](https://github.com/zeeker-sg/sglawwatch) | Legal commentary data pipeline |

## License and attribution

Data is sourced from public Singapore government and judicial sources. Individual repositories document their respective data licenses and attribution requirements.

## Contributing

Issues and pull requests are welcome. We especially appreciate bug reports, data quality issues, and documentation improvements.

*Zeeker is an independent project. It is not affiliated with the Singapore government or any of the data sources it indexes.*
