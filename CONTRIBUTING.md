# Contributing

Help keep this list small, accurate, and useful. Suggest a resource through a pull request or the resource submission issue template.

## Inclusion Criteria

- Directly relevant to Poppy / Personal Agent Protocol, or useful as a clearly labeled related protocol.
- Publicly accessible at a working, canonical URL, with enough documentation to understand its value.
- Offers something useful beyond repeating an announcement. Prefer primary sources and maintained repositories with clear licenses.
- Claims are supported by the linked content or inspectable code. State whether the resource is official, community-built, a demo, or a proposal.
- Descriptions reflect the current specification. Name the draft or version when claiming implementation support; do not imply full compatibility from a project's name or README alone.

Do not submit unrelated projects named Poppy or PAP, duplicates, affiliate links, generic AI directories, speculative projects without substantive content, or lists of design partners presented as live implementations. Keep PACT separate from PAP. Open topics and proposed extensions must not be described as implemented features.

## Entry Format

Use one bullet with a name, canonical HTTPS URL, and short factual description. For example:

```markdown
- [Protocol Overview](https://personalagentprotocol.org/docs/overview) - Explains the goals, access controls, and design principles.
```

Start the description with a capital letter and end with a period. Explain what readers can learn or use; avoid marketing language, star counts, and claims such as "best" or "production-ready" without evidence.

## Submitting a Change

1. Search the README and open issues/pull requests for duplicates.
2. Open the resource and inspect its contents. For code, check the source, documentation, and maintenance status.
3. Add the entry at the end of the most relevant category. Create a category only when verified resources justify it, and update Contents when headings change.
4. Explain why the resource belongs and link to evidence supporting the description. Disclose your connection to the resource, if any.
5. Check formatting, anchors, and links. Keep the change focused and respond to review feedback.

Corrections and removals are welcome. Explain what changed and provide a source. A bot-blocked or rate-limited response is a reason to investigate, not proof that a resource is gone.

## Checks

GitHub Actions runs Markdown linting, Awesome conventions, and link checks. To run the same checks locally with Node.js 22+ and Lychee 0.24.2 installed:

```sh
npx --yes markdownlint-cli2@0.23.3 README.md CONTRIBUTING.md .github/pull_request_template.md
npx --yes awesome-lint@2.3.0 README.md
lychee --no-progress --include-fragments --max-retries 3 --timeout 20 README.md CONTRIBUTING.md .github/pull_request_template.md
```

The README disables the GitHub metadata check (description, topics, and license detection on the default branch) for the initial PR. Content conventions remain enabled. Review those settings separately after merging and remove the exception once they are configured. Passing checks does not indicate acceptance by the Awesome index. Review HTTP 403/429 and timeout reports manually before treating them as broken links.

Contributions are published under this repository's [CC0 license](LICENSE). Linked resources retain their own licenses.
