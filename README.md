<!--lint disable awesome-github-->
<!-- GitHub metadata is reviewed separately from list content. -->

# Awesome Poppy 🌸 [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

Discover, build, and experiment with the **Personal Agent Protocol**.

A curated collection of docs, SDKs, demos, and tools for personal AI agents to discover companies, obtain user-authorized access, and get things done.

Awesome Poppy is a community-maintained list, not an official Poppy resource. Inclusion does not imply review or endorsement by the Poppy authors.

**Draft status:** Poppy is at Draft 0.1, checked October 15, 2026. It may change incompatibly before a stable release; community projects vary in coverage and maturity.

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
- [Protocol Overview](https://personalagentprotocol.org/docs/overview) - Learn the goals, access controls, and design principles.
- [Sharing a Draft of Personal Agent Protocol](https://sierra.ai/blog/poppy) - Read Sierra's draft announcement and its account of the Rocket mortgage demo with Meta's Muse.

<a id="developer-guides"></a>

## 🛠 Build with Poppy

**Official documentation** — Start with the specification and implementation guides, then explore optional extensions.

- [Specification](https://personalagentprotocol.org/docs/spec) - Read the authoritative Draft 0.1 requirements for discovery, sessions, authorization, web browsing, APIs, and conversations.
- [Implementation Guides](https://personalagentprotocol.org/docs/guides) - Apply recommended practices for metadata fetching, secrets, retries, and token handling.
- [Extensions](https://personalagentprotocol.org/docs/extensions) - Learn how optional extensions are advertised and versioned separately from the core protocol.
- [Operations Extension](https://personalagentprotocol.org/docs/extensions/operations) - Follow the draft's optional version 1 flow for proposing, approving, confirming, and tracking actions.
- [Official Poppy Implementation Skill](https://personalagentprotocol.org/kit/company) - Add company-side Poppy Draft 0.1 support with an official coding-agent skill, implementation milestones, JSON Schemas, and a validator; sign-in checks remain manual.

<a id="community-sdks-and-integrations"></a>

**Community SDKs and integrations** — Choose a starting point for your language or agent; check each project's supported flows.

- [Datalayer Personal Agent Protocol SDKs](https://github.com/datalayer/personal-agent-protocol) - Community Python and TypeScript SDKs targeting Draft 0.1, with focused examples; Operations models exist, but a complete Operations workflow is not implemented.
- [pi-poppy](https://github.com/richardanaya/pi-poppy) - Add Draft 0.1 sessions, conversations, API/MCP access, and operation approvals to the Pi coding agent; default client metadata is local and cannot be fetched by remote companies.
- [Poppyseed](https://github.com/akshay5995/poppyseed) - Explore an early-stage TypeScript implementation with a Next.js adapter, OAuth/DPoP, MCP/OpenAPI tools, conversations, and operation approvals for Draft 0.1.

<a id="community-demos"></a>

## 🎮 Try a Demo

See the protocol in action through community examples. Demo flows do not establish full conformance.

- [Poppy on Cloudflare Workers](https://github.com/irvinebroque/poppy-demo) - Run a two-Worker example of discovery, direct sign-in, conversations, and a simulated jacket exchange using a synthetic account.
- [Print with Poppy](https://github.com/spenciefy/print-with-poppy) - Explore photo ordering with Draft 0.1 discovery, DPoP sessions, OpenAPI, and Operations approvals; use the Agent Sandbox for simulated payment and fulfillment.

<a id="developer-tools"></a>

## 🔎 Check Your Implementation

Use a web checker for a quick look at published metadata, or a CLI for repeatable local and CI checks.

- [PAP Checker](https://papchecker.com) - Check Draft 0.1 discovery, OAuth metadata, OpenAPI, and MCP resource metadata in a community web tool; browse per-rule reports and a directory of sites publishing `poppy.json`.
- [poppy-validator](https://github.com/tusharck/poppy-validator) - Validate local files or live Draft 0.1 discovery URLs with an unofficial Python CLI, JSON Schema checks, OAuth metadata cross-checks, and JSON reports for CI.
- [Allowfy Check](https://github.com/allowfy/allowfy-check) - Test live Draft 0.1 discovery, sessions, device sign-in, account tokens, sign-out, and Operations flows with a community CLI and per-check reports.

## 🌐 Explore the Ecosystem

**Follow development** — Track the draft, source changes, and areas still being designed.

- [Official Poppy Repository](https://github.com/personal-agent-protocol/personal-agent-protocol) - Browse the specification and documentation website source, revision history, and issues; this repository does not implement the protocol APIs.
- [Open Topics](https://personalagentprotocol.org/docs/open-topics) - Follow draft gaps, including payments, push notifications, and attachments.

<a id="development-and-design-partners"></a>

**Development and design partners** — [Sierra's launch announcement](https://sierra.ai/blog/introducing-personal-agent-protocol) identifies Meta and Sierra as developing Poppy with industry partners. The [official roster](https://personalagentprotocol.org/docs/path-to-1#partners), checked October 15, 2026, lists partners by role. Participation does not establish a live implementation or a specific code contribution, and this roster does not cover every community contributor.

<details>
<summary>View development and design partners</summary>

| Official group       | Listed partners                                                                                                                                                                                                    |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Personal agents      | Instinct, Meta, OpenAI.                                                                                                                                                                                            |
| Companies            | Bank of America, BBVA, Chime, Cigna, Comcast, DIRECTV, FOX, Gap Inc., GEICO, Hertz, Insurify, Liberty Mutual, Nordstrom, PayPal/Venmo, Rocket, SiriusXM, Synchrony, Target, United Airlines, Walmart, Wells Fargo. |
| Technology providers | 1Password, Adyen, Atomic, Cloudflare, ElevenLabs, Genesys, Klaviyo, Mastercard, NiCE, Notion, Okta, OneSignal, Plaid, Shopify, Sierra, Stripe, Visa, Zapier, Zendesk.                                              |

</details>

<a id="live-company-implementations"></a>

**Live company implementations**: Companies serving a Poppy draft at public endpoints; coverage varies by company.

- [Stacktree](https://stacktr.ee/.well-known/poppy.json) - Publish an HTML page to a private link that opens with no account: signed-out Sessions publish a 24-hour page, and Direct or Device Sign-In (`poppy:read`, `poppy:write`) keeps it on the User's account and shows who opened it; MCP and OpenAPI, plus the Draft 0.2 feedback endpoint. Live since October 11, 2026, on Draft 0.2 since October 19; Mediated Sign-In, conversations, and Operations are not implemented.

<a id="related-protocols"></a>

**Related protocols** — These have their own specifications; inclusion does not imply Poppy compatibility.

- [Model Context Protocol (MCP)](https://modelcontextprotocol.io/docs/getting-started/intro) - Connect AI applications to tools and data; the Poppy draft includes MCP as an API interface companies can offer.
- [Universal Commerce Protocol (UCP)](https://ucp.dev) - Explore commerce flows such as discovery and checkout; Sierra describes UCP as complementary to Poppy's broader agent-to-company interactions.
- [Personal Agent Consent & Trust (PACT)](https://github.com/openpactprotocol/openpactprotocol) - Explore a separate protocol built on A2A and OAuth, with schemas, a client, and a reference stack; it is not Poppy.

## Contributing

Found something useful? Read [CONTRIBUTING.md](CONTRIBUTING.md), then open a pull request or use the resource submission issue template. Small, verified additions and corrections are welcome.
