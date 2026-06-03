---
name: cs-daily-job-leads
description: Find, verify, dedupe, score, and summarize daily job leads matching a user's target roles, companies, locations, and preferences.
---
# Daily Job Leads
## Goal
Find high-quality job leads for the user on a recurring basis. Prioritize verified, recent, relevant postings with direct source links and clear next actions.
## Inputs
Ask for or use configured values for:
- Target job titles or role families
- Preferred companies or industries
- Location and remote preferences
- Seniority level
- Compensation requirements, if available
- Excluded companies, roles, locations, or contract types
- Existing lead tracker or prior results for deduplication
## Workflow
1. Search official company career pages, reputable job boards, and relevant industry sources.
2. Prefer direct employer postings over reposts.
3. Verify each lead has an active source URL.
4. Remove duplicates and previously reported leads.
5. Score each lead based on role fit, company fit, location fit, recency, and application quality.
6. Return only strong matches unless asked for a broader sweep.
## Output Format
Return a table with:
- Company
- Role
- Location/Remote
- Posted date, if available
- Source link
- Fit score
- Why it matches
- Recommended next action
## Quality Rules
- Do not include stale, closed, or unverifiable postings.
- Do not hallucinate salary, visa, or remote details.
- Mark unknown fields clearly as `Unknown`.
- Prefer fewer, better leads over noisy volume.
- Include source links for every lead.
