# Learning OS Prompt Examples

Use these prompts after installing the skill.

## Start A New Workspace

```text
$learning-os
Turn this folder into a Learning OS workspace for {topic}.
The learner is {adult/child/mixed}.
The real goal is {observable outcome}.
Start with a diagnostic before teaching.
Create the core files and explain the first recommended next step.
```

## Continue A Session

```text
$learning-os
Read MISSION.md, LEARNER_PROFILE.md, DIAGNOSTIC.md, MASTERY_MAP.md, MISCONCEPTIONS.md, and REVIEW_SCHEDULE.md.
Pick the highest-value 15-minute lesson for today.
Start with retrieval, teach one thing, give practice, then update the learner model.
```

## Child Math

```text
$learning-os
Use Child Mode.
The learner is a 4th grader who gets nervous with fractions.
Run a 5-question diagnostic that starts easy.
Do not call mistakes "wrong" harshly. Treat mistakes as clues.
Create MASTERY_MAP.md, MISCONCEPTIONS.md, REVIEW_SCHEDULE.md, and COACH_NOTES.md.
```

## Parent-Assisted Study

```text
$learning-os
Use Mixed Mode.
Teach the learner directly, but write parent-facing observations separately in COACH_NOTES.md.
After the lesson, tell me:
1. what improved
2. what is still fragile
3. what I should say tomorrow
4. what I should avoid saying
```

## Adult Technical Learning

```text
$learning-os
I want to learn TypeScript type design so I can review production pull requests.
Start by diagnosing generics, inference, conditional types, mapped types, and unsafe escape hatches.
Build a mastery map with prerequisites and transfer tasks.
```

## AI Product Learning

```text
$learning-os
I want to understand AI agent architecture well enough to make product roadmap decisions.
Use Adult Mode.
Do not make this a theory lecture. Diagnose what I know, then teach through product decision scenarios.
```

## Language Learning

```text
$learning-os
I want to improve English business writing for investor and partner emails.
Diagnose my current writing with a short task.
Track recurring mistakes in MISCONCEPTIONS.md.
Schedule retrieval for phrases, structure, and tone patterns.
```

## Exam Prep

```text
$learning-os
I have an exam in 6 weeks.
Create a mastery map from the syllabus.
Diagnose the knowledge frontier.
Build a review schedule that mixes new learning, retrieval, and cumulative quizzes.
```

## Misconception Repair

```text
$learning-os
The learner keeps making the same mistake: {describe mistake}.
Do not just explain the correct rule.
Identify the likely misconception, design two contrast examples, then update MISCONCEPTIONS.md.
```

## Review Compression

```text
$learning-os
Several reviews are due today.
Compress them into the fewest mixed tasks possible.
If one higher-level task implicitly reviews prerequisites, record that in REVIEW_SCHEDULE.md.
```

## Mastery Map Update

```text
$learning-os
Based on today's performance, update MASTERY_MAP.md conservatively.
Only raise mastery where there is evidence.
If a score should go down because of forgetting or hint dependence, lower it and explain why.
```

## Generate A Lesson File

```text
$learning-os
Create one HTML lesson in lessons/ for the next topic in the mastery map.
It should teach exactly one thing, include 3 practice tasks, and end with a retrieval prompt.
Make it print-friendly.
```

## Build A Practice Bank

```text
$learning-os
Create PRACTICE_BANK.md entries for the weak topics in MASTERY_MAP.md.
Tag each task by difficulty, targeted misconception, and what evidence it can produce.
```

## Coach Notes Only

```text
$learning-os
Do not make a new lesson.
Read the workspace files and update COACH_NOTES.md with what the coach should do in the next 10-minute session.
```
