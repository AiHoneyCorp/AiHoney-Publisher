# Security

AiHoney Publisher is a private-source Windows desktop application. This public repository contains documentation only.

## Security principles

AiHoney Publisher is designed around the following principles:

- credentials and OAuth secrets are never committed to this repository
- users should not provide AiHoney with platform passwords when OAuth is available
- platform access is scoped to the publishing functionality required by the connected account
- publishing actions remain tied to the account and destination selected by the user
- persistent scheduling and retry state is kept isolated per Publisher Profile
- the application performs account-identity checks before publishing to reduce accidental cross-account posting

## Reporting a security issue

Please do **not** disclose suspected vulnerabilities, tokens, credentials, private account information, or exploit details in a public GitHub issue.

Report security concerns privately to:

**aihoneyinfo@gmail.com**

Please include:

- affected AiHoney Publisher version
- affected platform/integration
- steps to reproduce
- expected and observed behavior
- any relevant logs with credentials/tokens removed

## Secrets and credentials

Never commit or post:

- OAuth client secrets
- OAuth refresh/access tokens
- browser cookies/session credentials
- API keys
- private platform identifiers that should remain confidential
- user media that is not intended to be public

## Repository scope

No production application source code is distributed from this documentation repository. Security-sensitive implementation details may be shared privately with platform reviewers when required.
