<!--lint disable awesome-github-->
<!-- GitHub metadata is reviewed separately from list content. -->

# Awesome Poppy 🌸 [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

Discover, build, and experiment with the **Personal Agent Protocol**.

A curated collection of docs, SDKs, demos, and tools for personal AI agents to discover companies, obtain user-authorized access, and get things done.

Awesome Poppy is a community-maintained list, not an official Poppy resource. Inclusion does not imply review or endorsement by the Poppy authors.

**Release status:** Sierra announced Poppy 1.0 on November 13, 2026. When checked that day, the official specification and [changelog](https://personalagentprotocol.org/docs/changelog) still labeled 1.0 as a draft. Community projects target different versions and draft snapshots, and vary in coverage and maturity.

## Contents

- [🌱 Start Here](#-start-here)
- [🛠 Build with Poppy](#-build-with-poppy)
- [🎮 Try a Demo](#-try-a-demo)
- [🔎 Check Your Implementation](#-check-your-implementation)
- [🌐 Explore the Ecosystem](#-explore-the-ecosystem)

<a id="official-resources"></a>
<a id="introductions"></a>

## 🌱 Start Here

New to Poppy? Start with the overview, then explore an example before diving into the specification.

- [Personal Agent Protocol](https://personalagentprotocol.org) - Explore the official home and interactive walkthroughs with fictional companies.
- [Protocol Introduction](https://personalagentprotocol.org/docs/introduction) - Learn the goals, access controls, and design principles.
- [Releasing Personal Agent Protocol 1.0](https://sierra.ai/blog/releasing-poppy) - Read Sierra's release announcement, including its reports of Shopify's rollout, support in Meta's Muse, and new design partners.

<a id="developer-guides"></a>

## 🛠 Build with Poppy

**Official documentation** — Start with the specification and implementation guides, then explore optional extensions.

- [Specification](https://personalagentprotocol.org/docs/1.0/spec) - Read the 1.0 specification for discovery, sessions, authorization, web browsing, APIs, and conversations.
- [Implementation Guides](https://personalagentprotocol.org/docs/1.0/guides) - Apply recommended practices for metadata fetching, secrets, retries, and token handling.
- [Extensions](https://personalagentprotocol.org/docs/1.0/extensions) - Learn how optional extensions are advertised and versioned separately from the core protocol.
- [Operations Extension](https://personalagentprotocol.org/docs/1.0/extensions/operations) - Follow the optional version 3 flow for approving exact action terms and retrying requests with protection against duplicate execution.
- [Official Company Implementation Kit](https://personalagentprotocol.org/kit/company) - Build company-side Poppy Draft 1.0 support with a coding-agent skill and validator; some requirements need manual review.
- [UCP Extension](https://personalagentprotocol.org/docs/1.0/extensions/ucp) - Use the optional version 1 extension to connect Poppy discovery and sign-in with UCP shopping, checkout, and conversations.

<a id="community-sdks-and-integrations"></a>

**Community SDKs and integrations** — Choose a starting point for your language or agent; check each project's supported flows.

- [Datalayer Personal Agent Protocol SDKs](https://github.com/datalayer/personal-agent-protocol) - Use community Python and TypeScript SDKs targeting Poppy 0.4 by default, with opt-in support for the November 11, 2026 Draft 1.0 snapshot and Operations v3.
- [pi-poppy](https://github.com/richardanaya/pi-poppy) - Add Draft 0.1 sessions, conversations, API/MCP access, and operation approvals to the Pi coding agent; default client metadata is local and cannot be fetched by remote companies.
- [Poppyseed](https://github.com/akshay5995/poppyseed) - Explore a community TypeScript implementation targeting a Draft 0.3 snapshot, with a Next.js adapter, OAuth/DPoP, MCP/OpenAPI tools, conversations, and Operations v1.
- [PoppyKit server](https://github.com/LMol-4/poppykit-server) - Explore a community TypeScript server implementation built for a Poppy Draft 0.3 snapshot.
- [PoppyKit client](https://github.com/LMol-4/poppykit-client) - Explore a community TypeScript client implementation built for a Poppy Draft 0.3 snapshot.

<a id="community-demos"></a>

## 🎮 Try a Demo

See the protocol in action through community examples. Demo flows do not establish full conformance.

- [Poppy on Cloudflare Workers](https://github.com/irvinebroque/poppy-demo) - Run a two-Worker demo of discovery, direct sign-in, conversations, and synthetic jacket exchanges targeting a November 8, 2026 Draft 0.4 snapshot; its hosted receiver still advertises 0.1.
- [Print with Poppy](https://github.com/spenciefy/print-with-poppy) - Explore photo ordering with Poppy 0.4, signed Session headers, OpenAPI, and Operations v3; its sandbox simulates payment and fulfillment.

<a id="developer-tools"></a>

## 🔎 Check Your Implementation

Use a web checker for a quick look at published metadata, or a CLI for repeatable local and CI checks.

- [PAP Checker](https://papchecker.com) - Check public metadata for versions 0.1–0.4 and the November 11, 2026 Draft 1.0 snapshot in a community web tool, with per-rule reports and a `poppy.json` directory; no live sessions are tested.
- [poppy-validator](https://github.com/tusharck/poppy-validator) - Validate local files or live Draft 0.1 discovery URLs with an unofficial Python CLI, JSON Schema checks, OAuth metadata cross-checks, and JSON reports for CI.
- [Allowfy Check](https://github.com/allowfy/allowfy-check) - Test live Draft 0.2 discovery, sessions, device sign-in, account tokens, sign-out, and Operations flows with a community CLI and per-check reports.

## 🌐 Explore the Ecosystem

**Follow development** — Track the protocol, source changes, and open design work.

- [Official Poppy Repository](https://github.com/personal-agent-protocol/personal-agent-protocol) - Browse the specification, documentation website, company implementation kit, revision history, and issues.
- [Roadmap](https://personalagentprotocol.org/docs/roadmap) - Follow open work on payment approvals, push notifications, attachments, and self-hosted personal agents.

<a id="development-and-design-partners"></a>

**Development and design partners** — The [official roster](https://personalagentprotocol.org/docs/path-to-1#partners), checked November 13, 2026, lists 103 partners: 4 personal agents and 99 companies. All 60 new partners named in Sierra's 1.0 announcement are included below. Participation does not establish a live implementation or a specific code contribution, and this roster does not cover every community contributor.

<details>
<summary>View all 103 development and design partners</summary>

| Official group  | Listed partners                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Personal agents | Instinct, Manus, Meta, OpenAI.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Companies       | 1Password, Adyen, Affirm, Aflac, Agoda, Aircall, Akoya, Atomic, Aviva, Banco Sabadell, Bank of America, BBVA, Braze, Browserbase, Checkout.com, Chime, Cigna, Cisco, Cloudflare, Comcast, Cover Genius, Creditas, Crunch Fitness, Cue, Delta Air Lines, Descope, DIRECTV, EarnIn, ElevenLabs, Five9, FOX, Freshworks, Fullstory, Gap Inc., GEICO, Gen Digital, Genesys, Global Payments, GoFundMe, GoodRx, Guardian, HealthEx, HelloFresh, Hertz, Hyatt, Infoblox, Insurify, Intuit, Kernel, Kin Insurance, Klaviyo, Lemonade, Liberty Global, Liberty Mutual, Mastercard, Mercury, Navy Federal Credit Union, Neptune Flood, NiCE, Nordstrom, Notion, Okta, OneSignal, Ora, PayPal/Venmo, Persona, Pindrop, Ping Identity, Plaid, Profound, Prosus, Remitly, Rocket, Runlayer, Salesforce (Fin, Commerce Cloud, and Agentforce), Shopify, Sierra, SiriusXM, Socure, SoFi, Stripe, Symphony by Wix, Synchrony, Target, The Knot, The Zebra, Travelers, Turkish Airlines, Twilio, United Airlines, Visa, Walmart, Wayfair, Wells Fargo, Wix, WorkOS, Zapier, Zendesk, Zoom. |

</details>

<a id="related-protocols"></a>

**Related protocols** — These have their own specifications; inclusion does not imply Poppy compatibility.

- [Model Context Protocol (MCP)](https://modelcontextprotocol.io/docs/getting-started/intro) - Connect AI applications to tools and data; Poppy includes MCP as an API interface companies can offer.
- [Universal Commerce Protocol (UCP)](https://ucp.dev) - Explore the commerce protocol used by Poppy's UCP extension for catalog search, carts, and checkout.
- [Personal Agent Consent & Trust (PACT)](https://github.com/openpactprotocol/openpactprotocol) - Explore a separate protocol built on A2A and OAuth, with schemas, a client, and a reference stack; it is not Poppy.

## Contributing

Found something useful? Read [CONTRIBUTING.md](CONTRIBUTING.md), then open a pull request or use the resource submission issue template. Small, verified additions and corrections are welcome.
