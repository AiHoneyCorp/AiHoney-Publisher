# Platform Integrations

AiHoney Publisher is designed as a multi-platform publishing workspace. Different platforms expose different integration models, so AiHoney uses official APIs where practical and browser-assisted publishing where necessary.

## Current status

### DeviantArt

**Status:** Working integration

AiHoney supports account-aware publishing, subscription-tier discovery, gallery/destination mapping, scheduling, metadata transfer, and Auto-Calendar publication through a dedicated browser bridge.

### X

**Status:** Working integration

AiHoney supports creator-directed publishing through a dedicated browser session. Community targeting is planned as a platform-specific destination option where supported by the connected account.

### RedGIFs

**Status:** Working integration

AiHoney supports video publication and capture of the resulting RedGIFs URL. This can be reused by other platform integrations that require or benefit from an external video URL.

### Fanvue

**Status:** Working integration in testing

Fanvue uses its official OAuth/API integration. The current development path supports authenticated account connection, media upload, media-processing status, and post creation.

### Reddit

**Status:** In development

The intended production implementation uses Reddit OAuth/Data API access rather than fragile browser automation.

Planned Reddit publishing supports:

- user profile or subreddit destinations
- native image posts
- link posts
- text posts
- subreddit-specific metadata
- flair where available
- NSFW and spoiler flags
- creator-selected scheduling through AiHoney Auto-Calendar

For video assets, AiHoney may first publish the user's video to RedGIFs and then use the returned RedGIFs URL for the Reddit link post.

See [REDDIT-INTEGRATION.md](REDDIT-INTEGRATION.md).

## Integration philosophy

AiHoney aims to make platform connection easy for a mass-market creator audience. Production users should normally see a simple **Connect** or **Reconnect** action rather than having to understand API keys, tokens, redirect URIs, or developer tooling.

Where an official OAuth/API integration exists, AiHoney's long-term preference is to use it. Browser-assisted integrations are used where they are required or provide functionality not otherwise exposed to the desktop application.

## Account isolation

AiHoney Publisher Profiles are designed to keep platform account identity, destination mappings, schedule state, and publishing history separated. The application performs account-identity checks before publishing to reduce accidental publication under the wrong connected account.

## Additional platforms

Additional creator platforms are planned. New integrations are evaluated individually for:

- official API/OAuth availability
- media-upload support
- scheduling capabilities
- account/destination metadata
- rate limits and platform terms
- reliability for unattended Auto-Calendar publishing
