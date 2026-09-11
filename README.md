# AiHoney Publisher

**AiHoney Publisher** is a Windows desktop application for reviewing, preparing, scheduling, and publishing creator media across multiple platforms from one local workflow.

> **Development status:** Private development / pre-release.  
> This repository contains public product and integration documentation only. The production source code is maintained privately.

## What AiHoney Publisher does

AiHoney Publisher is designed to reduce repetitive publishing work while keeping the creator in control of what is posted, where it is posted, and when it is posted.

The application combines:

- media import and review
- image/video preparation and lightweight editing
- platform-specific metadata
- account and destination selection
- scheduling through Auto-Calendar
- immediate publishing
- persistent publishing history and failure handling
- multi-platform publishing from one desktop workspace

## Platform integrations

| Platform | Status | Integration model |
| --- | --- | --- |
| DeviantArt | Working integration | Dedicated browser bridge |
| X | Working integration | Dedicated browser bridge |
| RedGIFs | Working integration | Dedicated browser bridge / authenticated web API flow |
| Fanvue | Working integration in testing | Official OAuth/API |
| Reddit | In development | Intended official OAuth/Data API integration |
| Additional creator platforms | Planned | Platform-dependent |

See [PLATFORM-INTEGRATIONS.md](PLATFORM-INTEGRATIONS.md) for more detail.

## User control

AiHoney Publisher is built around explicit creator actions. Users choose the content, destination, metadata, account, and publishing schedule. The application is not intended to automate voting, artificial engagement, mass commenting, unsolicited messaging, account creation, or other manipulative activity.

## Reddit integration

The intended Reddit integration allows an authenticated user to publish their own selected content to their own Reddit profile or to subreddits they choose and are permitted to post in.

Planned Reddit-specific metadata includes:

- profile or subreddit destination
- subreddit
- post title
- post type
- body text
- URL
- post flair
- NSFW status
- spoiler status

See [REDDIT-INTEGRATION.md](REDDIT-INTEGRATION.md) for the full integration description.

## Privacy and security

AiHoney Publisher is a local desktop application. Platform credentials, OAuth tokens, and user media are not published in this repository.

See:

- [PRIVACY.md](PRIVACY.md)
- [SECURITY.md](SECURITY.md)
- [DATA-USE.md](DATA-USE.md)

## Documentation-only repository

This repository exists to provide public product, privacy, security, and platform-integration documentation for AiHoney Publisher. It does **not** contain the application source code, private platform credentials, OAuth secrets, or user data.

For a higher-level product description, see [docs/PRODUCT-OVERVIEW.md](docs/PRODUCT-OVERVIEW.md).

## Roadmap

Current development priorities include broadening official platform integrations, improving automated scheduling and retry flows, and simplifying account connection for a mass-market creator audience.

See [ROADMAP.md](ROADMAP.md).

## Contact

For product, security, or platform-integration enquiries:

**AiHoney**  
Email: **aihoneyinfo@gmail.com**

---

© 2026 AiHoney. All rights reserved. This repository contains product documentation only and does not grant a license to the AiHoney Publisher application or its source code.
