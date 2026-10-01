# Job Match & Resume Keyword Scanner - ResumeNext

Compare a resume with a job description: matched and missing keywords, coverage, and a job-tailored ATS score.

## What it does

Give Claude a resume and a job posting and it gets the posting's keywords that the resume covers and the ones it misses, with how often each appears on both sides, the coverage percentage and an ATS score for that specific job. Tailor the resume in the conversation without inventing anything, match it again, then open the tailored version in the ResumeNext editor with the job attached as its target.

The scores and letters come from fixed rules and templates on ResumeNext's servers: the same input always gives the same result. The plugin does not call an AI model.

## Setup

The plugin connects Claude to the ResumeNext MCP server at `https://resumenext.io/api/claude/job-match/mcp` (Streamable HTTP).

- No account or sign-in is needed to use the tools. Opening a link creates a temporary ResumeNext account for the document, so the work is still there when you come back. Editing and previewing in ResumeNext need no payment; downloading the finished file follows the plans at resumenext.io/pricing.
- The tools take plain text: Claude reads an attached file and passes its text. Claude Code works with text and links.

## Tools

| Tool | What it does |
|---|---|
| `match_resume_to_job` | Keywords found and missing, counts on both sides, coverage and job-tailored ATS score. Read-only, stores nothing. |
| `prepare_tailored_resume` | Private link, valid 7 days, that opens the editor with the resume and its target job. Stores both for the link. |

## Example prompts

- "Here is my resume and a job posting. Which keywords am I missing?"
- "Tailor my resume to this job description without inventing anything, then match it again."
- "Open the tailored resume in the ResumeNext editor with this job attached."

## Data and privacy

Read-only tools process the text Claude sends and store nothing. The tool that creates a link stores the document you asked to open, for 7 days; opening the link saves it in your ResumeNext account or in a temporary account created for it. The plugin has no hooks or local scripts, calls no AI model, and reads nothing in your conversation beyond the text passed to a tool.

- Privacy policy: https://resumenext.io/privacy
- Terms of service: https://resumenext.io/terms
- Documentation: https://resumenext.io/mcp#job-match
- Support: https://resumenext.io/contact

ResumeNext is not affiliated with Anthropic or LinkedIn.
