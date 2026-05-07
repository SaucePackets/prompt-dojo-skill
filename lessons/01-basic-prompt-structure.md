# Lesson 1 — Basic Prompt Structure

## Idea

A useful prompt gives the model a job, the context it needs, the constraints it must obey, the output shape you want, and the quality bar for success.

If any of those are missing, the model fills gaps with guesses. Cute. Dangerous.

## Bad prompt

```text
Review this repo and tell me what you think.
```

## Better prompt

```text
Task:
Review this GitHub repo before I share it publicly.

Context:
It is a small public skill bundle. I care about clarity, installability, and not leaking private notes.

Constraints:
Do not rewrite files. Do not suggest fake features. Focus on README, install docs, repo layout, and privacy leaks.

Output:
Return three sections:
- Ship blockers
- Nice-to-have improvements
- Final verdict

Quality bar:
A blocker must name the exact file and why it would embarrass or confuse a public user.
```

## Why it works

- The task is specific.
- The context explains what matters.
- The constraints prevent wandering.
- The output format is scannable.
- The quality bar makes the review testable.

## Your rep

Write a prompt for this task:

```text
You want an AI agent to review a blog post before publishing it.
```

Use this shape:

```text
Task:
Context:
Constraints:
Output:
Quality bar:
```

## Scorecard

- Clarity: /10
- Context: /10
- Constraints: /10
- Output format: /10
- Testability: /10
- Model control: /10
