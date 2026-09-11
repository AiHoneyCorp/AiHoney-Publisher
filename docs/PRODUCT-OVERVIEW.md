# Product Overview

AiHoney Publisher is a Windows desktop workspace for creators who publish media across several online platforms.

The product brings the repetitive parts of the publishing workflow into one place: importing media, reviewing it, applying lightweight edits, setting platform-specific metadata, scheduling posts, connecting publishing accounts, and monitoring publication results.

## Workflow

A typical AiHoney Publisher workflow is:

1. Import selected images and videos.
2. Review each asset and approve, hold, or reject it.
3. Apply optional edits such as crop, blur, censor overlays, and link overlays.
4. Assign platform-specific metadata and destinations.
5. Schedule content through Auto-Calendar or mark it for immediate publication.
6. Publish to the connected accounts selected by the user.
7. Record success, failure, retry, ignored, and publication-history state locally.

## Multi-platform design

Different platforms expose different publishing capabilities. AiHoney therefore separates common creator metadata from platform-specific metadata.

Examples include:

- DeviantArt subscription tiers and galleries
- Reddit profile/subreddit, flair, post type, NSFW, and spoiler options
- X profile/community destination
- Fanvue audience/paywall metadata
- RedGIFs video hosting and returned publication URLs

## Auto-Calendar

Auto-Calendar is the persistent scheduling layer. It maintains future publication state across sessions, supports redistribution and manual movement between days, and can reconnect required platform sessions close to publication time.

## Local-first architecture

AiHoney Publisher is designed as a local desktop application. Media preparation, review state, metadata, schedules, and history remain associated with the user's local Publisher Profile. Only the content and metadata required for publication are transmitted to the platform selected by the user.

## Audience

AiHoney Publisher is being developed for creators who want multi-platform publishing automation without having to understand APIs, browser automation, OAuth internals, or individual platform upload workflows.

The long-term product goal is simple account connection followed by a consistent review → metadata → schedule → publish workflow across supported platforms.
