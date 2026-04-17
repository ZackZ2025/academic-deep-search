# Academic Deep Search

`academic-deep-search` is an AI agent skill for literature review tasks where the goal is not just to find papers, but to extract structured, source-grounded answers that are immediately useful.

It is designed for requests such as:

- What markers or molecules do studies in a topic usually measure?
- What methods are commonly used in this field?
- What do Results sections usually report?
- What does a representative figure in this topic look like?

## What This Skill Does

- distinguishes between method/marker questions and figure-oriented questions
- respects user-specified journal, database, or URL scope
- prefers PubMed and PMC for biomedical topics
- emphasizes full-text reading over abstract-only summaries
- organizes output by experiment type or by representative figure

## Repository Structure

- `SKILL.md`: core AI-facing workflow
- `agents/openai.yaml`: optional Codex/OpenAI-style interface metadata
- `references/query-guide.md`: query-building tips and answer templates

## Notes

- This skill is especially useful for biomedical literature review.
- It is designed to reduce shallow citation dumping and encourage source verification.
- Full-text evidence is preferred whenever available.

## Current Release Focus

The latest local revision simplifies the main skill instructions, separates detailed query guidance into a reference file, and makes source-scope rules clearer.
