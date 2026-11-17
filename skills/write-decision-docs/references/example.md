# 完整案例 / Worked example

**输入。** 已确认员工可在培训报名截止前自助撤回，名额释放。承办方建议截止后也能撤回，但还没决定是否自动释放名额。旧文档只写「支持取消」。

**业务评审。** 当前请承办方决定：「截止后撤回是否释放名额？」如果释放，还需定义候补是否继续递补。负责人确认前，截止后维持人工处理。这条写在待决策表里。

**开发交接。** R-01 已确认。报名状态为「已报名」且服务端时间早于截止时间时，显示撤回入口。撤回成功后，报名状态变为「已撤回」并释放一席。同一笔重复回传只释放一次。点击时如果已经到截止时间，系统保留状态和名额并显示人工联系入口。

**验收。** 截止前撤回后，状态变化、剩余名额加一。重复回传后名额数无额外变化。截止时间到达时提交，状态和名额不变，看到人工联系入口。截止后自动释放名额的验收标为待业务决定。

---

**Input.** Staff can withdraw from training before the deadline and release their seat. The organizer is considering late withdrawals, but automatic seat release is undecided. The old document says “Cancellation supported.”

**Stakeholder review.** Ask the organizer whether late withdrawals should release a seat. If yes, confirm whether the waitlist should advance. Pending that decision, keep late withdrawals manual. Record this in the open-decision table.

**Implementation handoff.** Confirmed rule R-01. When registration is active and server time is earlier than the deadline, show Withdraw. A successful withdrawal moves registration to Withdrawn and releases one seat. Duplicate callbacks release no additional seats. If the cutoff has already passed when the action is processed, preserve registration and capacity and show a contact option.

**Acceptance.** Before cutoff, status changes and capacity increases by one. A duplicate callback leaves capacity unchanged. At cutoff, status and capacity stay the same and the user sees the contact option. Testing automatic release after cutoff depends on the organizer's decision.
