# trask

Source-backed question answering for KOTOR modding and troubleshooting: answers come with citations from an approved source list, or the bot says it does not know.

## Scope

- Discord bot and HTTP API
- Retrieval, source policy and answer composition packages
- Indexer (Python) and ingest worker
- Cloudflare Workers for the public API, retrieval and scheduled reindexing
- Web UI

## Contracts

- Sign-in: client of the org-wide OpenID Connect service. No login code lives here.
- Discord plumbing: `kolto-bot-kit`.

## Status

Scaffold. Code is being migrated from `OpenKotOR/community-bots` with history, one draft pull request at a time. The licence has not been chosen yet, so no licence is granted until a `LICENSE` file lands.

Kolto Labs is an independent, non-commercial fan project, not affiliated with Lucasfilm, Disney, BioWare, Electronic Arts, Obsidian, Aspyr or Saber Interactive. This repository contains no game assets.
