# 交互流程与异常规格 / Interaction flow and recovery spec

**用户目标和当前状态 / User goal and starting state** — [用户正做什么？已输入或确认什么？ / What is the user doing and what have they entered or confirmed?]

| 触发与范围 / Trigger and scope | 何时介入及为何 / Timing and reason | 界面与用户动作 / UI and user action | 状态变化及恢复 / State change and recovery |
| --- | --- | --- | --- |
| [主路径 / Main path] | [直接继续 / 就近提醒 / 集中补问 / 明确确认 / Proceed, inline cue, focused prompt, or confirmation] | [用户实际看到和能做什么 / What the user sees and can do] | [保存、撤销或返回后的结果 / Saved state, undo, or return behavior] |
| [关键异常 / Consequential exception] | [误操作的成本、是否可撤回 / Cost and reversibility of error] | [发生了什么、一个明确下一步 / What happened and one clear next action] | [失败时保留什么，何时算成功 / State preserved on failure and what counts as success] |

按相关性验收 / Check only relevant states: 已填 / 空白 / 已确认无；单一目标 / 多个目标；失败、重试及返回；不可逆操作。
Test entered, blank, and confirmed-none states when applicable; single vs. ambiguous target; failure, retry, return; and irreversible actions.
