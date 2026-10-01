# LinkedIn Profile Review & Resume Converter - ResumeNext

Review the text of a LinkedIn profile section by section and turn it into a resume that opens in the ResumeNext editor.

## What it does

Paste the text of a LinkedIn profile, or the text of LinkedIn's Save to PDF export, and Claude gets a reproducible profile score with findings for headline, About, experience, keywords and completeness, plus the priorities to fix. The same text can be converted into a resume that opens in the ResumeNext editor, ready to format and export. The connector reads the text you supply; it does not connect to LinkedIn. ResumeNext is not affiliated with LinkedIn.

The scores and letters come from fixed rules and templates on ResumeNext's servers: the same input always gives the same result. The plugin does not call an AI model.

## Setup

The plugin connects Claude to the ResumeNext MCP server at `https://resumenext.io/api/claude/linkedin/mcp` (Streamable HTTP).

- No account or sign-in is needed to use the tools. Opening a link creates a temporary ResumeNext account for the document, so the work is still there when you come back. Editing and previewing in ResumeNext need no payment; downloading the finished file follows the plans at resumenext.io/pricing.
- The tools take plain text: Claude reads an attached file and passes its text. Claude Code works with text and links.

## Tools

| Tool | What it does |
|---|---|
| `review_linkedin_profile` | Deterministic profile score with findings by section. Read-only, stores nothing. |
| `convert_linkedin_to_resume` | Private link, valid 7 days, that opens the editor with the profile as a resume. Stores the profile text for the link. |

## Example prompts

- "Here is my LinkedIn profile text. Score it and tell me what to improve for a Data Analyst role."
- "Rewrite my headline and About section, then review the profile again."
- "Turn my LinkedIn profile into a resume and open it in the editor."

## Data and privacy

Read-only tools process the text Claude sends and store nothing. The tool that creates a link stores the document you asked to open, for 7 days; opening the link saves it in your ResumeNext account or in a temporary account created for it. The plugin has no hooks or local scripts, calls no AI model, and reads nothing in your conversation beyond the text passed to a tool.

- Privacy policy: https://resumenext.io/privacy
- Terms of service: https://resumenext.io/terms
- Documentation: https://resumenext.io/mcp#linkedin
- Support: https://resumenext.io/contact

ResumeNext is not affiliated with Anthropic or LinkedIn.
