# Agent Instructions

Use this repository as a portable skill for Arabic bilingual translation and Arabic RTL Word deliverables.

## Canonical Entry

- Load `SKILL.md` first. It is the source of truth for task triggers, workflow, translation rules, output formats, and validation.
- Use `agent-manifest.yaml` only for routing or integration metadata. If it conflicts with `SKILL.md`, follow `SKILL.md`.
- Do not load every reference file by default. Follow the reference routing rules in `SKILL.md`.

## Platform Mapping

- **Codex / Claude / OpenClaw-style skill runners:** register the folder as a skill and use the `SKILL.md` frontmatter `name` and `description` for discovery.
- **Claude Code or other repository-aware coding agents:** read this `AGENTS.md`, then follow `SKILL.md`.
- **GLM, Kimi, or prompt-only agents:** use `SKILL.md` as the system or developer instruction. Attach only the relevant reference files and source documents for the task.
- **Custom orchestrators:** parse `agent-manifest.yaml` for triggers, inputs, outputs, resources, and fallback modes.

## Non-Negotiable Behavior

- Ask for the output format before translating unless the user already specified side-by-side bilingual output, clean translated output, or both.
- Preserve numbering, headings, citations, identifiers, party names, tables, and signature blocks.
- Never silently resolve ambiguity. Translate the most defensible reading and flag the issue in the translator's note.
- Treat OCR or PDF text extraction as draft aid only for Arabic PDFs/images unless visually checked.
- Do not claim to have created or visually validated a Word file when the current environment cannot create or inspect files.

## Minimal Prompt-Only Workflow

When no tools or local files are available:

1. Ask the user for the source text or readable page images.
2. Detect source and target languages.
3. Ask for side-by-side, clean translation, or both.
4. Translate segment by segment while preserving structure and references.
5. Provide a translator's note with ambiguities, source defects, date conversions, and terminology choices.

