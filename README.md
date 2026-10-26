# demo-lesson1

Material for the four live demos in Lesson 1 of *Agentic AI for Economic
Research*. Clone it and follow along:

```
git clone https://github.com/MarcoLeMoglie/demo-lesson1
cd demo-lesson1
```

`code/analysis.do` contains a deliberate bug. Do not fix it before the lesson.

| Demo | What we do | What to watch |
|------|------------|---------------|
| Chat vs agent | Paste the do-file into a chat window and ask for the bug. Then give the same request to an agent in this folder. | The chat guesses; the agent runs Stata, reads `analysis.log`, edits, reruns. |
| Context and compaction | Long session, then `/compact` in Codex. | The context meter before and after; what the summary keeps. |
| MCP and skills | Ask for "a regression table" with the skill in `.agents/skills/` available. | The agent loads `SKILL.md` only when the request matches. |
| Model swap | Same task in OpenCode, first with a closed model, then with an open-weight model via OpenRouter. | Same harness, same tools, different model: speed, cost, result. |

## Requirements

Stata 17 or later with `esttab` (`ssc install estout`). One of: Codex CLI,
Claude Code, Cursor, OpenCode.
