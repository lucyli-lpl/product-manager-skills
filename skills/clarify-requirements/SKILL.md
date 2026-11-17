---
name: clarify-requirements
description: "Clarify or review vague product requirements: trace them back to the real business task, resolve conflicting rules and signals, weigh scope trade-offs, and turn business feedback, bad cases, or feature proposals into actionable requirements with defaults, exceptions, and acceptance criteria. Works in English and Chinese. 中文：梳理或评审模糊产品需求，分析业务场景、规则冲突和范围取舍。适用于从业务反馈、错例或功能提议形成可执行需求。"
---

> **Language:** Respond in the user's language. If the user writes in Chinese, reply in Chinese; otherwise reply in English. 请使用用户的语言回复。

# Clarify Requirements

- Translate the requested feature back into the underlying business task. Find out who runs into what problem in which situation, how they get it done today, who uses the result, and what they use it for. Read existing materials and real examples first, and only ask questions whose answers would change the solution.
- Start with a default handling that covers the main scenario, then use real positive and negative examples to find the exceptions. When signals conflict, spell out under which conditions each source can be trusted, which conflicts are worth flagging, and how to proceed when it still can't be determined. A single bad case can reveal a gap in the rules, but how far a rule applies is decided by evidence.
- Compare reusing an existing flow, adding a local rule, and building a new capability. Put frequency, the cost of a wrong decision, the extra steps users take, and development and maintenance cost into one trade-off. For low-frequency tasks that are cheap to recover from, evaluate the existing entry points first.
- Give the current recommendation, the conditions it applies under, the explicit exceptions, and observable acceptance results. Write confirmed business definitions in directly; for points still awaiting a decision, note exactly which rule they would change. Reversible assumptions can be used in a draft first, as long as they are marked.

For example, when the business asks for a new category field, first check whether it is used for downstream search, reporting, or real-time validation. A field used for search can be collected later than one used for real-time validation, and it only needs to be triggered in the scenarios that actually require the category.

## 中文版

# 需求澄清

- 把提出的功能还原成业务任务。找出谁在什么场景遇到什么问题、目前怎么完成、结果给谁用、用来做什么。优先读已有资料和真实样例，只问答案会改变方案的问题。
- 先给覆盖主场景的默认处理，再用真实正例和反例找出例外。信号冲突时，写清各来源在哪些条件下可信、什么冲突才值得提醒、仍无法判断时如何继续。一个错例可以揭示规则缺口，规则适用范围由证据决定。
- 比较复用现有流程、局部加规则和新增能力。把频率、误判代价、用户多做的动作、研发与维护成本放进同一次取舍。低频且低成本可恢复的任务优先评估现有入口。
- 给出当前建议、适用条件、明确的例外和可观察的验收结果。确认过的业务口径直接写入，待拍板的点注明具体会改变哪条规则。可逆假设可以先用于草案并标明。

例如，业务要求新增一个分类字段时，先查它是否用于下游检索、统计或实时校验。检索字段的收集时机可以晚于实时校验字段，只有需要分类的场景才需要触发。
