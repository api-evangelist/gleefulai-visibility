# Visibility (GleefulAI)

API Evangelist catalog entry for [Visibility](https://visibility.gleefulai.com) by
[GleefulAI](https://gleefulai.com) — an AI-visibility and answer-engine-optimization audit API.
It scores how visible and understandable a website is to AI assistants and agents, then generates
the artifacts to improve it.

| | |
|---|---|
| Spec | OpenAPI 3.1.0 — 22 paths, 36 operations |
| Auth | **None.** No API keys — paid per call via x402 micropayments in USDC on Base |
| Base | `https://visibility.gleefulai.com` |

Every path answers both `GET` and `POST`. Coverage spans audit scoring at three depths, fix
generation, competitor gap analysis, bot-access auditing, citation checking, and generation of
`llms.txt` and schema markup.

The payment model is the interesting part: with no keys and no signup, an agent holding a wallet
can call it directly. That is a genuinely different onboarding shape from the rest of the catalog.

## Known gaps

Recorded in `apis.yml` under `x-evidence`, and reported to the submitter:

- **No schemas** — 36 operations with no `components.schemas`, so request and response bodies are
  undescribed.
- **`info.version: 0.1.0`** — reads as pre-release to anything parsing the API's own version.

## This is a catalog entry, not GleefulAI

This repo is API Evangelist's profile *about* Visibility. For the product or support, go to
[visibility.gleefulai.com](https://visibility.gleefulai.com).

If something here is wrong, open an issue on this repo or in the
[APIs.io Inbox](https://github.com/api-search/inbox).
