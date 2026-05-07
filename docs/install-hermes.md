# Install in Hermes

Copy or symlink the skill into your Hermes skills directory.

## Copy install

```bash
mkdir -p ~/.hermes/skills/education
cp -R skills/prompt-dojo ~/.hermes/skills/education/prompt-dojo
```

Start a new Hermes session, then ask:

```text
Use the prompt-dojo skill. Start Lesson 1.
```

## Symlink install for contributors

From the repo root:

```bash
mkdir -p ~/.hermes/skills/education
ln -sfn "$PWD/skills/prompt-dojo" ~/.hermes/skills/education/prompt-dojo
```

## Verify

```bash
hermes skills list | grep prompt-dojo
```

If the current chat session does not see the skill, start a new session. Skill loading is session-scoped.
