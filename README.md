# 产品经理工作 Skills

一套在 Codex 中复用的产品工作方法。适合把模糊的业务请求变成可执行需求、让评审材料围绕待定事项展开，以及把项目进展讲成有证据的一页。

| Skill | 适合什么时候用 |
| --- | --- |
| [需求澄清](skills/clarify-requirements/SKILL.md) | 业务提了一个方案，想拆清真实用途、规则和本期范围。 |
| [决策型文档](skills/write-decision-docs/SKILL.md) | 要写供业务评审、开发交接或验收使用的文档。 |
| [项目汇报与信息取舍](skills/build-project-briefs/SKILL.md) | 原始材料很多，需要提炼进展、证据和下一步。 |
| [低打扰交互设计](skills/design-low-friction-flows/SKILL.md) | 要决定何时追问、何时确认，以及如何让用户继续。 |

## 在 Codex 中使用

把 `skills/` 下想用的 Skill 文件夹放到个人 Skills 目录 `~/.codex/skills/`，或放到项目的 `.agents/skills/`。保留文件夹名和其中的 `SKILL.md`。在 Codex 里可以直接指定 Skill，例如：

```text
用 $clarify-requirements 分析这条「所有申请都加归档标签」的需求。给我推荐范围，以及需要业务确认的问题。
```

```text
用 $build-project-briefs 把下面的测试记录压成一页项目汇报，注明每个数字说明什么。
```

## 示例

- [把「加个字段」拆成业务需求](examples/clarify-a-field-request.md)
- [把测试记录改成一页阶段汇报](examples/turn-test-notes-into-a-brief.md)

示例中的业务、角色和数据均为虚构。
