# Panda Skills Community

Public skill catalog for [ai-assitant-panda](https://github.com/jinqishen0725/ai-assitant-panda).

The Panda app scans the `skills/` folder in this repository. Each subfolder with a valid `SKILL.md` appears in **Skills → Community**.

## Install a skill

1. Open Panda → **Skills → Community**
2. Pick a skill → **Install**

## Contribute a skill

See **[CONTRIBUTING.md](CONTRIBUTING.md)** for the full PR workflow.

Quick version:

1. Export your skill in Panda (**My Skills** → swipe right → **Export**)
2. Fork this repo
3. Add `skills/<your-skill-slug>/` (copy from `skills/_template/` if helpful)
4. Open a pull request

After merge, the skill shows up in the Community store on refresh — no app update required.

## Layout

```
skills/
  _template/          # starter template (ignored by the app)
  your-skill-slug/
    SKILL.md          # required
    scripts/          # optional
    references/       # optional
    templates/        # optional
```

Legacy folders (`index.json`, `packages/`) may remain for reference but are not used by the current app catalog.
