# raise-it-land-it-skills

Two portable Agent Skills for the proposed MDOE407 **Raise It, Land It** course, version 0.1.1.

**Frame** records a learner-owned four-field preparation card for cycle 1 formative practice. It asks questions and preserves the learner’s words without supplying arguments, inferred motives or coaching. **Trace** helps a tutor review a deidentified completed role-play, locating evidence for five markers (with M2a/M2b observations), uncertainty and opportunity concerns. It is advisory and does not grade.

## Layout

```text
skills/frame/SKILL.md       Frame instructions, with references and card asset
skills/trace/SKILL.md       Trace instructions, rubric, protocol and review template
examples/                  Fictional inputs only
tests/                     Separate intended behaviour checks
VALIDATION.md              What has and has not been verified
```

## Use in a compatible agent

Choose an agent that supports Agent Skills and access to the skill’s local resources. Follow that agent’s native installation/import instructions: install the complete `skills/frame` and/or `skills/trace` folder, keeping `SKILL.md`, `references/` and `assets/` together. If it installs from a repository, select the appropriate skill subfolder. Invoke Frame or Trace using that agent’s documented skill-selection mechanism. Use a fresh conversation per attempt/run and the fictional input in `examples/` for a first check.

These are skills for compatible agents, not standalone software or a prompt guaranteed to work in a bare language model. Installation, skill selection and resource access vary by agent. Portability of the files does not establish identical behaviour, reliable loading or cross-provider validation. Trace must stop if its required resources are unavailable.

## Runtime boundaries

Frame accepts a public fictional cycle 1 brief supplied at runtime or confirmation that the learner has one. It does not support assessed/cycle 2 preparation, live calls, coaching or grading. The facilitator controls timing and card handling; the skill does not lock, save or collect cards.

Trace operates after a run, including a tutor’s post-run review of an assessed run; it never assists the assessed performance. Supply deidentified transcript roles, coverage and only the public context needed. No hidden counterpart card, assessed solution, private workplace data or other learner’s run is required. Reasoned retention can evidence M2b; concession is not the goal. M5 requires explicit decision, owner, review condition, agreement and feasibility evidence. The tutor retains assessment responsibility.

Neither skill guarantees privacy, consent, memory isolation, deletion, institutional compliance or fairness. Use the institution’s approved environment and data arrangements. Human preparation/coding remains available. See [validation limits](VALIDATION.md) and [intended behaviour](tests/expected-behaviour.md).
