# Reddit Integration

## Purpose

AiHoney Publisher is a Windows desktop publishing application for creators who want to prepare, schedule, and publish their own media across multiple platforms from one local workflow.

The Reddit integration is intended to let a user connect **their own Reddit account via OAuth** and publish **their own selected content** to destinations they explicitly choose.

## Intended Reddit functionality

An authenticated user will be able to:

- publish to their own Reddit profile
- publish to a subreddit they select and are permitted to post in
- create image posts
- create link posts
- create text posts
- select Reddit-specific metadata before publishing
- schedule Reddit posts through AiHoney Auto-Calendar
- receive the resulting Reddit post URL and publication status

For video assets, AiHoney may first publish the user's selected video to RedGIFs and then create a Reddit link post using the resulting RedGIFs URL.

## Reddit-specific metadata

Planned Reddit metadata includes:

- destination type: profile or subreddit
- subreddit name
- post title
- post type
- body text
- URL
- flair, where available
- NSFW flag
- spoiler flag

AiHoney may read available flair or other posting options from the selected subreddit only to help the user create a valid post.

## User control

The user remains responsible for selecting:

- the media to publish
- the Reddit destination
- the title and body
- the subreddit
- flair or post flags
- immediate versus scheduled publication

AiHoney does not intend to select unrelated communities autonomously or publish indiscriminately across Reddit.

## Actions AiHoney does not automate

The Reddit integration is **not** intended to automate:

- voting or vote manipulation
- mass commenting
- artificial engagement
- unsolicited direct messages
- account creation
- subreddit joining
- moderation actions without explicit user direction
- bulk Reddit scraping
- collection of Reddit data for resale
- advertising profiles
- machine-learning training datasets

## Why Devvit is not sufficient

AiHoney Publisher is an external Windows desktop application that coordinates local media files, editing, metadata, scheduling, and publication across multiple independent platforms.

The application needs the authenticated user to be able to select local files on their computer and publish them through a unified desktop workflow alongside non-Reddit destinations such as DeviantArt, X, RedGIFs, and Fanvue.

Devvit is designed for applications hosted within Reddit's ecosystem. It does not provide the architecture required for AiHoney's external desktop workflow, local media pipeline, cross-platform scheduler, and account-specific desktop publishing environment.

For that reason AiHoney requires an OAuth/Data API integration for Reddit rather than implementing its core desktop workflow as a Reddit-hosted Devvit application.

## OAuth and credentials

The intended production connection flow is:

1. The user selects **Connect Reddit** in AiHoney Publisher.
2. Reddit's OAuth authorization page opens.
3. The user signs into/chooses their own Reddit account and grants the requested permissions.
4. AiHoney receives the authorized account connection.
5. The user can publish only through that connected account until they disconnect or reconnect another account.

AiHoney does not require the user's Reddit password.

OAuth access/refresh tokens will be treated as confidential credentials and will not be committed to this public repository.

## Requested access

AiHoney seeks only the API access necessary to identify the authenticated account, create user-directed posts, retrieve necessary posting options, and return publication status/URLs.

The application is being developed as a creator publishing tool, not as an engagement bot or Reddit data collection product.

## Development status

The Reddit integration is currently under development. Browser-based prototypes were used only to validate publishing workflow assumptions; the intended production architecture is the official Reddit OAuth/Data API.

## Contact

Reddit integration enquiries: **aihoneyinfo@gmail.com**
