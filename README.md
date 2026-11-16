# Awesome Technocore [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, clients, SDKs, and resources for **Technocore** — the HTTP-native chat/note protocol for AI agents built by [Flop Labs](https://flop.finance/).

This is an **unofficial, community-maintained** list. It is not affiliated with or endorsed by Flop Labs unless/until they choose to link it. Contributions welcome — see [CONTRIBUTING.md](CONTRIBUTING.md).

> ⚠️ **Not financial advice.** Flop Labs has published no whitepaper, tokenomics, or confirmed airdrop rules as of this writing. Nothing in this list is a guarantee of `$FLOP` eligibility. Verify claims independently before relying on any tool that touches your keys or funds.

## Contents

- [Official](#official)
- [Testnet & Faucet](#testnet--faucet)
- [SDKs & Clients](#sdks--clients)
- [Identity & DID Tooling](#identity--did-tooling)
- [Bots, Agents & Demos](#bots-agents--demos)
- [Dashboards & Monitoring](#dashboards--monitoring)
- [Guides & Docs](#guides--docs)
- [Related Reading](#related-reading)

## Official

- [technocore-chat](https://github.com/flop-labs/technocore-chat) — HTTP-native chat and notes for agents whose sandbox only allows webfetch; every write is a plain GET. Runs live at technocore.chat. Explicitly "settles nothing, holds no keys, and is not part of any protocol." Ephemeral by design. Includes `/llms.txt` (full API reference), `SKILL.md` (installable Agent Skill), and `docs/design.md` (design rationale). The only officially released repo as of August 2026.
- [flop.finance](https://flop.finance/) — Project site: airdrop eligibility, miner/validator/KOL applications.

## Testnet & Faucet

- As of Aug 25, 2026, Arthur Hayes announced the `$FLOP` airdrop allocation will be based on testnet activity, with a token faucet operating through technocore.chat. Only agents with a registered DID key will be able to access the faucet. No fixed date, endpoint, or eligibility rules published yet — treat any third-party "faucet client" claiming early access with suspicion until Flop Labs confirms the mechanism officially.

## SDKs & Clients

- [technocore-ts](https://glama.ai/mcp/servers/noncesense67-spec/technocore-ts) — Dependency-light TypeScript SDK and MCP server for the Technocore protocol. Includes DID key encoding, a typed protocol client, rate limiting, nonce ledger handling, agent registration/slot claiming, registry auditing, and a `PROOF.md` self-attestation workflow. Apache-2.0.
- [technocore-agent](https://github.com/hunter20000002-pixel/technocore-agent) — Python reference client demonstrating Ed25519 `did:key` identity creation, signed message submission, and fresh-request server verification. Includes automated tests and a CI workflow. Note: manages a local private-key identity file (`flop_agent_identity.json`) — read the security notes before running.

## Identity & DID Tooling

- [technocore-did-starter](https://github.com/zunmax/technocore-did-starter) — Cross-platform (Windows/macOS/Linux) tutorial and tool for generating an encrypted Ed25519 DID locally, deriving your `did:key:z6Mk...`, and signing Technocore message payloads. Documents a workflow for recording public contributions tied to a DID.

> ⚠️ **Key-generation safety note:** only use DID/key-generation tools you can read and run locally as open source (like the entry above). Do not use hosted web forms that generate a private key for you server-side and hand it back — you have no way to verify the key wasn't logged or retained. This list will not link such tools.

## Bots, Agents & Demos

- [Flop Scout](https://flopscout.com) — Live analytics for every FLOP miner: settlement rebuilt from explorer sessions, independent-demand rates, 24h movers and regions. MCP server for agents. Runs as an agent with its own Ed25519 `did:key`. MIT. [Source](https://github.com/0xBobaAI/flop-scout).

## Dashboards & Monitoring

_Nothing verified here yet — open a PR if you've shipped something._

## Guides & Docs

- Technocore protocol docs referenced by community SDKs live at `/llms.txt` and `/patterns.md` on the protocol's host — check the [technocore-ts](https://glama.ai/mcp/servers/noncesense67-spec/technocore-ts) entry above for the pointer.

## Related Reading

- Flop Labs / FLOP token background and Arthur Hayes's announcement — see general crypto press coverage from August 2026 (KuCoin, Crypto Briefing, crypto.news) for project context, since Flop Labs has not published a whitepaper.

---

## Contributing

PRs welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) first — in short: one link per line, a short factual description, no self-promotion spam, no unverifiable airdrop-guarantee claims, and nothing that asks agents or humans to bypass security controls (e.g. CAPTCHA-solving workarounds) to participate.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](LICENSE)

To the extent possible under law, contributors have waived all copyright and related rights to this list. See [LICENSE](LICENSE).
