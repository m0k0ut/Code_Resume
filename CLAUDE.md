# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

This is a resume/career development workspace. Use the `paramchoudhary/resumeskills` skill suite for all resume and job application work.

## Resume Format Standard

All resumes in this project are written in **Markdown** and built using [junian/markdown-resume](https://github.com/junian/markdown-resume) — an ATS-friendly and human-readable resume tool.

### Conventions
- Source files live in `01_Variants/` and `00_Master/` as `.md` files
- Use `markdown-resume` to generate PDF/HTML output from `.md` source files
- When creating or editing resume content, write valid Markdown compatible with the `junian/markdown-resume` schema
- Prefer semantic Markdown sections: `# Name`, `## Experience`, `## Education`, `## Skills`, etc.
- Do not use raw HTML or non-standard Markdown extensions in resume `.md` files

## Directory Structure

| Folder | Purpose |
|--------|---------|
| `00_Master/` | Master resume source + changelog |
| `01_Variants/` | Role-specific variants (AI_Product, TPM_PMO, Big_Tech_TPM, etc.) |
| `02_CoverLetters/` | Cover letters keyed to applications |
| `03_InterviewPrep/` | STAR stories and interview prep docs |
| `04_Applications/` | `application_tracker.md` — tracks pipeline status |
| `05_Archive/` | Old/unused versions |

## File Naming Convention

`Tupakula_<Variant>_<Company>_<YYYY-MM-DD>.md`
Example: `Tupakula_TPM_PMO_MiracleSoft_2026-05-13.md`

## markdown-resume Usage

`junian/markdown-resume` is a **browser-based web app** (fork of Oh My CV!), not a CLI tool.

**To generate PDF/HTML/DOCX from a `.md` resume:**
1. Open https://www.junian.dev/markdown-resume/ in Chrome or Edge
2. Paste the `.md` source content into the editor
3. Use the in-app **Export** menu to save as PDF (A4 / US Letter), HTML, or DOCX

Data is stored locally in the browser — no server upload, no tracking.

## Available Resume Skills

| Task | Skill command |
|---|---|
| Tailor resume to a job posting | `/resume-tailor` |
| Optimize for ATS systems | `/resume-ats-optimizer` |
| Improve bullet points | `/resume-bullet-writer` |
| Add metrics and quantify impact | `/resume-quantifier` |
| Fix formatting and layout | `/resume-formatter` |
| Build or rewrite a section | `/resume-section-builder` |
| Optimize for tech/engineering roles | `/tech-resume-optimizer` |
| Write for executive-level roles | `/executive-resume-writer` |
| Write a cover letter | `/cover-letter-generator` |
| Optimize LinkedIn profile | `/linkedin-profile-optimizer` |
| Analyze a job description | `/job-description-analyzer` |
| Generate interview prep materials | `/interview-prep-generator` |
| Compare job offers | `/offer-comparison-analyzer` |
| Prepare salary negotiation | `/salary-negotiation-prep` |
| Translate skills across industries | `/career-changer-translator` |
| Build an academic CV | `/academic-cv-builder` |
| Design a creative portfolio resume | `/creative-portfolio-resume` |
| Write portfolio case studies | `/portfolio-case-study-writer` |
| Build a reference list | `/reference-list-builder` |
| Manage multiple resume versions | `/resume-version-manager` |
