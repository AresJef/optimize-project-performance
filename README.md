# optimize-project-performance

把项目提速从定位瓶颈做到交付：在真实入口跑基线，逐项试验，在同一交付工件上复验收益、正确性和回归边界。既可从头全面优化，也可续接已有实测；只要求分析时，不改代码。

## 适用场景

- **全面优化：** 盘点主要入口和代表负载，明确目标、保护项和预算，再决定哪些改动值得进入最终版本。
- **已有实测：** 核对版本、覆盖和证据，区分真实退步、已确认目标未达和仅仅证据不足。按需读取慢项优化方法，不重跑无关项。
- **只做分析：** 交付最值得查证的瓶颈、最小对照试验和停止条件。

## 安装与使用

在支持从 GitHub 安装 Skill 的宿主中，可交给安装器以下请求：

> 请从 https://github.com/AresJef/optimize-project-performance 安装 optimize-project-performance，仓库根路径是 .，固定到 v1.0.0。

也可下载 [v1.0.0](https://github.com/AresJef/optimize-project-performance/releases/tag/v1.0.0) 源码，将目录命名为 `optimize-project-performance` 并放到宿主支持的 Skill 路径。保留根目录的 `SKILL.md` 和 `references/`，不要覆盖既有同名 Skill，安装后确认宿主能发现它。

示例：

> 使用 $optimize-project-performance，只分析这个库，不改代码。基于真实使用入口找出最值得验证的瓶颈，列出基线、最小对照试验和停止条件。

完整流程见 [SKILL.md](SKILL.md)。参考文档按需读取，不要求额外安装基准工具。历史案例数值不是默认门槛。使用此 Skill 不授予测量、改代码、采用例外或发布的权限，按本次任务的授权执行。

[agents/openai.yaml](agents/openai.yaml) 仅提供 OpenAI 宿主的可选界面信息，不影响技能流程。

[MIT License](LICENSE)
