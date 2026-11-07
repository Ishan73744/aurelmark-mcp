# Aurelmark MCP: sanctions changes and EU official data

Remote MCP server (Streamable HTTP) for AI agents: official sanctions-list changes and EU compliance data, each answer with its official source and date.

**Endpoint:** `https://aurelmark.live/mcp` · **Docs:** https://aurelmark.live/docs · **Official MCP Registry:** `io.github.Ishan73744/aurelmark`

## Tools

| Tool area | What it returns | Official source |
|---|---|---|
| Sanctions list changes | Who was added to, amended on or removed from the lists; name search; single entries | US OFAC SDN, UK Sanctions List (FCDO), EU Financial Sanctions Files |
| EU compliance deadlines | Dated obligations for CBAM, EUDR, AI Act, CSRD, CSDDD and more, with the legal article | EUR-Lex / Official Journal |
| CBAM | Default embedded emissions and estimated cost per CN code and origin; certificate price | Commission Implementing Regulation (EU) 2025/2621 as amended, Commission price page |
| EUDR | Whether a CN/HS code is in scope of the EU deforestation regulation | Regulation (EU) 2023/1115 Annex I |
| EU contract winners | Who won which public contract, with buyer, value, CPV and country | TED award notices |
| EU grant calls | New, amended and closed EU Funding & Tenders calls | EU Funding & Tenders portal |
| EU trade defence | Anti-dumping, countervailing and safeguard measures and quotas by CN code and origin | EU acts |

Sanctions data is a monitoring feed of what the official lists say, not a sanctions clearance decision or legal advice. The UN list is not included.

## Connect

```json
{
  "mcpServers": {
    "aurelmark": { "type": "http", "url": "https://aurelmark.live/mcp" }
  }
}
```

## Pricing

- Keyless: 10 successful calls per caller per day on metered tools.
- Optional API key (`Authorization: Bearer <key>`) with prepaid credits.
- The same data over REST and x402 pay-per-call on Base: 2 US cents per answer with records; empty answers and errors are free. Catalogue: https://aurelmark.live/.well-known/x402

## Contact

hello@aurelmark.live · https://aurelmark.live

This repository only describes the hosted server; the service itself runs at aurelmark.live.
