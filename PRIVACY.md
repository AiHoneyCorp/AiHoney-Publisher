# Privacy

AiHoney Publisher is designed as a local Windows desktop application for creators who manage and publish their own media.

## Data handled by the application

Depending on the platforms a user connects, AiHoney Publisher may process:

- media files selected by the user
- titles, descriptions, tags, scheduling information, and platform-specific metadata
- publishing destinations selected by the user
- account identifiers returned by connected platforms
- OAuth tokens or browser-session information required to publish on the user's behalf
- local publishing history, retry state, and scheduling state

## Local-first operation

Media preparation, review, scheduling state, and publishing workflow data are primarily handled locally on the user's computer.

AiHoney Publisher does not require users to upload their local media library to AiHoney-operated storage merely to prepare or schedule posts.

## Platform authentication

Where a platform provides OAuth, AiHoney Publisher is intended to use OAuth authorization rather than collecting the user's platform password.

Where browser-based integration is required, publishing uses the browser profile chosen by the user.

Authentication credentials, OAuth tokens, and browser-session information are not published in this GitHub repository.

## User control

Users choose:

- which files to import
- which assets to approve
- which platforms receive an asset
- which account or destination is used
- what metadata is submitted
- whether a post is published immediately or scheduled

AiHoney Publisher is not intended to perform artificial engagement, unsolicited messaging, automatic voting, or autonomous account creation.

## Third-party platforms

When the user publishes content, the selected content and metadata are transmitted to the relevant third-party platform according to that platform's API, OAuth, browser, privacy, and content policies.

Those platforms process data under their own terms and privacy policies.

## Public repository

This repository contains product and integration documentation only. It does not contain user media, production credentials, private OAuth secrets, or the proprietary AiHoney Publisher source code.

## Contact

Privacy enquiries: **aihoneyinfo@gmail.com**
