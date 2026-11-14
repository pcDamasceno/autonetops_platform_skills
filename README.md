# AutoNetOps platform skills

Agent skills for the AutoNetOps platform. Each skill lives in
`skills/<name>/` with a `SKILL.md` (YAML front matter + instructions) and
any extra reference `.md` files next to it.

| Skill | Used by |
|---|---|
| [`write-lesson`](skills/write-lesson/SKILL.md) | Claude Code in the platform repo, and the lesson widget (loaded at runtime by the negotiator service from `main`) |

The negotiator fetches `skills/write-lesson/` from `main` through the GitHub
API and caches it by commit SHA, so a push here reaches the widget within a
few minutes, with no deploy.
