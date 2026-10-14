# Skills MCP — give your agent exactly the skills you choose

**[Live site →](https://skillzbench.github.io/skills-mcp/)** · [Get an API key](https://skillzbench.github.io/skills-mcp/get-api-key.html) · [Directory](https://skillzbench.com/skills) · [Leaderboard](https://skillzbench.com/leaderboard)

`mcp.skillzbench.com/mcp` is one Model Context Protocol server for the
[SkillzBench](https://skillzbench.com) catalog — the trusted, benchmarked
directory of agent skills. Connect Claude Code, Cursor, Zed, or any MCP client
with a single `sb_live_` key, then enable skills per agent. Your agent
discovers with `search_skills` / `list_enabled` and loads on demand with
`get_skill` — progressive disclosure keeps context small.

```bash
claude mcp add --transport http skillzbench https://mcp.skillzbench.com/mcp \
  --header "Authorization: Bearer sb_live_YOUR_KEY"
```

## Why this skills MCP

- **Vetted catalog** — every published skill passes static security scanning,
  license classification, two LLM judges, and human review (admin 2FA).
- **Benchmarked** — skills carry measured **Lift**: the pass-rate delta of a
  reference agent with vs. without the skill, with confidence intervals.
- **You stay in control** — agents can only load what you enabled, and
  enabling is ask-by-default with a one-click approval link.
- **Also plain git** — the whole servable catalog is mirrored at
  [SkillzBench/skills](https://github.com/SkillzBench/skills).

## Pages

| Page | What it covers |
|---|---|
| [Skills MCP](https://skillzbench.github.io/skills-mcp/) | What the MCP is, tools, connect snippets |
| [Get an API key](https://skillzbench.github.io/skills-mcp/get-api-key.html) | 3-step key setup + CLI |
| [The platform](https://skillzbench.github.io/skills-mcp/platform.html) | Directory, trust pipeline, benchmarks |

## Repo maintenance

Static HTML, no build step. Pages are served by GitHub Pages from `main`.
Content questions → [skillzbench.com](https://skillzbench.com); security →
team@skillzbench.com.
