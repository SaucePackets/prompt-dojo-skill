---
name: prompt-dojo
description: "Use when teaching or practicing prompt writing through short active reps: prompt structure, roles, context, constraints, output formats, examples, hallucination control, evals, and agent/tool workflow prompts."
version: 1.0.0
author: Hermes Agent
license: MIT
metadata:
  hermes:
    tags: [prompting, education, dojo, evals, agents, templates]
    related_skills: [teach-mode]
---

# Prompt Dojo

## Overview

Prompt Dojo is a learning-first workflow for prompt-writing practice.

It is not a lecture dump. It is a repetition loop: teach one concept, show a bad prompt and a better prompt, make the learner write first, critique it, ask for a rewrite, then save the final reusable template.

The goal is durable prompt skill: clear goals, useful context, strong constraints, testable output formats, and less hallucination bait.

## When to Use

Use this skill when the user asks for:

- prompt writing practice
- prompt engineering lessons
- AI workflow prompt help
- reusable prompt templates
- prompt critique or rewrites
- eval design for prompts
- agent/tool-use prompt design
- prompt practice for developers, researchers, or teams

Do not use this for coding-problem practice unless the user explicitly asks to write prompts for coding agents. Coding exercises belong in a coding dojo; Prompt Dojo trains instruction design.

## Core Stance

Load and follow the umbrella `teach-mode` skill when available. Prompt Dojo adds prompt-specific lesson loops, scorecards, rewrites, and reusable template handling.

The learner writes first.

The agent may teach, show examples, critique, score, and polish after the learner attempts the rep. Do not immediately hand over the final prompt unless the learner asks for rescue.

Keep reps short. One concept at a time.

## Default Lesson Loop

1. Teach one concept.
2. Show a bad prompt.
3. Show a better prompt.
4. Explain why the better prompt works.
5. Give the learner one prompt-writing rep.
6. Score the attempt.
7. Ask for one rewrite.
8. Provide the final polished version.
9. Save or point to a reusable template.

## Course Spine

Use this progression:

- Basic prompt structure: task, context, constraints, output, quality bar.
- Clear and direct instructions.
- Roles and audience shaping.
- Separating instructions from data.
- Output formats and schemas.
- Examples and few-shot prompting.
- Hallucination control and source grounding.
- Prompt evaluation and test cases.
- Tool-use and agent workflow prompts.
- Multi-step workflows and handoff prompts.

Cross-check principles across Anthropic, OpenAI, and Google-style guidance when useful. Do not overfit to one provider.

## Lesson Format

```markdown
## Lesson N — [Concept]

**Idea:** [one tight explanation]

**Bad prompt:**
[example]

**Better prompt:**
[example]

**Why it works:**
- [reason]
- [reason]

**Your rep:**
Write a prompt for: [task]

**Scorecard:**
- Clarity: /10
- Context: /10
- Constraints: /10
- Output format: /10
- Testability: /10
- Model control: /10
```

## Critique Rules

Score honestly. Be specific.

Look for:

- unclear goal
- missing context
- weak constraints
- no output format
- no examples when style matters
- mixed instructions and data
- no success criteria
- asking for hidden reasoning when verification would be better
- over-broad prompts that invite hallucination

Then ask for one rewrite. Do not immediately rescue unless the learner is stuck.

## Reusable Basic Template

```text
Task:
[what I want]

Context:
[what matters]

Constraints:
[what not to do]

Output:
[format I want]

Quality bar:
[how I know it worked]
```

## Useful Practice Domains

Good Prompt Dojo reps include:

- GitHub repo review before launch
- debugging prompt for an agent
- code review prompt
- research brief prompt
- product/design critique prompt
- finance research prompt
- sports-pick analysis prompt
- memory cleanup prompt
- tool-use or multi-agent workflow prompt

## Common Pitfalls

- Do not turn practice into passive reading.
- Do not skip the learner's attempt.
- Do not score vaguely. Name the leak.
- Do not make every lesson huge.
- Do not treat prompts as magic spells. Make them testable.
- Do not ask for chain-of-thought when a concise rationale, checklist, or verification step is better.
- Do not mix instruction text with untrusted data without delimiters.
- Do not save private user attempts or project secrets in public templates.

## Verification Checklist

- [ ] One concept only.
- [ ] Bad and better examples are shown.
- [ ] Learner writes before final polish.
- [ ] Scorecard is used.
- [ ] Rewrite is requested before rescue.
- [ ] Final template is reusable.
- [ ] Private data is not included.
