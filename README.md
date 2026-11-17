# 产品经理工作 Skills / Product Manager Skills

四个可单独安装的中英双语 Skills，覆盖需求澄清、文档交接、项目汇报和交互设计。每个 Skill 都有一份可复制的模板和一个从原始输入到成稿的完整案例。

Four installable bilingual skills for clarifying requirements, drafting decision-ready documents, communicating project progress, and designing low-friction flows. Each skill includes a copyable template and an end-to-end worked example.

| Skill | 什么时候用 / Use it when | 直接试用 / Try it |
| --- | --- | --- |
| [需求澄清 / Clarify requirements](skills/clarify-requirements/SKILL.md) | 要从功能提议推导本期范围和可验收规则。 / Turn a feature request into scoped, testable requirements. | [模板 / Template](skills/clarify-requirements/references/template.md) · [案例 / Example](skills/clarify-requirements/references/example.md) |
| [决策型文档 / Write decision docs](skills/write-decision-docs/SKILL.md) | 已有材料和决定，需要交给业务、开发或 QA 使用。 / Package existing inputs and decisions for stakeholders, engineering, or QA. | [模板 / Template](skills/write-decision-docs/references/template.md) · [案例 / Example](skills/write-decision-docs/references/example.md) |
| [项目汇报 / Build project briefs](skills/build-project-briefs/SKILL.md) | 要让读者快速判断进度、证据和下一步。 / Help an audience assess progress, evidence, and next steps. | [模板 / Template](skills/build-project-briefs/references/template.md) · [案例 / Example](skills/build-project-briefs/references/example.md) |
| [低打扰交互 / Design low-friction flows](skills/design-low-friction-flows/SKILL.md) | 要决定何时追问、提示和确认，以及中断后如何继续。 / Decide when to ask, confirm, or recover from failure. | [模板 / Template](skills/design-low-friction-flows/references/template.md) · [案例 / Example](skills/design-low-friction-flows/references/example.md) |

把需要的 Skill 目录完整复制到 个人 Skills 目录 `~/.codex/skills/` 或项目的 `.agents/skills/`，保留其中的 `references/`。示例中的业务与数据均为虚构。

Copy the entire folder for each skill you want into `~/.codex/skills/` for personal use or `.agents/skills/` for a project, including its `references/`. The examples use fictional scenarios and data.

```text
用 $clarify-requirements 分析这个提议。请给我本期范围、关键例外，以及会改变方案的待确认事项。

用 $write-decision-docs 把这段评审记录写成研发交接稿。保留未拍板的规则，并给 QA 可验证的预期结果。

Use $build-project-briefs to turn these QA and pilot notes into a one-page update. Tell me what belongs in speaker notes.

Use $design-low-friction-flows to redesign this failed-upload step. Show what remains on screen, what happens on retry, and when submission is blocked.
```

## 更多示例 / More examples

- [把「加个字段」拆成业务需求](examples/clarify-a-field-request.md)
- [把测试记录改成一页阶段汇报](examples/turn-test-notes-into-a-brief.md)

## License / 许可

[MIT](LICENSE) © 2026 Lucy Li
