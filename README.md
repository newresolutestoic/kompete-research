# Kompete Research

Central repository for customer research, interviews, and synthesized insights for Kompete.ai.

This repo is included as a **git submodule** in:
- `backend-mark3/research/`
- `frontend-mark3/research/`
- `rohith-m5/research/`
- `kompete-website/research/`

## Structure

```
interviews/          # Raw customer/prospect interview notes
  001-company-YYYY-MM-DD.md
  002-company-YYYY-MM-DD.md
  ...

synthesis/           # Analyzed and synthesized outputs
  pain-points.md     # Extracted pain points across all interviews
  personas.md        # Customer personas derived from interviews
  key-themes.md      # Recurring themes and patterns
```

## How to Use

### Adding a new interview
1. Create a new file in `interviews/` following the naming convention: `NNN-company-YYYY-MM-DD.md`
2. Use the interview template below
3. After adding, update `synthesis/` files with any new insights

### Interview template
```markdown
# Interview NNN — [Company Name]
**Date:** YYYY-MM-DD
**Interviewer:** [Name]
**Interviewee:** [Name, Title]
**Company:** [Company, Industry, Size]

## Context
[Why this interview, what stage of relationship]

## Key Quotes
- "..."

## Pain Points Identified
1. ...

## Current Workflow / Tools
- ...

## Willingness to Pay / Budget Signals
- ...

## Feature Requests / Wishes
- ...

## Follow-up Actions
- [ ] ...
```

### Updating across repos
After pushing changes here, run in each consuming repo:
```bash
git submodule update --remote research
git add research
git commit -m "Update research submodule"
```

## 28 Interviews
Place your 28 existing interview files in `interviews/`. Supported formats: `.md`, `.txt`, `.pdf`, `.docx`
