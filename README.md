# Optimize Project Performance

这套工具提供三个 Codex Skill，可按任务选择入口。要交付一个经过实测的优化版本，从主入口开始：需要测量时转入测量专项，选定版本仍有已证实的退步或未达已确认目标时转入差距诊断。同一任务在入口之间切换时，沿用原项目记录、预算和复测次数。

## 选择入口

| Codex 显示名与入口文件 | 使用示例 |
| --- | --- |
| [Optimize Project Performance](skills/optimize-project-performance/SKILL.md) | 使用 `$optimize-project-performance` 为这个项目提速，在同一个最终版本上验证收益、功能和相邻入口。 |
| [Noise-Resilient Benchmarking](skills/noise-resilient-benchmarking/SKILL.md) | 使用 `$noise-resilient-benchmarking` 比较 A、B 两版在同一负载下的耗时，并说明机器波动会怎样影响结论。 |
| [Diagnose Performance Gaps](skills/diagnose-performance-gaps/SKILL.md) | 使用 `$diagnose-performance-gaps` 分析这份最终版本的慢项表，指出哪些方案值得试、哪些可以停止，以及理由。 |

「可独立调用」指可以直接从任一入口开始，不必先运行主 Skill。例如，只需要设计或复核跑分，就直接调用测量入口；已有实测差距，只需要查原因，就直接调用诊断入口。若诊断还需要补测或进入选版，它会用到对应的专项或主入口。要跑完整优化流程，请从同一标签或提交安装三个 Skill，不要混用版本。

直接从本地使用时，让 Agent 读取上表对应的入口文件；如需其他入口，沿用同一份本地文件树。只要求分析或设计测量时，交付判断、方案和停止条件。改动代码、采集数据、采用例外和发布沿用任务本身的授权。历史案例中的数值只适用于对应案例。

## 安装

把下面这句话发给 Codex：

> 请用 `$skill-installer` 安装 [AresJef/optimize-project-performance](https://github.com/AresJef/optimize-project-performance) 中 `skills/` 下的三个 Skill：`optimize-project-performance`、`noise-resilient-benchmarking`、`diagnose-performance-gaps`。三个都使用同一标签或提交。

[MIT License](LICENSE)
