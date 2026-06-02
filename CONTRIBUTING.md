# Contributing Skills

Thank you for sharing a skill with the Panda community!

## What you need

- A GitHub account
- A skill that works in [ai-assitant-panda](https://github.com/jinqishen0725/ai-assitant-panda)
- A fork of this repository

## Step-by-step

### 1. Export from Panda

1. Open **Skills → My Skills**
2. Swipe right on your skill → **Export**
3. Save the `.panda-skill.zip` package (AirDrop, Files, etc.)

### 2. Prepare the folder

1. Fork [panda-skills-community](https://github.com/jinqishen0725/panda-skills-community)
2. Clone your fork locally
3. Unzip the export into `skills/<skill-slug>/`
   - The folder name must match the skill slug (lowercase, hyphenated), e.g. `daily-standup-summary`
   - Or copy `skills/_template/` and edit `SKILL.md`

### 3. Check `SKILL.md` frontmatter

Required fields:

```yaml
---
name: your-skill-slug
display_name: Your Skill Title
description: One-line summary shown in the Community store.
author: your-github-username
tags: productivity,community
session_behavior: always_create_new
execution_mode: send_message
---
```

Optional: `version: 1.0.0`

If `author` is omitted, the app displays `panda-community`.

### 4. Validate locally (recommended)

Import the folder back into Panda:

- **Skills → Import** (zip), or
- Copy the folder into Panda's skills directory on a simulator/device

Run the skill once to confirm it behaves as expected.

### 5. Open a pull request

```bash
git checkout -b add-skill-your-skill-slug
git add skills/your-skill-slug
git commit -m "Add your-skill-slug community skill"
git push origin add-skill-your-skill-slug
```

Open a PR against `main` on [panda-skills-community](https://github.com/jinqishen0725/panda-skills-community).

Include in the PR description:

- What the skill does
- How you tested it
- Any parameters the user must fill in

### 6. Review and merge

Maintainers will review for:

- Valid `SKILL.md` and folder layout
- Sensible prompt / no harmful instructions
- Unique slug (no collision with existing skills)

After merge, users see the skill in **Skills → Community** within a refresh.

## No GitHub?

Open a [GitHub issue](https://github.com/jinqishen0725/panda-skills-community/issues/new) with your exported zip attached and we can help land it via PR.

## Template

Start from [`skills/_template/SKILL.md`](skills/_template/SKILL.md).
