# Resignation Letter Generator - ResumeNext

Write a resignation letter in a standard, formal or grateful style and open it in ResumeNext to edit and save as PDF, DOCX or TXT.

## What it does

Tell Claude where you work, your last day and, if you like, your role and your manager's name. The connector returns a complete resignation letter in one of three styles (standard, formal for HR files, grateful for a team you want to stay in touch with) from a fixed template, so the same details always give the same letter. A link opens the letter in ResumeNext, where you can edit it and save it as PDF, DOCX or TXT. Your details travel in the link's fragment, which is not sent to the server.

The scores and letters come from fixed rules and templates on ResumeNext's servers: the same input always gives the same result. The plugin does not call an AI model.

## Setup

The plugin connects Claude to the ResumeNext MCP server at `https://resumenext.io/api/claude/resignation-letter/mcp` (Streamable HTTP).

- No account or sign-in is needed, in Claude or on ResumeNext. Downloads carry a ResumeNext watermark unless you are on a paid plan (resumenext.io/pricing).
- The tools take plain text: Claude reads an attached file and passes its text. Claude Code works with text and links.

## Tools

| Tool | What it does |
|---|---|
| `write_resignation_letter` | Complete letter in the chosen style plus a link to edit and save it. Template-based. Read-only, stores nothing. |

## Example prompts

- "Write a formal resignation letter: I am a Senior Designer at Acme Studio, my last day is March 14, 2026."
- "Make it warmer: my manager is Jane Doe and I want to stay in touch."
- "Give me the standard version and the link to download it."

## Data and privacy

The tools process the text Claude sends and store nothing. The plugin has no hooks or local scripts, calls no AI model, and reads nothing in your conversation beyond the text passed to a tool.

- Privacy policy: https://resumenext.io/privacy
- Terms of service: https://resumenext.io/terms
- Documentation: https://resumenext.io/mcp#resignation-letter
- Support: https://resumenext.io/contact

ResumeNext is not affiliated with Anthropic or LinkedIn.
