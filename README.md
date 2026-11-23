# trask

Source-backed question answering for KOTOR modding and troubleshooting: answers come with citations from an approved source list, or the bot says it does not know.

## Scope

- Discord bot and HTTP API
- Retrieval, source policy and answer composition packages
- Retrieval index built from the HoloVec corpus
- Cloudflare Workers for the public API, retrieval and scheduled reindexing
- Web UI

## Contracts

- Sign-in: client of the org-wide OpenID Connect service. No login code lives here.
- Corpus: [`holovec`](https://github.com/kolto-labs/holovec) owns acquiring and archiving the sources. Trask reads that corpus and does not crawl or ingest the same sources itself.
- Discord plumbing: `cantina` (packages `@kolto-labs/cantina-*`).

## Status

Scaffold. Code is being migrated from `OpenKotOR/community-bots` with history, one draft pull request at a time. The licence has not been chosen yet, so no licence is granted until a `LICENSE` file lands.

Kolto Labs is an independent, non-commercial fan project, not affiliated with Lucasfilm, Disney, BioWare, Electronic Arts, Obsidian, Aspyr or Saber Interactive. This repository contains no game assets.
