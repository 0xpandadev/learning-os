# Learning System Distillation

This skill distills several strong learning-system patterns into a lightweight Codex workspace protocol.

## Sources Used

- Matt Pocock `teach`: stateful teaching workspace, mission grounding, one-thing lessons, learning records, trusted resources.
  - https://github.com/mattpocock/skills/tree/main/skills/productivity/teach
- Math Academy: knowledge graph, student model, adaptive diagnostic, knowledge frontier, task selection, spaced repetition on connected topics, interleaving, and foundation repair.
  - https://www.mathacademy.com/how-our-ai-works
  - https://mathacademy.com/pedagogy
- Carnegie Learning MATHia: mastery workspaces and skill-level mastery estimates updated by evidence from correct answers, mistakes, and answer requests.
  - https://support.carnegielearning.com/help-center/math/teaching-strategies/educators/teaching-strategies/mathia/getting-started-in-mathia/article/understanding-mastery-and-concept-builder-workspaces-in-mathia/
- Anki / FSRS: retention-workload tradeoff, review scheduling, and honest failure signals.
  - https://docs.ankiweb.net/deck-options
  - https://faqs.ankiweb.net/what-spaced-repetition-algorithm.html
- Duolingo learning science: student model, forgetting curves, practice weak skills, lightweight play, mistake review, and personalized practice.
  - https://blog.duolingo.com/how-we-learn-how-you-learn/
  - https://blog.duolingo.com/spaced-repetition-for-learning/
- OpenStax Algebra 1: spaced retrieval practice inside a school curriculum.
  - https://openstax.org/books/algebra-1/pages/spaced-retrieval-practice

## Distilled Ideas

1. `Mission`: learning needs an outcome, not only a topic.
2. `Knowledge graph`: topics are connected by prerequisite and component relationships.
3. `Student model`: learner state is estimated from evidence and can change.
4. `Diagnostic frontier`: a good diagnostic finds the boundary between ready and not-yet-ready.
5. `Mastery`: mastery has dimensions: conceptual, procedural, retrieval, transfer, and fluency.
6. `Retrieval`: durable learning requires producing answers after time has passed.
7. `Spacing`: the review time should respond to recall success, effort, and workload.
8. `Interleaving`: mix related skills carefully; avoid blocked practice creating false fluency.
9. `Misconceptions`: errors should be classified and repaired, not merely marked wrong.
10. `Motivation`: especially for children, task selection should protect morale and momentum.

## What This Skill Adds To `teach`

- Initial and periodic diagnostic protocol.
- Explicit mastery map with prerequisites and skill dimensions.
- Review schedule for spaced retrieval.
- Misconception register.
- Practice bank.
- Child/adult/mixed learner modes.
- Coach or parent notes.
- Task selection rules that weigh due reviews, prerequisites, mission relevance, interference, and motivation.
