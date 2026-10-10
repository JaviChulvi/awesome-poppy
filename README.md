<!--lint disable awesome-github-->
<!-- GitHub metadata is reviewed separately from list content. -->

# Awesome Poppy — Personal Agent Protocol [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

Poppy, the **Personal Agent Protocol (PAP)**, is a draft open protocol for personal AI agents to discover companies, obtain user-authorized access, and work through websites, APIs, or company agents.

This is an **unofficial community list**, unaffiliated with Sierra or Meta. The Awesome badge identifies the list format; it does not imply endorsement or inclusion in the upstream Awesome index.

**Current specification:** Draft 0.1, updated October 9, 2026; checked October 10, 2026. It may change incompatibly before a stable release. Design partners are not automatically live implementations.

## Contents

- [Official Resources](#official-resources)
- [Introductions](#introductions)
- [Developer Guides](#developer-guides)
- [Community SDKs and Integrations](#community-sdks-and-integrations)
- [Community Demos](#community-demos)
- [Related Protocols](#related-protocols)

## Official Resources

- [Personal Agent Protocol](https://personalagentprotocol.org) - Official home, with interactive walkthroughs using fictional companies.
- [Protocol Overview](https://personalagentprotocol.org/docs/overview) - Explains the goals, access controls, and design principles.
- [Specification](https://personalagentprotocol.org/docs/spec) - Authoritative Draft 0.1 covering discovery, sessions, authorization, web browsing, APIs, and conversations.
- [Open Topics](https://personalagentprotocol.org/docs/open-topics) - Tracks areas the draft does not yet cover, including payments, push notifications, and attachments.

## Introductions

- [Sharing a Draft of Personal Agent Protocol](https://sierra.ai/blog/poppy) - Sierra's explanation of the draft, including a report of the Rocket mortgage demo with Meta's Muse; the reference implementation is announced as forthcoming.

## Developer Guides

These are official documents for the draft, not evidence of deployed features.

- [Implementation Guides](https://personalagentprotocol.org/docs/guides) - Recommended practices for personal agents and companies, including secrets, metadata fetching, retries, and token handling.
- [Extensions](https://personalagentprotocol.org/docs/extensions) - Explains how optional extensions are advertised and versioned separately from the core protocol.
- [Operations Extension](https://personalagentprotocol.org/docs/extensions/operations) - Optional version 1 extension for proposing, approving, confirming, and tracking actions across channels; part of the draft.

## Community SDKs and Integrations

- [Datalayer Personal Agent Protocol SDKs](https://github.com/datalayer/personal-agent-protocol) - Community Python and TypeScript SDKs targeting Draft 0.1, with discovery, protocol models, and signed-out session flows; conversations, full sign-in flows, and Operations execution are not yet implemented.
- [pi-poppy](https://github.com/richardanaya/pi-poppy) - Community Draft 0.1 extension for the Pi coding agent, with sessions, conversations, API and MCP access, operation approvals, and local examples; its default client metadata is served locally and cannot be fetched by remote companies.

## Community Demos

- [Poppy on Cloudflare Workers](https://github.com/irvinebroque/poppy-demo) - Community two-Worker demo of discovery, direct sign-in, conversations, and a simulated jacket exchange; uses a synthetic account and is not a full conformance suite.

## Related Protocols

These have their own specifications; listing them does not imply PAP compatibility.

- [Model Context Protocol (MCP)](https://modelcontextprotocol.io/docs/getting-started/intro) - Connects AI applications to tools and data; the PAP draft includes MCP as an API interface a company can offer.
- [Universal Commerce Protocol (UCP)](https://ucp.dev) - Defines commerce flows such as discovery and checkout; Sierra describes it as complementary to PAP's broader agent-to-company interactions.
- [Personal Agent Consent & Trust (PACT)](https://github.com/openpactprotocol/openpactprotocol) - Separate protocol built on A2A and OAuth, with schemas, a client, and a reference stack; it is not PAP or Poppy.

## Contributing

Found a useful resource? Read [CONTRIBUTING.md](CONTRIBUTING.md), then open a pull request or use the resource submission issue template. Small, verified additions are welcome.
