# 完整案例 / Worked example

> Fictional scenario / 虚构场景

**输入。** 支持团队提出「所有订单加一个必填的配送备注」。回看 20 条配送失败工单，7 条涉及门禁，且都来自需要门禁的楼宇。配送员在派单后查看进楼说明，普通地址无需补充。调研尚未覆盖门禁状态未知的地址。

**产出。** 本期复用地址编辑页。确认需要门禁的地址，在下单前补充进楼说明。普通地址可直接下单。门禁状态未知时，可先让用户选择「需要门禁 / 不需要 / 不确定」。选「不确定」时按现有下单流程继续，把门禁状态标为未知。先验证哪些地址可由现有数据可靠判断，再决定是否预填。配送员在派单后能看到说明。门禁信息的可见范围由配送团队确认后再定。

**验收。** 对需要门禁的地址，填入说明并下单，接单配送员可见。普通地址无补填步骤。状态未知时保留选择结果，避免下次无故重复问；如果地址发生变化，重新判断。

**取舍。** 7 条工单足以证明存在这个问题，但样本来自失败订单，无法推断整体发生率。建议把新增负担集中在有需要的人群，先验证判定是否可靠。

---

**Input.** Support proposes a required delivery note for every order. Seven of 20 reviewed failed-delivery tickets involve building access, all at access-controlled addresses. Couriers use instructions after assignment. Ordinary addresses require no extra information. Addresses with unknown access status haven't been studied.

**Output.** Reuse the address editor. Ask for instructions before order placement when an address is known to require access. Let ordinary addresses proceed. Where access status is unknown, offer “Access required / Not required / Unsure.” An unsure answer follows the existing checkout flow and records the status as unknown. Confirm where existing data can reliably determine status before introducing prefills. Show instructions after courier assignment. Treat who else may view them as an open decision for the delivery team.

**Acceptance.** A courier assigned to an access-controlled address sees the submitted instructions. An ordinary address proceeds with no additional step. Store the user's selection for unknown status and reassess if the address changes.

**Trade-off.** Seven tickets establish that the problem exists. A sample restricted to failures cannot establish its population-wide frequency. Target the affected users and validate how reliably they can be identified.
