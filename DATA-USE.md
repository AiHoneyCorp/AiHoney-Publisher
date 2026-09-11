# Data Use

AiHoney Publisher uses platform data only to provide creator-directed publishing and scheduling functionality.

## Intended uses

Depending on the connected platform, AiHoney Publisher may read limited account and destination information such as:

- the authenticated account identity
- available publishing destinations
- subscription tiers, galleries, communities, subreddits, or similar destination metadata
- platform-specific posting options required to create a post
- publishing status and returned post URLs

This information is used to let the user choose where their own content should be published and to verify that publishing occurs under the intended account.

## Reddit-specific intended use

For Reddit, AiHoney Publisher intends to use OAuth/Data API access to allow an authenticated user to:

- identify the Reddit account they connected
- publish user-selected text, link, and image posts
- publish to the user's own profile or a subreddit selected by the user
- retrieve posting options such as available flair where appropriate
- mark posts NSFW or spoiler when selected by the user
- receive the created Reddit post URL/status

AiHoney Publisher does not intend to use Reddit data to:

- train machine-learning models
- build user profiles for advertising
- sell or broker Reddit data
- automate voting
- manufacture engagement
- mass-comment
- scrape Reddit for unrelated datasets
- send unsolicited messages
- create accounts automatically

## Retention

Local publishing metadata and history may be retained on the user's device so AiHoney can prevent accidental duplicate publishing, maintain schedules, and provide retry/history information.

Platform access tokens are retained only as required to maintain the user's authorized connection and should be protected using platform-appropriate secure credential storage in production builds.

## User-directed actions

Publication is based on media, metadata, destinations, and schedules selected by the authenticated user. AiHoney Publisher is intended as a workflow and automation tool for the user's own publishing activity, not as an autonomous engagement bot.

## Contact

Data-use enquiries: **aihoneyinfo@gmail.com**
