# Install in Hermes

Copy or symlink both `prompt-dojo` and the vendored `teach-mode` skill into your Hermes skills directory.

## Copy install

```bash
mkdir -p ~/.hermes/skills/education
cp -R skills/teach-mode ~/.hermes/skills/education/teach-mode
cp -R skills/prompt-dojo ~/.hermes/skills/education/prompt-dojo
```

## Hermes hub install

```bash
hermes skills install SaucePackets/prompt-dojo-skill/skills/teach-mode --yes
hermes skills install SaucePackets/prompt-dojo-skill/skills/prompt-dojo --yes
```

Start a new Hermes session, then ask:

```text
Use the prompt-dojo skill. Start Lesson 1.
```

## Symlink install for contributors

From the repo root:

```bash
mkdir -p ~/.hermes/skills/education
ln -sfn "$PWD/skills/teach-mode" ~/.hermes/skills/education/teach-mode
ln -sfn "$PWD/skills/prompt-dojo" ~/.hermes/skills/education/prompt-dojo
```

## Verify

```bash
hermes skills list | grep -E 'teach-mode|prompt-dojo'
```

If the current chat session does not see the skill, start a new session. Skill loading is session-scoped.
