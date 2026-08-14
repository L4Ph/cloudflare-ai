---
"@cloudflare/tanstack-ai": minor
---

Add `byokAlias` on AI Gateway **credentials / REST** config so OpenAI, Anthropic, Gemini, Grok, OpenRouter, and Workers AI (gateway REST) can select a stored BYOK key via `cf-aig-byok-alias`. The AI binding does not honor this header for third-party models. Gemini maps the header through `httpOptions.headers` (it does not use `createGatewayFetch`).
