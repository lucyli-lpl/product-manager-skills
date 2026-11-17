---
name: write-decision-docs
description: "Write or rewrite PRDs, decision tables, rule specs, and project docs built for decisions: business review, cross-team alignment, engineering handoff, or acceptance testing. Organizes content by what each reader must confirm, build, or test. Works in English and Chinese. 中文：编写或改写供评审、跨团队对齐、开发交接或验收使用的 PRD、决策表、规则说明和项目文档。"
---

> **Language:** Respond in the user's language. If the user writes in Chinese, reply in Chinese; otherwise reply in English. 请使用用户的语言回复。

# Decision-Oriented Docs

- First decide what the reader needs to do after reading. For business review, highlight the scenarios, definitions, and choices to be confirmed. For engineering handoff, state the trigger conditions, actions, resulting state or data, and exception paths. For acceptance materials, give the test scenarios, observable results, and the scope of this round.
- Organize by the actual workflow. If two kinds of questions need to be confirmed by different people, or rest on different grounds, split them into separate sections or tables by decision topic. Give similar scenarios their own row only when the handling, evidence, or acceptance result differs.
- Use a short table for the same kind of choice, keeping only the columns the reader actually needs. Prefer giving one concrete example with its expected result. When order matters, use a short flow or one continuous paragraph.
- Make clear what is a confirmed rule, what is the current recommendation, and what is still to be confirmed. For open items, state the choice to be made and its impact, and cite the source when a definition already exists. When updating an existing doc, write the decision back into the relevant sections and add a change-log entry as needed.
- Before delivering, read it once from the target reader's point of view. Readers should quickly find what they need to confirm, build, or test, and know how to judge when it's done.
- Use stable rule IDs when engineering and QA need to trace decisions across separate documents. Give acceptance checks observable outcomes. Mark an unassigned decision owner as TBD.

For example, a table for the business to check scope can keep just "Scenario, Applicable rule, Example, Open question." Field-level details for implementation and testing can go in the corresponding delivery materials.

## Resources

- Use the [copyable template](references/template.md) for structured deliverables. Keep the fields the current audience needs.
- Read the [worked example](references/example.md) to see how the inputs lead to an output and how it handles missing evidence or exceptions.

## 中文版

# 决策型文档

- 先判断读者看完要做什么。业务评审突出要确认的场景、口径和选择。开发交接写明触发条件、处理动作、状态或数据结果、异常路径。验收材料给出测试场景、可观察结果和本轮范围。
- 按实际工作流组织。如果两类问题要由不同的人确认，或依据不同，按决策主题拆节或拆表。只有处理方式、证据或验收结果发生变化时，才为相似场景单独占一行。
- 对同一类选择用短表，列只保留读者要用到的信息。优先给一条具体示例和预期结果。需要说明前后顺序时用短流程或一段连续描述。
- 明确已确认规则、当前建议、待确认事项。对待确认项写清要确认的选择及其影响，已有定义时引用来源。更新现有文档时，把决定写回相关章节，按需要补一条变更记录。
- 交付前从目标读者视角读一遍。读者应能快速找到自己该确认、实现或测试的事项，并知道用什么判断完成。
- 研发和 QA 需要在多份文档间追溯时，复用稳定的规则 ID。验收写明可观察的结果。待决项尚无负责人时，标记为待定。

例如，面向业务核对适用范围的表可以只保留「场景、适用规则、例子、待确认点」。实现和测试用的字段级细节可放在相应交付材料中。

## 配套资料

- 需要正式交付稿时，按任务使用[可复制模板](references/template.md)，保留当前读者用得到的栏目。
- 对产出粒度或取舍不确定时，查看[完整案例](references/example.md)，了解原始输入如何变成可用的结果。
