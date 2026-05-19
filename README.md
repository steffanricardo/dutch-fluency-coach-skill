# Dutch Fluency Coach Skill

A Claude Skill that turns the Dutch Fluency MCP server into a friendly,
structured Dutch-learning coach — CEFR placement, sentence correction,
inburgering practice, and verifiable certificates.

**MCP server:** `https://mcp.dutchfluency.com/mcp` (streamable HTTP, no auth required)

## Install

In Claude Code (or any client with skill support), drop the folder into your
skills directory:

```bash
git clone https://github.com/steffanricardo/dutch-fluency-coach-skill.git
cp -R dutch-fluency-coach-skill/dutch-fluency-coach ~/.claude/skills/
```

Then add the MCP server once via Claude Desktop → Settings → Connectors →
Add custom connector → paste the URL above.

## Try it

Once the MCP server is connected and the skill is installed, try one of these:

> "Run the Dutch CEFR placement test for me. I'm intermediate, learning for work."

> "Check this Dutch sentence: *Ik heb gisteren naar de winkel gegaan.*"

> "Give me a random KNM question from chapter 1, then check my answer."

> "Verify this Dutch Fluency certificate: `https://www.dutchfluency.com/cert/<hash>`"

The skill guides Claude through each workflow one step at a time, with safety
guardrails (e.g. placement results are framed as Dutch Fluency estimates, not
official exam scores).

## What's in here

- [`dutch-fluency-coach/SKILL.md`](dutch-fluency-coach/SKILL.md) — the skill
  itself: workflows, tone, and guardrails Claude follows when using the MCP
  tools.

This Skill does not replace the MCP server and does not include private
curriculum data. It only teaches Claude a simple public workflow for using the
16 publicly available Dutch Fluency tools.

## License

MIT — see [LICENSE](LICENSE).
