# Unicorn Model Review

用于复盘历史图表的中文 Codex Skill，依据 Takumi Tominaga 的《The Unicorn Model》（2026）整理。给它一张带品种、周期和截止时刻的历史图表，它会核对先扫哪个高低点、哪次位移改变了结构，以及 Breaker 和该次位移产生的 FVG 在哪些价格上重叠。

## 安装

下载并解压仓库，将 `skills/unicorn-model-review` 整个目录复制到个人的 `~/.agents/skills/`，或放进项目的 `.agents/skills/`。保留 `SKILL.md` 与同级 `references/` 的目录结构。

## 示例

附上图表或按时间排列的 OHLC 数据，然后输入：

> 用 $unicorn-model-review 复盘这段行情。只用当时已收盘的 K 线，列出扫单、结构突破及 FVG 形成的时间，计算它与 Breaker 的交集。分别标记形态确认和首次回踩的时刻。

五张能力卡分别处理高周期背景、形态识别、入场与分批退出、仓位风险和交易日志。复盘会区分可见价格、模拟成交假设和缺失证据。原书案例用于演示判读过程，策略胜率仍需独立数据检验。

[Skill 入口](skills/unicorn-model-review/SKILL.md) · [能力索引](skills/unicorn-model-review/references/capability-index.md)
