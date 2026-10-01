# Resume Examples & Templates - ResumeNext

Browse resume examples by role and resume templates, each with a link that opens it in the ResumeNext editor as a starting point.

## What it does

Ask Claude for a resume example for a role and it gets complete examples from ResumeNext's library, with headline, summary, experience bullets and skills, a link to the example's page and a link that opens it in the editor to adapt. It can also list ResumeNext's resume templates, say which are ATS-safe and which are visual, who each suits, and open a new resume in the one you pick. Every person and company in the examples is fictional.

The scores and letters come from fixed rules and templates on ResumeNext's servers: the same input always gives the same result. The plugin does not call an AI model.

## Setup

The plugin connects Claude to the ResumeNext MCP server at `https://resumenext.io/api/claude/resume-examples/mcp` (Streamable HTTP).

- No account or sign-in is needed to use the tools or to open an example or a template in the editor. Editing and previewing in ResumeNext need no payment; downloading the finished file follows the plans at resumenext.io/pricing.
- The tools take plain text: Claude reads an attached file and passes its text. Claude Code works with text and links.

## Tools

| Tool | What it does |
|---|---|
| `find_resume_examples` | Up to three complete examples for a role, with links to the page and the editor. Read-only. |
| `list_resume_templates` | Templates with layout type, description and audience, each with an editor link. Read-only. |

## Example prompts

- "Show me a resume example for a software engineer."
- "Which ResumeNext templates suit a student?"
- "Open the Classic template in the editor."

## Data and privacy

The tools process the text Claude sends and store nothing. The plugin has no hooks or local scripts, calls no AI model, and reads nothing in your conversation beyond the text passed to a tool.

- Privacy policy: https://resumenext.io/privacy
- Terms of service: https://resumenext.io/terms
- Documentation: https://resumenext.io/mcp#resume-examples
- Support: https://resumenext.io/contact

ResumeNext is not affiliated with Anthropic or LinkedIn.
