# 能力索引（完整版）

| capability_id | 标题 | 重要度 | 意图 | 关键词 | 能力卡 |
|---|---|---|---|---|---|
| cap.unicorn.context | 标注区间和高周期背景 | high | 判断候选处于哪个参考区间，是否有逆向障碍 | HTF、折价、溢价、流动性、时段 | capabilities/context.md |
| cap.unicorn.setup | 验证独角兽形态 | high | 按事件顺序验证扫单与位移，并计算 Breaker 和 FVG 的重叠区 | 独角兽、Unicorn、Breaker、FVG、MSS、扫单 | capabilities/setup.md |
| cap.unicorn.execution | 回放入场和分批退出 | high | 从确认后的回踩逐步判读成交、失效、分批止盈和余仓 | 回踩、结构止损、TP1、TP2、保本 | capabilities/execution.md |
| cap.unicorn.risk | 折算仓位并核对风险额度 | high | 按用户给定的账户与合约参数计算模拟仓位及组合约束 | 每点价值、手数、敞口、相关性、日损 | capabilities/risk.md |
| cap.unicorn.journal | 审阅日志与退出规则 | high | 用同一品种的逐笔记录评估保本时机、执行偏差和样本缺口 | 复盘、日志、截图、回测、分批退出 | capabilities/journal.md |
