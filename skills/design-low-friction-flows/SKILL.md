---
name: design-low-friction-flows
description: "Design or review forms, conversational flows, business processes, and error or edge-case interactions with minimal friction: decide when to ask, when to confirm, and how to cut steps and interruptions. Works in English and Chinese. 中文：设计或评审表单、对话、业务流程与异常交互。适用于判断何时追问、何时确认以及如何减少操作与打断。"
---

> **Language:** Respond in the user's language. If the user writes in Chinese, reply in Chinese; otherwise reply in English. 请使用用户的语言回复。

# Low-Friction Interaction Design

- Start from the task the user is trying to complete: pin down the current state, the information already at hand, and the next step. Prefer finishing the action where the original task happens, and keep whatever the user has already entered or confirmed.
- Choose how strong an interaction should be based on frequency, the cost of interrupting, the cost of a mistake, and whether it can be undone. When confidence is high and the result can be corrected, prefill or just continue. When something important is missing required information, ask once, all together, before it's used. For high-impact actions, give a clear chance to confirm.
- When information is missing, ask only for the one thing needed right now. Distinguish "not filled in yet" from "the user confirmed there is none," and for the latter offer an explicit option when the business allows it. When there is only one clear target, act on it directly; when there are several and it's unclear which is meant, ask for the choice right where it happens.
- For waits, failures, and conflicts, explain what happened and give one clear next step. Before and after an update, check whether drafts, manual edits, and existing confirmations are still valid. Keep the user's valid input when retrying.
- Deliver the design as trigger conditions, UI changes, user actions, results, and recovery paths. Walk through the one or two scenarios most likely to be misunderstood, and provide mockups only as actually needed.
- For partial success, identify exactly which items are retried and how already-completed items are treated. Define when a replacement becomes effective and which inputs survive failure or a return to the draft.

For example, if only one type of application needs an archive tag filled in, collect it right before that type of application is used. If having no tag is allowed, offer a "None this time" option and save the confirmed result.

## Resources

- Use the [copyable template](references/template.md) for structured deliverables. Keep the fields the current audience needs.
- Read the [worked example](references/example.md) to see how the inputs lead to an output and how it handles missing evidence or exceptions.

## 中文版

# 低打扰交互设计

- 从用户正在完成的任务出发，定位明确的当前状态、手头已有信息和下一步。优先在原任务位置完成操作，保留用户已经填写或确认的内容。
- 用频率、打断成本、误操作代价和可撤回来选择交互强度。高置信且可纠正时可预填或直接继续，重要但缺少必要信息时在使用前集中问一次，影响重大的操作给出明确的确认机会。
- 缺信息时只问当前需要的一件事。区分还没填和用户确认没有，后者在业务允许时提供明确选项。只有一个可确定目标时可直接操作，多个目标且指向不明时就近选择。
- 对等待、失败和冲突，说明发生了什么并给一个明确下一步。更新前后检查草稿、手工修改和已有确认是否仍然有效。重试时保留用户的有效输入。
- 交付可用触发条件、界面变化、用户动作、结果和恢复路径描述。用最易误解的一两个场景走一遍，交互稿按实际需要提供。
- 出现部分成功时，写清重试哪些项目、已成功项如何处理。明确替换何时生效，以及失败或返回草稿时保留哪些输入。

例如，只有某类申请需要补填归档标签时，可在该类申请使用前就近收集。允许没有标签时，提供「本次没有」选项并保存已确认的结果。

## 配套资料

- 需要正式交付稿时，按任务使用[可复制模板](references/template.md)，保留当前读者用得到的栏目。
- 对产出粒度或取舍不确定时，查看[完整案例](references/example.md)，了解原始输入如何变成可用的结果。
