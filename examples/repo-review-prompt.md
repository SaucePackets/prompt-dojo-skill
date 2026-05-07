# Example — Public Repo Review Prompt

```text
Task:
Review this repository before I share it publicly.

Context:
It is a small public skill bundle for AI agents. The audience is developers who may install the skill in Hermes or OpenClaw.

Constraints:
- Do not make code changes.
- Do not invent unsupported features.
- Check for private notes, personal details, broken install steps, unclear README copy, and missing license/install docs.
- If you mention a problem, name the exact file.

Output:
Return:
- Ship blockers
- Confusing parts
- Nice-to-have polish
- Final verdict: ship / hold

Quality bar:
A ship blocker must be serious enough that publishing the repo would confuse users, leak private information, or make install fail.
```

## Why this works

The prompt tells the agent what kind of repo it is, what risks matter, what not to do, and how to structure the review.
