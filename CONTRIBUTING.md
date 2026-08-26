# Contributing to Awesome Technocore

Thanks for helping build this out. A few ground rules so the list stays useful and trustworthy:

## What belongs here

- Tools, SDKs, clients, bots, dashboards, or docs that work **with** the Technocore protocol.
- Entries you (or someone you can vouch for) have actually run. Don't list vaporware.
- Original write-ups/guides that help newcomers understand the protocol.

## What doesn't belong here

- Anything that instructs agents or humans to bypass security controls (CAPTCHA workarounds via social engineering, rate-limit evasion, credential stuffing, etc.) to participate in Technocore or farm airdrop eligibility. This list is for building useful things, not gaming anti-abuse systems.
- Sybil-farming toolkits (mass DID generation scripts with no other functionality).
- **Hosted key-generation tools.** Any "DID assistant" or similar web app that generates an Ed25519 private key *for* the user server-side (rather than providing open-source code the user runs locally) will not be listed, regardless of how legitimate it looks. There's no way for a reader to verify the key wasn't logged or retained. If you're unsure whether a tool qualifies, err on the side of not submitting it.
- Unverifiable claims about guaranteed `$FLOP` airdrop eligibility. Flop Labs has not published official rules — say what a tool *does*, not what you assume it *earns*.
- Pure self-promotion with no working link or with a link to a private/paywalled repo.

## How to submit

1. Fork the repo.
2. Add your entry under the most relevant section in `README.md`, alphabetically within its section.
3. Use this format:
   ```markdown
   - [Project Name](https://link) — One or two sentence factual description. License if known.
   ```
4. Open a PR. Include a one-line note on how you verified the project works (ran it, read the source, etc).

## Style

- Keep descriptions factual and short (under ~40 words).
- No emoji spam, no ALL CAPS, no "🚀🚀🚀 must see 🚀🚀🚀".
- If a project requires a private key, encrypted key, or signs on-chain/off-chain messages, say so explicitly in the description so readers know before they click through.
