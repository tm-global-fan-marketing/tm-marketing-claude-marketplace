# tm-marketing-core Plugin

This plugin provides marketing skills and the LN Confluence connector for Ticketmaster's central marketing org (B2C and B2B teams).

## Skills

When the user's request matches a trigger below, invoke the corresponding skill IMMEDIATELY as your first action before responding or taking any other steps.

| Skill | Triggers When |
|---|---|
| `tm-marketing-core:marketing-wizard` | Any general marketing request that doesn't explicitly name another skill — use this as the default entry point; it classifies and routes to the right skill |
| `tm-marketing-core:backstage-writer` | User asks to write, rewrite, or review copy in the TM/LN brand voice, check tone/voice, or work with Fan Support, Product/UX, B2C, or B2B copy for a named product or messaging pillar |
| `tm-marketing-core:brief-writer` | User asks to draft a Campaign and Creative Brief (B2C only) |
| `tm-marketing-core:content-creator` | User needs a coordinated set of two or more B2B marketing assets (blog, case study, LinkedIn post, one-sheet, email, etc.) for a single campaign or theme |
| `tm-marketing-core:social-pulse` | User wants to check social performance (Instagram, Facebook, X, TikTok) against market history or peer markets, or wants a testable content idea grounded in what's working elsewhere |

## LN Confluence Connector

The `ln-confluence` MCP connector is available for all skills. Use it proactively:

**Do not produce final copy, a translation, or a campaign brief without first searching Confluence for relevant guidelines or prior work, unless the user explicitly waives this step.**

- **Before writing copy:** Search Confluence for brand guidelines, tone of voice docs, and approved messaging.
- **Before planning a campaign:** Search Confluence for existing campaigns, briefs, and channel strategies relevant to the audience or product.
- **When producing a report or plan:** Offer to publish the output back to Confluence when the user is satisfied with the result.

The `ln-confluence` connector authenticates via SSO — no API key is required.
