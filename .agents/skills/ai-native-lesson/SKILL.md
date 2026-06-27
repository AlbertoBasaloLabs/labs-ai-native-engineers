---
name: ai-native-lesson
description: Build lesson material for Alberto Basalo's course "From Vibe Coders to AI-Native Engineers". Produces a Marp-ready Markdown lesson in the fixed Connections / Concepts / Concrete practice / Conclusion structure, advancing the AstroBookings demo by one coherent increment closed with a single Conventional Commit. Use this whenever drafting, writing, or formatting any of the 24 course lessons — when the user references a lesson number (e.g. "1.2", "4.1"), a module name (e.g. "Context Engineering", "Spec-Driven Development"), or asks for the "guion", "slides", "material" or "práctica" of a lesson for this course.
---

# AI-Native Engineers — Lesson Builder

Generate one self-contained lesson as a Marp slide deck that doubles as the live teaching script. Every lesson follows the same four-part rhythm and advances the same demo, so the 24 lessons feel like one continuous project.

**Before drafting, read `references/course-map.md`** — it holds the full 24-lesson outline, the AstroBookings domain model, the commit conventions, and the narrative constraints. Use it to place the requested lesson in context (what came before, what the demo state is, what this lesson must introduce). Read the `references/astro-bookings.md` file to understand the domain model and the demo.

**Inspirational:** At this repo I have a pro version of the skills I want to teach in this course. https://github.com/AIDDbot/AIDDbot/tree/main/.agents/skills The gaol is to take the attendees in a a journey to build their own skills. Those are examples, but naming and philosophies should be taken as inspiration.


## Conventions that always hold

- **Language:** narration in Spanish; prompts, commit messages, code identifiers and the four section headings (`Connections`, `Concepts`, `Concrete practice`, `Conclusion`) in English.
- **Tech-agnostic:** never name a framework, language or library. Refer to "the endpoint", "the UI view", "the model". The stack is chosen only at recording/delivery time.
- **One demo, one thread:** each lesson moves AstroBookings forward by one increment that feels like a natural next step in a real project, never an artificial exercise.
- **One commit per lesson:** close every Concrete practice with a single Conventional Commit `type(scope): description` (see commit rules below).
- **Concise:** student-facing, no instructor stage directions, no meta-commentary, no mention of the pedagogical model. Each section fits on one slide.
- **Short:** Use short sentences and avoid long paragraphs.

## Output format

Read and use this exact skeleton `assets/lesson-template.md` filling any {placeholder} with the actual content.


## Section rules

**Connections (1–2 questions).** Surface what the learner already knows or has felt about this lesson's topic. Professional developers who already use AI informally are the audience — tap that. Short and concise questions only, no answers.

**Concepts (up to 3).** The new ideas, one sentence each, ordered so they build toward the lesson's AI-native concept. Three is a ceiling, not a quota — use two if two suffice.

**Concrete practice.** The hands-on increment. Give the literal prompts/actions to run (English, in backticks) so they can be copied live. Keep loops short. End with the commit. The practice must leave AstroBookings in a coherent, runnable state consistent with the next lesson's starting point.
Can be a set of slides (one for each step) or a single slide with the steps numbered if short enough.
Only add extra files when attendees must copy artifacts into their repos (skills, rules, prompts, specs, etc.). Not every lesson needs them.

**Conclusion.** Learner summarizes the gain/cost, evaluates one decision, and the last bullet bridges to the next lesson's concept (the loop lengthens, control moves earlier). Short and concise.

## Commit rules

`type(scope): description` carries three traceability axes:
- **Functional:** `feat`, `fix`
- **Quality / non-functional:** `test`, `refactor`, `ci`, `docs`, `chore`
- **AI-course:** scopes `ai`, `rules`, `agents`, `context`, `obs`, `hooks`, `loop`

Choose the scope that names what the lesson introduces (domain scope like `rockets`/`launches`/`bookings` for pure feature steps; an AI-course scope when the lesson's point is the practice itself).

**Green by default.** The whole course has exactly **two intentionally "red" (failing-then-fixed) moments**: the overbooking fix in **4.2** and the DTO→Value-Object refactor in **5.3**. Every other lesson commits green. This sparseness is the thesis: disciplined AI workflows reduce chaos rather than amplify it — do not add red moments elsewhere.

If Alberto has a master commit already assigned to the lesson, use his; otherwise propose one consistent with these rules and flag it as a proposal.

## File naming
- Create a lesson directory: `/lessons/M-L-slug/`.
- Main lesson file is always the index file numbered with `0`: `/lessons/M-L-slug/M-L-0-slug.md` (example: `/lessons/1-1-vibe-coding/1-1-0-vibe-coding.md`).
- Optional extra files are only for attendee copy/paste artifacts and are not required in every lesson.
- Optional extra files must be numbered sequentially from `1` onward and named after how the artifact will actually be used once copied into the attendee's repo — not after the lesson slug. Pattern: `/lessons/M-L-slug/M-L-N-<artifact-slug>.<kind>.md`, where `<kind>` reflects the primitive (`prompt`, `rules`, `skill`, `spec`, `plan`, etc.).
- Example: the reusable prompt of lesson 1.2 is `/lessons/1-2-ai-coding-primitives/1-2-1-scaffold-resource.prompt.md`, the rules are `1-2-2-project-conventions.rules.md`, and the skill is `1-2-3-create-endpoint.skill.md`.