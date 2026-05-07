# prompt-dojo-skill

Prompt Dojo is a practical prompt-writing skill bundle for Hermes and OpenClaw.

It teaches prompt design through short reps: learn one concept, compare bad and better prompts, write your own prompt, critique it, rewrite it, then save a reusable template.

## What this includes

- `skills/prompt-dojo/SKILL.md` — the teaching workflow and guardrails.
- `skills/prompt-dojo/references/lesson-template.md` — reusable lesson format.
- `lessons/01-basic-prompt-structure.md` — first public lesson.
- `templates/basic-task-context-constraints-output.md` — starter template.
- `examples/repo-review-prompt.md` — practical developer example.
- `docs/install-hermes.md` and `docs/install-openclaw.md` — runtime install notes.

## Who it is for

- Developers learning to work better with AI agents.
- Teams trying to make prompts testable and reusable.
- People tired of vague AI instructions and mushy output.
- Meetups or study groups that want prompt practice, not prompt theory sludge.

## Learning stance

This is active practice.

The learner writes first. The agent teaches, critiques, scores, and helps refine after the attempt.

## First rep

Ask your agent:

```text
Use the prompt-dojo skill. Start Lesson 1.
```

## Repo layout

```text
prompt-dojo-skill/
├── README.md
├── LICENSE
├── docs/
│   ├── install-hermes.md
│   └── install-openclaw.md
├── examples/
│   └── repo-review-prompt.md
├── lessons/
│   └── 01-basic-prompt-structure.md
├── skills/
│   └── prompt-dojo/
│       ├── SKILL.md
│       └── references/
│           └── lesson-template.md
└── templates/
    └── basic-task-context-constraints-output.md
```

## Roadmap

- Add lessons for roles, examples, output schemas, hallucination control, evals, and tool-use prompts.
- Add promptfoo-style eval examples.
- Add agent workflow prompt patterns.
- Add domain examples for code review, research, finance, and product planning.

## Note

This repo is public-clean. It does not include private lesson history, personal critique logs, or private project notes.
