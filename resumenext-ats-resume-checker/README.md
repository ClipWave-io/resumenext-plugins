# ATS Resume Checker & Resume Builder - ResumeNext

Check a resume's ATS score, see what to fix first, and open it in the ResumeNext resume builder with templates and a live score.

## What it does

Paste or attach a resume and Claude gets a reproducible ATS score out of 100, a letter grade, the score by area and the issues to fix first, computed by fixed rules rather than guessed. Improve the resume in the conversation, score it again, then open the final version in the ResumeNext editor: it arrives already loaded, ready to format with an ATS-safe template and export.

The scores and letters come from fixed rules and templates on ResumeNext's servers: the same input always gives the same result. The plugin does not call an AI model.

## Setup

The plugin connects Claude to the ResumeNext MCP server at `https://resumenext.io/api/claude/resume/mcp` (Streamable HTTP).

- No account or sign-in is needed to use the tools. Opening a link creates a temporary ResumeNext account for the document, so the work is still there when you come back. Editing and previewing in ResumeNext need no payment; downloading the finished file follows the plans at resumenext.io/pricing.
- The tools take plain text: Claude reads an attached file and passes its text. Claude Code works with text and links.

## Tools

| Tool | What it does |
|---|---|
| `analyze_resume` | Deterministic ATS score, grade, score by area and issues to fix first. Read-only, stores nothing. |
| `prepare_resume_editor` | Private link, valid 7 days, that opens the editor with the resume loaded. Stores the resume for the link. |

## Example prompts

- "Check my resume for ATS problems and tell me what to fix first."
- "Rewrite my resume bullets to be more concrete, then score the new version."
- "My resume is ready: open it in the ResumeNext editor."

## Data and privacy

Read-only tools process the text Claude sends and store nothing. The tool that creates a link stores the document you asked to open, for 7 days; opening the link saves it in your ResumeNext account or in a temporary account created for it. The plugin has no hooks or local scripts, calls no AI model, and reads nothing in your conversation beyond the text passed to a tool.

- Privacy policy: https://resumenext.io/privacy
- Terms of service: https://resumenext.io/terms
- Documentation: https://resumenext.io/mcp#resume
- Support: https://resumenext.io/contact

ResumeNext is not affiliated with Anthropic or LinkedIn.
