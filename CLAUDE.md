# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repository Is

A collection of 15 Claude skill files for generating production-quality video prompts for **Seedance 2.0 on Higgsfield** (`https://higgsfield.ai/create/video?model=seedance_2_0`). There is no build system, test suite, or application code — the deliverable is Markdown content.

## Repository Structure

```
skills/
  XX-name/
    SKILL.md          # English version
    zh-CN/SKILL.md    # Simplified Chinese version
references/           # User-supplied reference images/media
assets/               # Banner and skill-map SVGs
```

## Seedance 2.0 on Higgsfield — Key Technical Constraints

Every skill must accurately document these platform specs:
- **Images:** ≤ 9 files, each < 30 MB (jpeg, png, webp, bmp, tiff, gif)
- **Videos:** ≤ 3 files, each < 50 MB, 2–15s total (mp4, mov)
- **Audio:** ≤ 3 files, each < 15 MB, ≤ 15s total (mp3, wav)
- **Combined maximum:** 12 files total
- **Output:** 4–15s, 720p video with sound
- **Reference syntax inside prompts:** `@image1`, `@video1`, `@audio1`

## SKILL.md File Format

Each skill file must follow this structure:

### YAML Frontmatter
```yaml
---
name: seedance-[skill-name]
description: [Trigger keywords + use cases. Must include "Seedance 2.0 on Higgsfield".]
---
```

The `description` field is critical — it controls when Claude auto-activates the skill. It should list all natural-language triggers a user might say.

### Required Sections (in order)

1. **Technical Specs** — Seedance 2.0 on Higgsfield input/output specs
2. **2-Second Hook Framework** — 10+ attention-grabbing opener patterns with prompt phrasing templates
3. **Prompt Philosophy** — Deep theory specific to this use case
4. **Master Template** — Reusable prompt structure for the skill's genre
5. **Camera Movement Encyclopedia** — 15+ techniques with exact prompt phrasing
6. **Lighting & Atmosphere** — 10+ setups
7. **Sound Design** — Ambient, foley, music, silence guidance
8. **5+ Large Example Prompts** — 15–25 lines each, production-ready (no generic placeholders)
9. **Common Mistakes** — 10+ pitfalls with fixes
10. **Platform Optimization** — TikTok/Douyin, Instagram, YouTube adjustments
11. **Output Instructions** — How the skill generates prompts for the user

## Quality Rules

- Target 400+ lines per skill file
- Every mention of Seedance 2.0 must be paired with "on Higgsfield" (e.g., "Seedance 2.0 on Higgsfield")
- Examples must be production-ready and genre-specific, not generic
- Both English and zh-CN versions are required for every skill
- The `references/` folder holds user-supplied media for prompt generation sessions

## Adding or Modifying Skills

When creating a new skill, use an existing skill (e.g., `skills/01-cinematic/SKILL.md`) as a structural template. The skill number prefix (01–15+) determines sort order in the README table. Update `README.md` (and all language variants) when adding a new skill entry.

Commit message format:
```
feat: add [skill-name] skill
fix: correct camera keywords in [skill-name]
docs: update README translations
```
