# 课程内容事实核查报告（2026-08-22）

## 结论

本轮核查发现并修正了若干会影响教学理解的实质性问题。当前版本的课程主线、核心概念和已核对论文数字总体可靠，但不应称为“零错误”或“最终完美版”：部分 2026 年阶段性研究材料、产品文档和会议状态仍具有时效性，授课前应再次核验。

## 核查范围与方法

- 对照 2026-07-04 修订版课程大纲，核对 34 学时、2 学分、17 周和行业专家 18 学时等课程信息。
- 扫描 17 讲 LaTeX 源文件中的公式、比例、实验数字、论文题名、作者、venue、DOI 和强结论。
- 优先以本地论文全文、论文表格/摘要和正式 DOI 元数据为证据，不以其他课件对同一结论的复述作为独立证据。
- 对受控实验、作者材料、系统原型、脱敏案例和课程示例分别标注证据边界。
- 对修改后的相关讲次执行两遍 XeLaTeX 编译，并渲染抽查关键修改页。

## 已确认并修正的问题

| 严重度 | 讲次 | 原问题 | 修正结果 | 核对依据 |
|---|---:|---|---|---|
| 高 | 1、2、3、5、12 | 把 TPOT 与单次相邻 Token 间隔混用，且时间线把 Prefill 结束误当作首 Token 时点 | 将平均 TPOT 定义为首 Token 后的平均每 Token 时间；把相邻 Token 间隔明确为 ITL；时间线增加“首 Token”节点 | 推理服务常用定义及本地性能材料 |
| 高 | 13 | 把查询成本直接写进信息增益 `IG(q)` 的定义 | `IG(q)` 只保留熵减少；另用 `U(q)=IG(q)-λCost(q)-μRisk(q)` 表示查询效用 | 信息论定义与决策效用分离 |
| 高 | 14 | StateFlow 的“13%/28%、5×/3×”是论文摘要的四舍五入口径，易被误解为相对百分比 | 改为表格可复算的 `+13.05 pp`、`+27.8 pp` 和约 `4.6×/2.5×` 成本倍率 | StateFlow 原文实验表 |
| 中 | 14 | 对移除 Verify 状态的结论过度外推为“适合低风险任务” | 改为准确消融：SQL 成功率 63.73%→62.28%，成本 3.82→3.68；明确不能据此取消生产终态 Oracle | StateFlow 消融表 |
| 高 | 8 | CauseLens 首作者被误写为 Tan | 全部改为 Qihan Liu / Liu et al.，补 DOI | IEEE/Crossref DOI 10.1109/IWQOS65803.2025.11143407 |
| 中 | 4、5、7、8、11、16 | TELLER 的首作者或题名/状态不统一 | 统一为 Xu et al.，正式题名为 *TELLER: Non-intrusive Cross-Layer Root-Cause Analysis for LLM Inference*，标注 ASE 2026 已录用 | 本地 TELLER 论文全文 |
| 中 | 8、12、13 | AgentChaos 题名/实验口径不统一 | 统一正式题名；把约 49.66% 写成“最大约 50 个百分点”，诊断数字分别对应类型和步骤 | 本地 AgentChaos 论文全文 |
| 高 | 17 | RCACopilot 的正式题名和 Table 3 数字不准确，“全量输入”被笼统写成不稳定 | 改为正式题名 *Automatic Root Cause Analysis via Large Language Models for Cloud Incidents*；补全 `.689/.510`、`.766/.533`、`.440/.349` | EuroSys 2024 论文全文 Table 3 |
| 高 | 17 | MetaRCA 把摘要总体优势与生产表格结果混成同一个结论，且 CIRCA 的 @3 数据缺失 | 区分生产集 AC@1 相对 CIRCA 的 28/42 个百分点，与摘要总体 29/48 个百分点；补齐表格 | FSE 2026 论文全文摘要与 Table 3 |
| 中 | 17 | AIOpsLab 论文作者归属写错 | 改为 Shetty et al. | 本地 AIOpsLab 论文全文 |
| 中 | 17 | AgentTrace-RCA 使用非正式简称，出处不完整 | 改为正式题名 *AgentTrace: Causal Graph Tracing for Root Cause Analysis in Deployed Multi-Agent Systems*，标注 ICLR 2026 Workshop | 本地论文全文 |

## 已复核的代表性数字

- TELLER：水平/垂直 Step F1 为 0.916/0.900；事件压缩率 83.88%；论文报告追踪墙钟开销约 +9.8%。
- AgentChaos：最高 pass@1 下降 49.66%；LLM 调用量变化 0.71×–4.24×；类型/步骤诊断约 52.45%/55.5%。
- Mint：传统采样查询 miss 27.17%；平均存储和网络占完整追踪基线 2.7%/4.2%。
- WorkArena++：682 项任务；93.9% 与 2.1% 的人类/GPT-4o 比较只对应相同的 98 任务子集，课件已保留限定。
- TapeAgents：学生 Agent 66.2%→77.5%，教师 93.1%，训练使用 1,000 条 Tape。
- Minder：平均反应时间 3.6 秒，Precision 0.904，F1 0.893。
- Aegis：诊断造成的 idle time 降低超过 97%，restart 减少 84%，性能退化降低 71%。
- FLARE：延迟开销 0.43%，生产回归 true-positive diagnostic accuracy 81.8%，部署规模超过 6,000 GPU、持续 8 个月以上。
- StriaTrace：相对替代方案 tracing overhead 降低 97.8%；论文报告诊断 19 类根因和数百个异常，不能把该相对降幅解释成绝对 overhead=2.2%。
- AgentTrace：550 个合成场景、10 个领域、每条 8–15 个动作；Hit@1 94.9%、Hit@3 98.4%、平均分析 0.12 秒，结论仅适用于其单根因和结构化日志设定。

## 尚未完全独立核验的风险

以下内容目前不能认定“有错”，但证据强度低于已拿到正式论文全文的条目：

1. OpsLens、WeRCA、AgentTracer 的部分 2026 实验数字主要来自作者/项目材料或阶段性论文版本。课件已保留“论文/作者材料中的条件化结果”及外部有效性限制；最终 proceedings 上线后应再核一次题名、页码和数字。
2. AgenticSRE、OpsLoop 界面和案例是系统原型/脱敏教学案例，不是同行评审论文的通用生产结论。
3. Langfuse、vLLM、OpenTelemetry GenAI、Grafana/Loki 等文档会随版本变化；当前内容按 2026-08 的材料组织，开课前需按实际部署版本复核指标名和生命周期状态。
4. Antithesis、Clockwork 只用于解释公开产品定位，课件未写未经核实的性能数字；官网表述变化时需同步更新。
5. 课程中自行构造的数值案例均应继续标为“教学示例”，不能与论文实验或企业生产结果混用。

## QA 结果

- 已重新编译本轮涉及的 13 个讲次：01、02、03、04、05、07、08、11、12、13、14、16、17。
- 所有编译均成功，无 LaTeX fatal error、未定义命令或 Overfull box。
- 日志中仍有少量 Underfull box，属于表格/段落的松散排版提示，不造成文本被裁切。
- 已渲染抽查 TPOT/ITL、CauseLens 参考文献、信息增益、StateFlow、RCACopilot、MetaRCA、AIOpsLab 和 AgentTrace 等关键修改页，未发现新增遮挡或裁切。

## 授课前建议

- 对所有标注“2026 已录用/阶段性版本”的论文做一次 proceedings 级元数据复核。
- 使用真实实验环境时，以实际 vLLM/OTel/Langfuse 版本的指标名替换教学示意名。
- 不删除页面上的“受控实验”“单服务”“合成场景”“作者材料”“教学示例”等限定语；这些限定是结论正确性的一部分。

