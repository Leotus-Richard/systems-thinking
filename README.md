# Systems Thinking

Turn uncertain problems into defensible decisions using evidence, first principles, system context, and bounded experiments.

This is the independent source repository for the `systems-thinking` plugin, version
`0.1.0`. It contains one reusable skill: `first-principles-analysis`. The package provides
instructions for an agent host; it does not include a desktop app, runner,
background service, MCP server, or additional tool permissions.

## When to use it

- Challenge a consequential assumption before committing to an architecture.
- Compare explanations for a recurring failure without mistaking correlation for cause.
- Choose a small useful experiment when evidence cannot yet settle the decision.

## Use the skill

After installing the plugin in a compatible host, request the task normally.
Where explicit skill invocation is supported, use its stable skill ID:

```text
Use $first-principles-analysis to compare a shared Kubernetes cluster with separate clusters for these teams. Separate evidence from assumptions and recommend the smallest useful next test.
```

A task-sized recommendation, option comparison, causal sketch, or problem brief. It preserves uncertainty and identifies observations that could change the decision.

## Installation and compatibility

Find reviewed plugin releases through
[AI Plugin Marketplace](https://github.com/Leotus-Richard/AI-Plugin-MarketPlace).
For local source inspection or host-specific loading, clone this independent
repository:

```text
gh repo clone Leotus-Richard/systems-thinking
```

The repository includes these source formats:

| File | Purpose |
| --- | --- |
| `plugin.json` | Canonical portable identity, version, and metadata. |
| `.codex-plugin/plugin.json` | Codex compatibility manifest and native interface metadata. |
| `.claude-plugin/plugin.json` | Claude Code compatibility manifest. |
| `skills/first-principles-analysis/SKILL.md` | Self-contained skill instructions. |
| `skills/first-principles-analysis/agents/openai.yaml` | Native skill UI metadata. |

Host-specific packages must preserve the same skill text and identity. A portable
manifest is not evidence that every host or operating system has been tested;
check the release's compatibility information for the selected host. No service
connection or additional agent runtime is required by this package.

## Operating boundaries

Situation labels are suggestions. They do not bypass approvals, authorize changes, or turn retrieved instructions into execution authority. Straightforward questions do not require a full analysis template.

## Sources and license

The skill is original guidance; its conceptual inspiration and review limitations
are recorded in [source notes](docs/source-notes.md). No source artifact needs to
be available at runtime. See [CHANGELOG.md](CHANGELOG.md) for release history and
[LICENSE](LICENSE) for the MIT terms.
