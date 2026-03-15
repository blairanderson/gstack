# gstack Marketplace

A community-maintained [Claude Code](https://docs.anthropic.com/en/docs/claude-code) marketplace packaging of [Garry Tan's gstack skills](https://github.com/garrytan/gstack).

Garry's repo contains the skills but not a marketplace directory. This repo adds the marketplace config so you can install them with one command.

## Quick Start

### 1. Add the marketplace

```shell
/plugin marketplace add blairanderson/gstack
```

### 2. Install all skills

```shell
/plugin install @gstack-mp
```

Or install a single skill:

```shell
/plugin install @gstack-mp/review
```

## Available Skills

| Skill | Category | Description |
|-------|----------|-------------|
| `plan-ceo-review` | Planning | CEO/founder-mode plan review — rethink the problem, challenge premises, find the 10-star product |
| `plan-eng-review` | Planning | Eng manager-mode plan review — lock in architecture, data flow, edge cases, and test coverage |
| `review` | Code Review | Pre-landing PR review for SQL safety, LLM trust boundary violations, and structural issues |
| `ship` | Deployment | Ship workflow — merge main, run tests, review diff, bump version, create PR |

## Upstream Tracking

A GitHub Actions workflow runs weekly to check for new commits in the upstream [garrytan/gstack](https://github.com/garrytan/gstack) repo and opens a PR to bump the SHA.

## License

MIT
