# API Access & Developer Resources

A placeholder repository for documenting legitimate API access options and developer resources.

[![Security first](https://img.shields.io/badge/Practice-Never%20commit%20secrets-critical)](https://docs.github.com/en/code-security/secret-scanning/about-secret-scanning)

## Current status

This repository currently contains only this README. It does **not** yet contain a verified API catalogue, provider integrations, or runnable code. No API key or token should be added to this repository.

## Intended scope

When this repository is expanded, entries should include:

- Provider and official documentation link
- What the API is for
- Free-tier limits and restrictions, verified from the provider
- Authentication method and setup instructions
- Rate limits, data handling, and attribution requirements
- Last verification date

Do not label an API as “free” without checking its current official terms. Free tiers can change and may require payment details.

## Safe credential handling

- Never commit API keys, access tokens, passwords, or private client secrets.
- Store local credentials in environment variables or an ignored `.env` file.
- Commit only a `.env.example` file containing placeholder values.
- If a secret is exposed, revoke/rotate it with the provider; deleting it from the latest commit alone is not sufficient.

Example local configuration:

```bash
# Example only — replace with a credential stored locally
export SERVICE_API_KEY="your_key_here"
```

Application code should read the environment variable rather than embedding the value in source code.

## Repository structure

```text
.
└── README.md
```

## Contribution checklist

Before adding a provider, verify its official documentation and terms, include a source link, state the date checked, and ensure the entry contains no real credentials.

## Maintenance

- **Review date:** 10 November 2026.
- **Validation:** No API catalogue or integration has been tested because none is present yet.
