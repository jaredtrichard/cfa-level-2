---
name: cfa-study
description: Run personal CFA Level II open-response study, resume unfinished work, grade evidence, and improve the current lesson within this Markdown project.
---

# Study and improve in place

The project root is three levels above this skill directory. On first study use, create ignored `local-data/` and copy public `RESUME.md`, `MEMORY.md`, and `TRACKER.md` into it only when each destination is missing. Never overwrite existing learner state. Create `local-data/log/` for actual attempts, using the public `log/TEMPLATE.md` as a shape. No dependency installation is needed.

Read `local-data/RESUME.md` and `local-data/MEMORY.md`. Use `local-data/TRACKER.md` for learner evidence and `sources/QUALITY.md` for source checks. When shared syllabus rows or coverage improve, merge those additions into the personal tracker by stable ID without resetting learner states. Public `TRACKER.md` records reusable scope/source coverage; its learning dimensions stay unassessed and it never links to private evidence. In private files, link to shared files using `../` where necessary. Do not invent prior knowledge or present a source gap as a student weakness.

## Teach

Select a current outcome with the learner. Check its exact wording in the official PDF using the tracker page and module-relative bullet ordinal. Verify substantive coverage before teaching it; an outline alone is not an answer key. Use ../../../modules/TEMPLATE.md as a provisional shape, adapting it to feedback. Author just the needed lesson in `modules/<topic>/` and original prompts and solutions in separate files under `practice/<topic>/`. Give the learner the prompt without revealing the solution. Use open-response explanation, calculations where relevant, and case interpretation. Keep unseen validation cases separate from teaching examples, and record exposure when shown.

## After every submitted answer

1. Before grading, append the exact available answer/transcript and all submitted calculations to `local-data/log/YYYY-MM-DD.md` (learner’s local timezone). Give the attempt a unique heading such as `attempt-001`. Record exact prompt or immutable prompt version, outcome IDs, hint/solution exposure, and timestamp. Mark pending grading and save `local-data/RESUME.md` with the attempt link. If persistence fails, resolve it before grading; do not claim it was saved.
2. Clarify ambiguous spoken numbers, units, signs, or wording before judging affected parts. Preserve the raw transcript and append the clarification separately. An unclear transcript is not evidence of a misconception.
3. Check the solution/rubric against sourced assumptions, applicable edition, and independently computed arithmetic. If unresolved, leave grading pending with the precise question. Assess what the learner actually said; confidence, hedging, or fluency alone does not determine correctness.
4. Append the assessment and specific feedback to the same log, linking the checked rubric/source version. Distinguish misconception, arithmetic slip, ambiguous transcription, grader error, and bad/ambiguous prompt. Explain the decisive reasoning. Never overwrite the original answer or an old assessment.
5. Update only the relevant private tracker dimensions with evidence links, then update `local-data/RESUME.md` with the exact stopping point, unfinished question, submitted work, hints, pending grading, and next action. Interrupted work resumes here before introducing a new task.
6. Improve the current lesson or solution immediately when evidence or learner feedback warrants it; no course rebuild. Log what changed and why, preserving the prior prompt/rubric text in the attempt record or an already-existing Git revision. Presentation can change; official requirements cannot be softened for agreement. Add durable memory only for confirmed recurring patterns, linking supporting attempts.

If a source or answer key was wrong, append a correction and reassessment linked to the old assessment. Repair affected tracker states and memory, identify other affected attempts, and preserve the original history. Do not silently turn a grading mistake into learner error. A source correction may reopen previously demonstrated outcomes.

## Evidence states

Track explain, calculate, and apply separately: `unassessed`, `developing`, `demonstrated`, or `revisit`. Use `not-applicable` only with an outcome-specific reason; initially calculation applicability is unchecked. Record source coverage separately as `unverified`, `partial`, or `checked`, with source/lesson links.

Use developing for incomplete or assisted evidence. Demonstrated requires correct independent work in fresh cases and cold retrieval on a later encounter, with reasoning and all relevant conditions covered. Immediate repetition, reading, or a single coached success is insufficient. No fixed study intervals or access gates. When only part of an outcome was tested, record that boundary; do not promote the entire dimension. Verbal mastery does not establish timed multiple-choice exam readiness.

## Publish reusable improvements

Apply source-checked improvements to shared lessons and solutions during study. Keep quotations of learner answers, grading history, personal details, and links to private attempts only in `local-data/`. Shared improvement notes explain the general correction and cite public sources; they do not narrate a learner's performance. Public practice is original authored material, not logs disguised as examples.

Follow AGENTS.md publishing authorization. Before committing and pushing shared changes, inspect the staged diff and file list, verify no private paths are tracked, check internal links, and verify changed numerical examples. Keep public templates blank. Do not force-add ignored files, push private/bootstrap branches, or publish source PDFs/textbooks. Commit and push meaningful shared improvements to the authorized public main branch; private-only session updates need no public commit.
