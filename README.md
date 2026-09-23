# Maya Architecture Docs

Public architecture diagrams and capability mapping for **Maya Travel AI**
(Anamaya / yBizTrip).

**Live site:** https://anamaya-maya.github.io/maya-architecture-docs/

Modeled on the Raisd campus public docs pattern
([raisd-campus/portal-api-docs](https://raisd-campus.github.io/portal-api-docs/)).

## Pages

| Page | Purpose |
|------|---------|
| [`index.html`](index.html) | Hub — one-line truth + TOC |
| [`architecture.html`](architecture.html) | Maya → Anamaya MCP → OMS |
| [`capabilities.html`](capabilities.html) | Must-know · may-share · never invent · tools |
| [`path.html`](path.html) | One chat turn + corporate ESPPD spine |

## One-line truth

Chat goes **Traveler → maya-api → Anamaya MCP → OMS**.
MCP holds behaviour / session context — **not** a flight/hotel inventory database.
Offers are always live OMS queries through MCP.

## Source of truth

Private specs remain in
[`maya-travel-ai-control-plane`](https://github.com/anamaya-maya/maya-travel-ai-control-plane).
Keep this public copy in sync when architecture / capability boundaries change.

## Local preview

```bash
python3 -m http.server 8765
# open http://127.0.0.1:8765/
```

## License

Documentation © Anamaya.AI / Maya Travel AI contributors.
Internal product architecture published for partner review.
