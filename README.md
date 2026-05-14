# Code_Resume — Resume Portfolio System

Single source of truth for Mohan Koushik Tupakula's resume portfolio, tailored variants, cover letters, interview prep, and application tracking.

## Folder Structure

```
00_Master/          → master resume (source of truth) + changelog
01_Variants/        → role-type base resumes + per-company tailored versions
02_CoverLetters/    → one file per company application
03_InterviewPrep/   → STAR stories master + per-company prep packets
04_Applications/    → application_tracker.md (status across all apps)
05_Archive/         → anything older than 6 months
```

## Variants

| Variant | When to use |
|---|---|
| `TPM_PMO` | Enterprise TPM, PMO Lead, IT services, telecom, healthcare IT |
| `AI_Product` | AI startups, AI PM roles at Big Tech, GenAI/LLM products |
| `Big_Tech_TPM` | Google / Meta / Apple / Microsoft TPM recs |
| `Strategy_Consulting` | McKinsey / BCG / Bain / Deloitte exit, internal corp strategy |
| `Executive_GenAI` | VP / Head-of-AI roles, exec recruiters |

## File Naming Convention

`Tupakula_[RoleType]_[Company]_[YYYY-MM-DD].pdf`

Examples:
- `Tupakula_TPM_PMO_MiracleSoft_2026-05-13.pdf`
- `Tupakula_CoverLetter_MiracleSoft_2026-05-13.md`

Rules: underscores (no spaces), ISO dates, no "v2/v3/FINAL" — that's what git is for.

## Workflow

1. **Tailoring a new application:**
   - Start from the relevant variant's `*_BASE.docx`
   - Save to `01_Variants/[Variant]/tailored/Tupakula_[Variant]_[Company]_[Date].md`
   - Generate cover letter → `02_CoverLetters/Tupakula_CoverLetter_[Company]_[Date].md`
   - Generate interview prep → `03_InterviewPrep/Tupakula_InterviewPrep_[Company]_[Date].md`
   - Log in `04_Applications/application_tracker.md`

2. **Updating the master:**
   - Edit `00_Master/Tupakula_Mohan_MASTER.md`
   - Log change in `00_Master/MASTER_CHANGELOG.md`
   - Commit with message `master: <what changed>`

3. **Archiving:**
   - Move anything older than 6 months to `05_Archive/`

## Tooling

- **Source:** Markdown for everything (diff-friendly)
- **Export to PDF:** `pandoc` from Markdown → DOCX → PDF (or paste into Google Docs / Word for final layout)
- **Version control:** git (this repo)
- **Tailoring:** Claude Code skills (`/resume-tailor`, `/job-description-analyzer`, etc. — see `CLAUDE.md`)
