# Cover Letter Checker & Builder - ResumeNext

Check a cover letter against a fixed checklist, read example letters by role, and open the final letter in the ResumeNext cover letter editor.

## What it does

Write a cover letter with Claude and have it reviewed by a fixed checklist: length, opening line, company and role named, quantified results, leftover placeholders, filler phrases, closing call to action, match with the resume and the job's keywords. Each check says whether it passes and how to fix it. Ask for example letters for a role from ResumeNext's library, then open the finished letter in the ResumeNext cover letter editor to format and export it.

The scores and letters come from fixed rules and templates on ResumeNext's servers: the same input always gives the same result. The plugin does not call an AI model.

## Setup

The plugin connects Claude to the ResumeNext MCP server at `https://resumenext.io/api/claude/cover-letter/mcp` (Streamable HTTP).

- No account or sign-in is needed to use the tools. Opening a link creates a temporary ResumeNext account for the document, so the work is still there when you come back. Editing and previewing in ResumeNext need no payment; downloading the finished file follows the plans at resumenext.io/pricing.
- The tools take plain text: Claude reads an attached file and passes its text. Claude Code works with text and links.

## Tools

| Tool | What it does |
|---|---|
| `score_cover_letter` | Deterministic score out of 100 with each check passed or failed and how to fix it. Read-only, stores nothing. |
| `find_cover_letter_examples` | Complete example letters for a role, with writing tips and links. Read-only. |
| `prepare_cover_letter_editor` | Private link, valid 7 days, that opens the cover letter editor with the letter loaded. Stores the letter for the link. |

## Example prompts

- "Check this cover letter for the Product Manager role at Acme and tell me what to fix."
- "Show me a cover letter example for a registered nurse."
- "The letter is final: open it in the ResumeNext editor."

## Data and privacy

Read-only tools process the text Claude sends and store nothing. The tool that creates a link stores the document you asked to open, for 7 days; opening the link saves it in your ResumeNext account or in a temporary account created for it. The plugin has no hooks or local scripts, calls no AI model, and reads nothing in your conversation beyond the text passed to a tool.

- Privacy policy: https://resumenext.io/privacy
- Terms of service: https://resumenext.io/terms
- Documentation: https://resumenext.io/mcp#cover-letter
- Support: https://resumenext.io/contact

ResumeNext is not affiliated with Anthropic or LinkedIn.
