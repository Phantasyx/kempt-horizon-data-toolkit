# Kempt Horizon Data Toolkit

A hosted, read-only MCP server with 17 tools for AI agents: web pages to clean Markdown, email, phone and CSV cleaning, and live US government data from SEC EDGAR, the Federal Register, USAspending and Grants.gov.

This repository holds the listing metadata only. The server is hosted, so there's nothing to install.

## Connect

Endpoint (Streamable HTTP, OAuth): `https://kempt-horizon-data-toolkit.mcpize.run/mcp`

Subscribe on [MCPize](https://mcpize.com/mcp/kempt-horizon-data-toolkit) (the Free plan includes 50 tool calls a month), then add the server to your client:

```json
{
  "mcpServers": {
    "kempt-horizon-data": { "url": "https://kempt-horizon-data-toolkit.mcpize.run/mcp" }
  }
}
```

Claude Code: `claude mcp add --transport http kempt-horizon-data https://kempt-horizon-data-toolkit.mcpize.run/mcp`

## Tools

| Group | Tools |
|---|---|
| Read the web | `page_to_markdown`, `page_metadata`, `page_extract` |
| Clean data | `validate_email`, `validate_emails`, `parse_phone`, `clean_csv`, `clean_text` |
| SEC EDGAR | `sec_company_search`, `sec_company_profile`, `sec_company_filings`, `sec_company_financials`, `sec_filing_search` |
| US federal data | `federal_register_search`, `usaspending_awards`, `grants_search`, `grant_details` |

All tools are read-only.

## Docs and REST APIs

- Docs: https://phantasyx.com/apis/docs
- REST APIs on RapidAPI: [Data Cleaner & Validator](https://rapidapi.com/Kemptonhoruzon/api/kempt-data-cleaner-validator) · [Page to Markdown & Metadata](https://rapidapi.com/Kemptonhoruzon/api/kempt-page-to-markdown-metadata) · [US Federal Data](https://rapidapi.com/Kemptonhoruzon/api/kempt-us-federal-data)
- Support: kempthorizon@mail.grokbot.com
