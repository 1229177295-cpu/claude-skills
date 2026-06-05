# project-retrospective

A Claude Code skill for systematic project retrospectives — covering the full cycle from reflection to methodology documentation to shareable slides.

Built for data analysts, UX researchers, product managers, and anyone who wants to turn project experience into reusable knowledge.

---

## What it does

Most retrospectives stop at "what went wrong / what went right." This skill goes further:

1. **Structured reflection** — guides you through a co-creation dialogue to surface root causes, not just surface observations
2. **Methodology documentation** — extracts reusable methods from the project (e.g. statistical frameworks, research protocols) into a standalone reference doc
3. **Slides generation** — converts the methodology doc into a shareable web presentation via the `frontend-slides` skill

---

## Workflow

| Phase | Activity | Output |
|-------|----------|--------|
| Phase 1 | Project info alignment | Project overview card |
| Phase 2 | Completion review by stage | Completion matrix |
| Phase 3 | Deep reflection dialogue | Reflection record |
| Phase 4 | Systematic synthesis | Retrospective report |
| Phase 5 | SOP + checklist generation | Reusable SOP + checklist card |
| Phase 6 | Methodology documentation | Methodology reference doc |
| Phase 7 | Slides generation | HTML presentation (via frontend-slides) |

---

## How to install

1. Copy the `project-retrospective/` folder into your `~/.claude/skills/` directory
2. Restart Claude Code — the skill will be auto-detected

```
~/.claude/skills/
└── project-retrospective/
    └── SKILL.md
```

---

## How to trigger

The skill activates automatically when you mention any of these:

**Retrospective triggers:**
复盘、回顾、retro、项目总结、项目回顾、经验沉淀、反思、lessons learned、做完总结、优化建议、改进方向

**Methodology triggers:**
方法论沉淀、把方法整理成文档

**Slides triggers:**
生成slides、做成PPT、生成演示文稿、可以分享的材料

Or just say: *"帮我复盘一下这个项目"*

---

## Quick-start examples

| You say... | Skill jumps to... |
|------------|------------------|
| "帮我复盘一下这个项目" | Phase 1 — full flow |
| "我来说说踩的坑" | Phase 3 — reflection dialogue |
| "给我出个复盘报告" | Phase 3 + 4 |
| "帮我沉淀一下方法论" | Phase 6 — methodology doc |
| "把方法论做成Slides" | Phase 6 → Phase 7 |
| "复盘完了，做一版可以分享的材料" | Phase 6 + 7 — full output |

---

## Dependencies

- **frontend-slides** skill (required for Phase 7 Slides generation) — install separately from the same marketplace

---

## Design principles

- **Co-creation over report generation** — the skill asks before it concludes; you shape the output
- **Root cause over symptom** — every "pit" gets traced to its underlying reason
- **Method over conclusion** — methodology docs capture *how to do things*, not project-specific results
- **Progressive depth** — you can stop at any phase; each phase produces standalone value

---

## License

MIT
