# Resume Bullet Point Checker & Action Verbs - ResumeNext

Check resume bullet points line by line for action verbs, numbers, pronouns and phrases to delete, and get action verbs by type of work.

## What it does

Paste the bullet points of a resume and Claude gets a verdict for every line, from fixed rules: whether it opens with an action verb, opens with a gerund or with a phrase to delete (Responsible for, Worked on, Helped with, Assisted with, Duties included), carries a number, a percentage or an amount, or slips into the first person, and what to change first. It also gets the totals, whether at least a third of the lines carry a number, and the lines to rewrite first. Ask for action verbs and it gets the verb groups of ResumeNext's action verb guide by type of work (leadership, building, process improvement, analysis, finance, communication, sales, teaching, care), each with its usage note, plus the phrases to delete and the rules for picking a verb without inflating it. Rewrite in the conversation, then check the new lines again.

The results come from fixed rules and ResumeNext's own guides on ResumeNext's servers: the same input always gives the same result. The plugin does not call an AI model.

## Setup

The plugin connects Claude to the ResumeNext MCP server at `https://resumenext.io/api/claude/bullet-points/mcp` (Streamable HTTP).

- No account or sign-in is needed to use the tools.
- The tools take plain text: Claude reads an attached file and passes its text. Claude Code works with text and links.

## Tools

| Tool | What it does |
|---|---|
| `check_resume_bullets` | A verdict for each line, the totals and the lines to rewrite first. Read-only. |
| `find_action_verbs` | Action verbs for a type of work, with the usage note, the phrases to delete and the rules. Read-only. |

## Example prompts

- "Check these bullet points from my resume and tell me which to rewrite first."
- "Give me action verbs for sales work, then rewrite my bullets with them and check them again."
- "Which phrases should I delete from my resume bullets?"

## Data and privacy

The tools process the text Claude sends and store nothing. The plugin has no hooks or local scripts, calls no AI model, and reads nothing in your conversation beyond the text passed to a tool.

- Privacy policy: https://resumenext.io/privacy
- Terms of service: https://resumenext.io/terms
- Documentation: https://resumenext.io/mcp#bullet-points
- Support: https://resumenext.io/contact

ResumeNext is not affiliated with Anthropic.
