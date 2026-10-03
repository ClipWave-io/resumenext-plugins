# Resume Skills & Keywords by Role - ResumeNext

Get the skills and terms that recur for a role and see where a resume uses them: listed and shown, listed only, shown only, or not mentioned.

## What it does

Ask Claude which skills a role calls for and it gets the vocabulary of ResumeNext's role guides: the tools, methods, certifications and domain terms that recur for that role, with a link to the role's example resume that uses them. Paste a resume with the target role and Claude gets every term sorted by where the resume uses it: listed in the Skills section and shown in a role or project, listed but not shown anywhere in the work, shown in the work but not listed, or not mentioned, with the number of skills the Skills section lists. The vocabulary is a list to check a resume against, not one to copy: list the terms you would accept an interview question on, and let a bullet show where you used each one. The guide covers the 20 roles of the ResumeNext examples library.

The results come from fixed rules and ResumeNext's own guides on ResumeNext's servers: the same input always gives the same result. The plugin does not call an AI model.

## Setup

The plugin connects Claude to the ResumeNext MCP server at `https://resumenext.io/api/claude/resume-skills/mcp` (Streamable HTTP).

- No account or sign-in is needed to use the tools.
- The tools take plain text: Claude reads an attached file and passes its text. Claude Code works with text and links.

## Tools

| Tool | What it does |
|---|---|
| `find_resume_skills` | The skills vocabulary of a role, with a link to its example resume. Read-only. |
| `check_resume_skills` | The role's terms sorted by where a resume uses them, and the size of its Skills section. Read-only. |

## Example prompts

- "Which skills should a data analyst resume show?"
- "Here is my resume for a registered nurse role. Which of the usual skills do I list without showing where I used them?"
- "Check the skills on my software engineer resume."

## Data and privacy

The tools process the text Claude sends and store nothing. The plugin has no hooks or local scripts, calls no AI model, and reads nothing in your conversation beyond the text passed to a tool.

- Privacy policy: https://resumenext.io/privacy
- Terms of service: https://resumenext.io/terms
- Documentation: https://resumenext.io/mcp#resume-skills
- Support: https://resumenext.io/contact

ResumeNext is not affiliated with Anthropic.
