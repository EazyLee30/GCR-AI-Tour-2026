# GCR-AI-Tour-2026

本仓库的可运行内容已整体迁移到 `Lab-01-Tech-Insights/` 目录下。

## Lab-01-Tech-Insights（你将做什么）

这是一个基于 RSS/Sitemap/HTML 的「技术动态聚合与洞察」Lab：抓取多源更新 → 归一为信号 → 聚类热点 → 生成洞察与 Markdown 报告。

你将得到：
- `report.md`：一份可阅读的技术洞察报告
- `raw_signals.json` / `clusters/hotspots.json` / `insights/insights.json`：可回放的中间产物（便于调试与复现实验）

- 入口文档：`Lab-01-Tech-Insights/README.md`
- 本地运行：先 `cd Lab-01-Tech-Insights`，再按文档执行 `./scripts/install_deps.sh` 或直接运行 `generated/tech_insight_workflow/run.py`

最短本地验证（mock，不消耗 Azure 额度）：

```bash
cd Lab-01-Tech-Insights
./scripts/install_deps.sh --python-only
python3 generated/tech_insight_workflow/run.py --mock-agents --non-interactive
```

> 说明：`.github/workflows` 仍保留在仓库根目录（GitHub Actions 规范要求）。

