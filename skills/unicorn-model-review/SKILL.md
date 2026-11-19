---
name: unicorn-model-review
description: |
  用 Takumi Tominaga 的 Unicorn Model（独角兽模型）复盘历史图表，核对扫单、结构转换及 Breaker 与 FVG 的重叠，审阅该模型的执行、仓位与回测日志。
metadata:
  cangjie.generated-by: cangjie-tools v2.5.0
  cangjie.variant: single
  cangjie.bundle-id: bundle.unicorn
  cangjie.capability-count: 5
  cangjie.entrypoint-count: 1
---
# The Unicorn Model — 全书能力入口

## 触发与不触发

**适用**：与本书能力域相关的咨询与任务（见下方路由表的意图列）。
**不适用**：
- 从书中示例推算策略胜率或给出实时买卖指令。

## 核心原则（常驻速览，概览类问题读到这里即可回答）

1. 先写复盘截止时刻。每个判断列出支持它的价格、周期或图中位置。
2. 按请求读取相应卡。完整案例依次给出背景、形态、执行、风险与复盘记录。
3. 区分作者示例、用户预设、已发生事件和信息缺口。

## 能力路由（先读本表，按意图加载 1 张能力卡）

| 用户意图 | 先读 | 补读/备注 |
|---|---|---|
| 判断候选处于哪个参考区间，是否有逆向障碍 | references/capabilities/context.md | references/capabilities/setup.md |
| 按事件顺序验证扫单与位移，并计算 Breaker 和 FVG 的重叠区 | references/capabilities/setup.md | references/capabilities/context.md、references/capabilities/execution.md |
| 从确认后的回踩逐步判读成交、失效、分批止盈和余仓 | references/capabilities/execution.md | references/capabilities/setup.md、references/capabilities/risk.md |
| 按用户给定的账户与合约参数计算模拟仓位及组合约束 | references/capabilities/risk.md | references/capabilities/execution.md |
| 用同一品种的逐笔记录评估保本时机、执行偏差和样本缺口 | references/capabilities/journal.md | references/capabilities/execution.md、references/capabilities/risk.md |

**非能力类查询**：
- 书名/作者/章节/整书概览 → references/overview.md
- 术语解释 → references/glossary.md
- 决策规则速查（不需要原文依据时） → references/cheatsheet.md
- 完整意图与关键词索引（本表未覆盖的意图先查这里） → references/capability-index.md

## 加载规则

- 每次任务先读本文件，再按路由表加载 **1** 张能力卡；任务明确跨域时最多加载 2 张。
- 概览/书名类问题不加载能力卡，用「核心原则」与 overview.md 回答。
- 路由表与 capability-index.md 都无法命中的意图，明确告知超出本书范围，不要硬套。

## 边界与判停

- 无法确定时序、价格边界或合约规格时，指出待补字段，完成仍有证据的部分。
