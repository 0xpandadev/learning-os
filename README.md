# Learning OS

Learning OS is a stateful tutoring skill for children and adults.

It turns a folder into a long-term learning workspace with diagnosis, mastery maps, prerequisite tracking, retrieval practice, spaced review, misconception repair, practice banks, and coach or parent notes.

It is not just a prompt that says "teach me." It is a lightweight learning system that keeps the learner model in files.

```text
diagnose -> map -> teach one thing -> practice -> retrieve later -> update the learner model
```

## Documentation

- [Interactive multilingual guide](docs/index.html): English, Japanese, and Chinese in one click-switchable page.
- [Skill instructions](SKILL.md): the actual Codex skill.
- [System distillation notes](references/learning-system-distillation.md): the sources and learning-system ideas distilled into this skill.
- [Prompt examples](docs/prompt-examples.md): ready-to-use prompts for adults, children, parents, teachers, and self-study.

## What This Is

Learning OS is a reusable Codex skill for long-term learning. It helps an AI tutor stop behaving like a one-off explainer and start behaving like a careful learning coach.

It maintains:

- a mission
- a learner profile
- a diagnostic record
- a mastery map
- a misconception register
- a spaced retrieval schedule
- a practice bank
- learning records
- lesson files
- reference notes
- coach or parent notes

The key idea: **coverage is not learning**. A topic is only treated as learned when the learner demonstrates recall, use, transfer, or fluency.

## Why It Exists

Normal AI tutoring often fails in predictable ways:

- It explains too much before diagnosing.
- It forgets the learner's prior knowledge.
- It teaches topics in a flat list instead of a prerequisite graph.
- It treats "I explained it" as "the learner learned it."
- It does not schedule retrieval after the learner starts forgetting.
- It misses recurring misconceptions.
- It is often too adult-shaped for children and too childish for adults.

Learning OS fixes those failure modes by turning learning into a stateful workspace protocol.

## Core Files

| File | Purpose |
|---|---|
| `MISSION.md` | The real-world reason for learning and observable success criteria. |
| `LEARNER_PROFILE.md` | Age band, learning context, motivation, attention span, style, constraints. |
| `RESOURCES.md` | Trusted sources, books, papers, videos, communities, and source gaps. |
| `DIAGNOSTIC.md` | Initial and periodic diagnosis, including the learner's knowledge frontier. |
| `MASTERY_MAP.md` | Topic graph, prerequisites, mastery dimensions, evidence, and next actions. |
| `MISCONCEPTIONS.md` | Recurring errors, likely causes, repair strategies, and status. |
| `REVIEW_SCHEDULE.md` | Due retrieval prompts and spaced review commitments. |
| `PRACTICE_BANK.md` | Reusable tasks tagged by topic, difficulty, misconception, and evidence target. |
| `learning-records/` | Decision-grade records of demonstrated learning. |
| `lessons/` | One tight HTML lesson per file. |
| `reference/` | Compressed reference sheets, summaries, formulas, examples, glossaries. |
| `COACH_NOTES.md` | Optional notes for a parent, teacher, tutor, manager, or self-coach. |
| `NOTES.md` | Scratchpad for preferences and operating notes. |

## Modes

### Adult Mode

Best for professional learning, self-study, projects, exam prep, technical subjects, and adult reskilling.

Use it for:

- TypeScript, Python, Rust, SQL, AI agents, finance, writing, sales, design, research
- practical workplace tasks
- learning plans tied to deliverables
- high-signal review and transfer exercises

### Child Mode

Best for children or confidence-sensitive learners.

Use it for:

- elementary math
- reading comprehension
- writing
- English vocabulary
- science basics
- homework support
- exam foundations

Child Mode prioritizes short sessions, diagnosis without shame, small wins, concrete examples, and parent or teacher notes.

### Mixed Mode

Best when an adult is helping a learner.

Use it for:

- parent-assisted study
- teacher planning
- tutoring
- homeschool workflows
- manager/mentor learning plans

The lesson speaks to the learner, while `COACH_NOTES.md` gives the adult actionable support guidance.

## Installation

### Codex

Clone or install this repository into your Codex skills directory:

```powershell
git clone https://github.com/0xpandadev/learning-os.git $env:USERPROFILE\.codex\skills\learning-os
```

Restart Codex after installing so the skill list refreshes.

Then invoke:

```text
$learning-os
```

### Manual Use

You can also copy the repository folder into any skill host that supports a `SKILL.md` at the skill root.

## Quick Start

Create one folder per learning mission:

```powershell
mkdir C:\Users\you\learning\typescript-review
cd C:\Users\you\learning\typescript-review
```

Ask:

```text
$learning-os
Turn this folder into a Learning OS workspace for learning TypeScript type design.
My goal is to review production PRs and catch unsafe type design.
Start with a diagnostic, then create MISSION.md, LEARNER_PROFILE.md, DIAGNOSTIC.md, and MASTERY_MAP.md.
```

For a child:

```text
$learning-os
Turn this folder into a Learning OS workspace for an elementary-school learner studying fractions.
Use Child Mode. Start with a short confidence-safe diagnostic.
Create the mastery map and parent notes.
```

For ongoing sessions:

```text
$learning-os
Read the workspace state files, decide what will produce the most learning in 15 minutes, and run one lesson.
Start with retrieval before explanation. Update the mastery map and review schedule afterward.
```

## Example Use Cases

### Adult Technical Learning

- "Teach me SQL window functions until I can debug analytics queries at work."
- "Help me learn LLM function calling for product design decisions."
- "Build a learning path for TypeScript generics based on my current mistakes."
- "Diagnose my weak spots in React state management and map prerequisites."
- "Make me fluent in reading financial statements for public company analysis."

### Children And School

- "Help a 4th grader learn fractions without losing confidence."
- "Diagnose why this student keeps missing word problems."
- "Build a mastery map for elementary multiplication, division, fractions, and ratios."
- "Create 10-minute reading comprehension lessons with parent notes."
- "Track misconceptions in algebra and schedule retrieval practice."

### Parent Or Tutor

- "Separate what I say to the child from what I need to know as the parent."
- "Give me a 15-minute lesson and a 3-minute parent debrief."
- "Track confidence and frustration signals."
- "Create a practice bank for the exact mistakes from today's homework."

### Professional Reskilling

- "Help a nontechnical founder learn enough AI architecture to make product calls."
- "Teach a sales team consultative discovery through weekly diagnostics and practice."
- "Create a mastery map for writing better investment memos."
- "Turn our internal training into a spaced retrieval curriculum."

### Exam Prep

- "Map the topics I need for this exam and find my knowledge frontier."
- "Make mixed review sessions that prevent false fluency."
- "Schedule retrieval for formulas, definitions, procedures, and transfer problems."
- "Track which mistakes are conceptual vs careless vs time-pressure errors."

## Expected Effects

Learning OS is designed to improve:

- retention through spaced retrieval
- transfer through varied practice
- confidence through small wins
- efficiency through diagnosis before teaching
- accuracy through misconception tracking
- progression through prerequisite mapping
- coaching quality through separate adult-facing notes
- continuity through durable workspace state

It does not guarantee learning outcomes by itself. The learner still needs attention, practice, sleep, motivation, and honest feedback.

## Design Inspirations

Learning OS distills ideas from:

- Matt Pocock's `teach` skill: stateful teaching workspace, mission grounding, one-thing lessons.
- Math Academy: knowledge graph, adaptive diagnostics, knowledge frontier, task selection, spaced repetition, interleaving.
- Carnegie Learning / MATHia: skill-level mastery estimates updated from evidence.
- Anki / FSRS: retention-workload tradeoffs and review scheduling.
- Duolingo: lightweight practice, strength meters, forgetting curves, motivation design.
- OpenStax: spaced retrieval practice in school curriculum.

See [learning-system-distillation.md](references/learning-system-distillation.md).

## Repository Structure

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
├── templates/
│   ├── MISSION.md
│   ├── LEARNER_PROFILE.md
│   ├── DIAGNOSTIC.md
│   ├── MASTERY_MAP.md
│   ├── MISCONCEPTIONS.md
│   ├── REVIEW_SCHEDULE.md
│   ├── PRACTICE_BANK.md
│   └── COACH_NOTES.md
├── references/
│   └── learning-system-distillation.md
└── docs/
    ├── index.html
    └── prompt-examples.md
```

## License

See [LICENSE](LICENSE).
