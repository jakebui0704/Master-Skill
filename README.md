# Master Skill

Jake's personal "chief of staff" skill. It interviews one question at a time, then tells you
which skill to use, why, how, with a copy-paste prompt, and who does it (Jake or Thanh).

```
master-skill/
├── .claude/skills/master-skill/SKILL.md      # the skill itself (trigger: /master-skill)
│   ├── references/catalog.md                 # every skill + overlap rules + Jake/Thanh split
│   ├── references/playbook-idea-to-validate.md # repeatable idea → validation system
│   └── evals/evals.json                     # test prompts for checking the skill
```

**Install (claude.ai):** build a `master-skill.skill` package with skill-creator, then click **Save skill**, or upload the
`master-skill/` folder in claude.ai → Settings → Capabilities → Skills.

**Keep it fresh:** when you add or remove skills, update `references/catalog.md`.
