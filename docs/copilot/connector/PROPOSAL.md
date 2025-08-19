# Independent Publisher Proposal (Summary)

Service: Olexi MCP Connector for AustLII

Problem & audience
- Problem: Efficient discovery of Australian primary law across AustLII without manual browsing.
- Audience: Legal researchers, practitioners, and students using Microsoft Copilot Studio.

Data source
- AustLII (austlii.edu.au) legacy CGI search. Primary law content is public domain; connector returns links and minimal metadata.

Auth
- None (for MCP endpoint) to simplify review.

Endpoints
- MCP Streamable HTTP at the service root: `https://olexi-mcp-root-au-691931843514.australia-southeast1.run.app/`
- Health endpoints are provided in the local combined app; production Cloud Run is MCP-only at the root.

Operations (tools)
- list_databases
- search_austlii
- build_search_url
- search_with_progress

Limitations
- Dependent on AustLII uptime. No full-text replication; links only.

Publisher
- Name: <Your Publisher Name>
- Website: https://<your-website>
- Support: ai@olexi.legal

Notes
- Attribution: "Results via AustLII (austlii.edu.au)".
