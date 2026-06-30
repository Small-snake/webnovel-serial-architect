---
name: webnovel-serial-architect
description: Help users build Chinese webnovel long-form serial fiction systems, including inspiration banks, market positioning, submission outlines, opening chapter plans, prose drafting, snowflake-style expansion, rolling outlines, character state tracking, foreshadowing logs, timelines, chapter breakdowns, and writer's block diagnosis. Use when the user wants to write, plan, pitch, continue, revise, or unblock a long webnovel, especially for 网文, 小说设定, 投稿大纲, 开篇, 第一章, 前十章, 滚动大纲, 卡文, 爽点, 伏笔, 人物卡, 双世界, 梦境, 精神病院, or an outline that can start small and evolve after writing begins.
---

# Webnovel Serial Architect

## Operating Principle

Help the user make the next useful creative decision for a long serialized webnovel.

Do not require a complete full-book outline before writing starts. Prefer a minimum viable plan that can support a strong opening, then update the outline as chapters, characters, hooks, and reader expectations evolve.

Always preserve the user's premise, tone, and ownership. When content is missing, name the gap and offer 2-3 usable directions instead of silently inventing everything.

## First Triage

Classify the user's current state before producing output:

1. **Inspiration capture**: They have fragments, images, tropes, character ideas, settings, scenes, phrases, or market observations.
2. **Market positioning**: They need genre, target reader, promise, core emotional payoff, or long-form viability.
3. **Submission outline**: They need a pitch-ready outline for editors, platforms, or self-evaluation.
4. **Opening / prose execution**: They want to plan or draft the first chapter, first three chapters, first ten chapters, scene prose, or revision variants.
5. **Rolling outline**: They have already written chapters and need continuation, repair, or expansion.
6. **Block diagnosis**: They are stuck, doubting the premise, or unable to move from outline to prose.

Ask at most one clarifying question when the next step is blocked. Otherwise, choose the most likely mode and proceed.

## Workspace Intake

When working inside an existing fiction project, inspect the workspace before proposing major story decisions or writing durable artifacts:

1. Run `rg --files` to find existing drafts, notes, outlines, character cards, timelines, and worldbuilding files.
2. Read only the files that appear relevant to the user's current request.
3. Treat existing drafts and confirmed notes as canon unless the user asks for a rebuild.
4. Separate discovered facts into confirmed, tentative, and unclear before extending the story.

Skip workspace scanning only when the user asks for a quick standalone brainstorm or provides all needed material in the chat.

## Core Workflow

Use this default flow for a fresh webnovel idea:

1. Capture raw inspiration as reusable cards.
2. Identify genre, target reader, core emotional promise, and commercial hook.
3. Expand the strongest idea using a snowflake-style path: one sentence -> one paragraph -> character pressure -> five-beat mainline -> first ten chapters.
4. Produce a submission outline only when the user needs a pitch or directional document.
5. Produce an opening execution plan when the user wants to start writing quickly.
6. Maintain rolling records after writing begins: inspiration bank, character state, foreshadowing log, timeline, unresolved conflicts, and next 5-10 chapters.

## Reference Routing

Load only the reference needed for the current task:

- Read `references/inspiration-system.md` for fragments, daily notes, idea banks, material capture, market observations, scene images, dialogue, descriptions, and raw creative fuel.
- Read `references/market-positioning.md` for genre choice, target readers, reader psychology, selling points, trope fit, and long-form viability.
- Read `references/submission-outline.md` for pitch-ready outlines, editor-facing summaries, full-book direction, endings, and copywriting.
- Read `references/opening-chapters.md` for first chapter hooks, first three chapters, first ten chapters, opening conflict, and early promise delivery.
- Read `references/prose-execution.md` for drafting or revising actual prose, first-chapter text, unreliable narration, suspense openings, viewpoint control, information density, and chapter-ending hooks.
- Read `references/rolling-outline.md` for continuing after existing chapters, updating character state, tracking unresolved conflicts, and planning the next 5-10 chapters.
- Read `references/plot-diagnosis.md` for writer's block, sagging momentum, unclear goals, weak conflict, slow payoff, overloaded setup, and continuity repair.

## Artifact Defaults

When the user wants work saved to files, use these default project paths unless the project already has a clearer structure:

- `novel/` for chapter drafts and prose scenes.
- `outlines/` for submission outlines, first-ten-chapter plans, rolling outlines, and arc plans.
- `characters/` for character state cards and relationship notes.
- `worldbuilding/` for rules, settings, power systems, timelines, and special premise constraints.
- `materials/` for inspiration banks, market observations, description drills, and reusable scene fragments.

Use descriptive Chinese filenames when the project is Chinese-first, for example `outlines/过稿大纲.md` or `worldbuilding/双世界规则书.md`. Before overwriting an existing artifact, read it and update it carefully instead of replacing it wholesale.

## Output Rules

Keep outputs actionable and serial-friendly:

- Separate diagnosis, options, and recommended next step.
- Prefer chapter-level and scene-level next actions over abstract theory.
- Keep endings flexible unless the user explicitly needs a complete full-book outline.
- Avoid overwhelming the user with full worldbuilding forms at the start.
- Preserve useful uncertainty by marking items as fixed, tentative, or deferred.
- When using templates, adapt them to the user's actual premise instead of returning blank forms.

## Reusable Assets

Use these templates when the user wants a durable artifact:

- `assets/inspiration-card-template.md`
- `assets/inspiration-bank-template.md`
- `assets/submission-outline-template.md`
- `assets/first-ten-chapters-template.md`
- `assets/rolling-outline-template.md`
- `assets/character-state-card.md`
- `assets/timeline-template.md`
- `assets/dual-world-rulebook-template.md`
