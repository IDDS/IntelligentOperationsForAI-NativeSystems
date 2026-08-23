# 面向 AI 原生系统的智能运维 - LaTeX 课件

## 2026-08-23 课程级优化

- 17 讲封面统一为“陈鹏飞｜中山大学”。
- 正文按论文、系统原型或脱敏案例引用，不再出现主讲人姓名或内部项目执行文件名。
- 新增 `COURSE-OPTIMIZATION-GUIDE.md`，明确每讲唯一主问题、上下游产物、跨讲边界和两学时授课策略。
- 新增 `MATERIALS-ANALYSIS-WEEK-01.md`，补齐第 1 讲的任务合同、来源登记、证据边界和 QA 记录。
- 第 11、17 讲新增“课堂主线与拓展阅读”页：完整 PDF 继续作为研究型讲义，课堂只沿主线选择讲解。
- 已完成一轮课程级事实核查并修正 TPOT/ITL、信息增益、论文元数据和实验结论口径；详见 `CONTENT-AUDIT-2026-08-22.md`。
- 已继续审校第 2–17 讲：补充案例/结果/边界 QA 记录，修正第 9 讲字体警告，并校正第 17 讲材料记录的最终页数为 154 页。

## 文件

- `AI-Native-AIOps-2026-Week-01.tex`：第 1 讲源文件。
- `AI-Native-AIOps-2026-Week-01.pdf`：编译后的 102 页授课 PDF；新增大模型基础、Transformer/后训练/推理模型、采样参数、Agent/ReAct/状态机/记忆/多智能体/评测等教学单元，并保留生产级 LLM Serving 与 Agent 工程架构总览页。
- `AI-Native-AIOps-2026-Week-02.tex`：第 2 讲源文件。
- `AI-Native-AIOps-2026-Week-02.pdf`：编译后的 72 页授课 PDF。
- `AI-Native-AIOps-2026-Week-03.tex`：第 3 讲源文件。
- `AI-Native-AIOps-2026-Week-03.pdf`：编译后的 89 页授课 PDF。
- `AI-Native-AIOps-2026-Week-04.tex`：第 4 讲源文件。
- `AI-Native-AIOps-2026-Week-04.pdf`：编译后的 90 页授课 PDF。
- `AI-Native-AIOps-2026-Week-05.tex`：第 5 讲源文件。
- `AI-Native-AIOps-2026-Week-05.pdf`：编译后的 94 页授课 PDF。
- `AI-Native-AIOps-2026-Week-06.tex`：第 6 讲源文件。
- `AI-Native-AIOps-2026-Week-06.pdf`：编译后的 92 页授课 PDF。
- `AI-Native-AIOps-2026-Week-07.tex`：第 7 讲源文件，覆盖调用链分析、HotSpot 风格多维归因、决策树/规则挖掘、Nezha、ChangeRCA、TELLER 与实验 2。
- `AI-Native-AIOps-2026-Week-07.pdf`：编译后的 92 页授课 PDF。
- `AI-Native-AIOps-2026-Week-08.tex`：第 8 讲源文件，覆盖因果语言、时间序列因果、CauseInfer、CauseLens、AI 系统六层故障特征、LLMRCA、AgentChaos、Langfuse 类调用链与三个贯穿案例。
- `AI-Native-AIOps-2026-Week-08.pdf`：编译后的 101 页授课 PDF。
- `AI-Native-AIOps-2026-Week-09.tex`：第 9 讲源文件，覆盖运维数字分身、自治阶梯、ReAct、StateFlow、TapeAgents、工具契约、SOP、HITL、OpsLens、WeRCA、AlertGuardian、AgentTracer、AgenticSRE 与三个综合案例。
- `AI-Native-AIOps-2026-Week-09.pdf`：编译后的 104 页授课 PDF。
- `AI-Native-AIOps-2026-Week-10.tex`：第 10 讲源文件，覆盖大型客户转型难点、AIOps/LLMOps/AgentOps 能力演进、场景选择、阶段门、数据治理、平台边界、组织协同与持续运营。
- `AI-Native-AIOps-2026-Week-10.pdf`：编译后的 100 页授课 PDF。
- `AI-Native-AIOps-2026-Week-11.tex`：第 11 讲源文件，覆盖企业级 AIOps 平台总体架构、数据平面/控制平面、对象与事件模型、数据流、监控/告警/自动化/配置/知识/故障处置能力分层、蓝鲸式工程实践，以及异常检测、告警聚合、事件排序和动作门禁算法；新增 NSDI 2025 Minder、ASE 2025 AlertGuardian、FSE 2024 ChangeRCA、ASE 2026 TELLER 等论文剖面。
- `AI-Native-AIOps-2026-Week-11.pdf`：编译后的 130 页授课 PDF；新增两学时课堂主线与拓展阅读分层。
- `AI-Native-AIOps-2026-Week-12.tex`：第 12 讲源文件，覆盖模型网关、推理运行时、RAG/证据数据平面、Agent Runtime、工具与记忆、Langfuse/OTel 可观测性、评测、成本、安全和综合架构。
- `AI-Native-AIOps-2026-Week-12.pdf`：编译后的 102 页授课 PDF；每个主要方法均按“问题—机制—结果—解释—边界—工程结论”展开，并补充 OSDI 2026 StriaTrace 的在线推理关键路径追踪与诊断。
- `AI-Native-AIOps-2026-Week-13.tex`：第 13 讲源文件，覆盖 RCA Agent 任务合同、状态机、工具契约、证据矩阵、候选排序、信息增益、反证、审批、回滚、终态验证、记忆、故障注入和实验评测。
- `AI-Native-AIOps-2026-Week-13.pdf`：编译后的 97 页授课 PDF；包含课程案例工作台、WeRCA、AgentTracer、LLMRCA、AgentChaos、OpsLens 的结果与边界解释。
- `AI-Native-AIOps-2026-Week-14.tex`：第 14 讲源文件，覆盖自然语言 Intent Contract、Workflow DSL、状态图、ReAct/StateFlow/TapeAgents、审批/回滚/Oracle、WorkArena++ 结果，以及 Antithesis 确定性测试和 Clockwork GPU 资源控制回路案例。
- `AI-Native-AIOps-2026-Week-14.pdf`：编译后的 94 页授课 PDF；每个主要方法均按“问题—机制—结果—解释—边界—工程结论”展开，工业界案例采用官网公开定位与 LaTeX/TikZ 教学重绘。
- `AI-Native-AIOps-2026-Week-15.tex`：第 15 讲源文件，覆盖 AI Native 对象宇宙、多源抽取、UniversalNER/Jellyfish、实体对齐、Kubernetes/Backstage/OTel/OpenLineage 关系、profiling 与近期 SIGCOMM/NSDI AI 集群观测/故障定位专题。
- `AI-Native-AIOps-2026-Week-15.pdf`：编译后的 117 页授课 PDF；前置增加多智能体概念、架构、消息契约与 Memory 一致性，并把 OSDI 2025 Neutrino/What-if、NSDI 2025 Aegis、NSDI 2026 FLARE 分布到 profiling 与 AI 集群关系证据专题；正文按对象档案、实体对齐和关系证据组织，不重复第 17 讲调查算法。
- `AI-Native-AIOps-2026-Week-16.tex`：第 16 讲源文件，覆盖告警解析、Canonical Event、去重/归并、事件图、影响关联、对象级 Episode Memory、摘要与记忆治理，并深入讲解 COLA、iPACK、Oasis、ESRO、AlertGuardian。
- `AI-Native-AIOps-2026-Week-16.pdf`：编译后的 105 页授课 PDF；增加 NSDI 2024--2026、OSDI 2025、SIGCOMM 2024--2025 的 AI 集群深层观测与故障事件专题，并通过 LLM 推理服务贯穿案例连接训练、推理、网络和 Agent 事件。
- `AI-Native-AIOps-2026-Week-17.tex`：第 17 讲源文件，覆盖 Investigation Contract、Evidence Bundle、竞争性假设、贝叶斯/信息增益查询、多 Agent 调查板、AgentTrace、GPU kernel/训练/推理/网络证据分辨率阶梯、完整 TTFT RCA 案例、评测、实验与综合考核。
- `AI-Native-AIOps-2026-Week-17.pdf`：编译后的 154 页完整讲义 PDF；新增两学时课堂主线，融合 OSDI 2025 Neutrino/What-if Straggler、NSDI 2025 Aegis、NSDI 2026 FLARE、OSDI 2026 StriaTrace、NSDI 2024 NetAssistant，以及 RCACopilot、Xpert、AIOpsLab、MetaRCA、OpsLens、AgentTrace 和 RCA Agent 失败研究。
- `ads-beamer-theme.sty`：从高级分布式系统模板适配的主题。
- `assets/`：论文图示裁剪与课件素材。
- `MATERIALS-ANALYSIS.md`：材料盘点、论文分析和采用矩阵。
- `COURSE-OPTIMIZATION-GUIDE.md`：17 讲课程主线、去重边界、页数策略、论文讲解模板与 QA 门槛。
- `CONTENT-AUDIT-2026-08-22.md`：17 讲内容事实核查、已修正问题、已复核数字、未决风险和编译/视觉 QA 记录。
- `MATERIALS-ANALYSIS-WEEK-01.md`：第 1 讲材料分析、来源登记、教学叙事和图片使用规则。
- `MATERIALS-ANALYSIS-WEEK-02.md`：第 2 讲材料分析、教学叙事和图片使用规则。
- `MATERIALS-ANALYSIS-WEEK-03.md`：第 3 讲论文、项目、代码和官方资料的逐段采用说明。
- `MATERIALS-ANALYSIS-WEEK-04.md`：第 4 讲日志、Trace、研究论文、版本校正和实验设计的证据登记。
- `MATERIALS-ANALYSIS-WEEK-05.md`：第 5 讲 GPU、Token、质量、成本、Langfuse、RAG/Agent 和实验设计的证据登记。
- `MATERIALS-ANALYSIS-WEEK-06.md`：第 6 讲时序异常检测、生产评测、告警降噪、论文证据和实验设计的登记。
- `MATERIALS-ANALYSIS-WEEK-07.md`：第 7 讲任务合同、议题树、竞争性假设、论文/项目材料证据登记、图像来源和实验 2 设计。
- `MATERIALS-ANALYSIS-WEEK-08.md`：第 8 讲任务合同、关键情报问题、竞争性假设、CauseInfer/CauseLens/LLMRCA/AgentChaos 证据登记、AI 六层特征矩阵与视觉 QA 说明。
- `MATERIALS-ANALYSIS-WEEK-09.md`：第 9 讲任务合同、关键问题、论文与项目材料证据登记、独立裁切图清单、案例脚本和视觉 QA 门槛。
- `MATERIALS-ANALYSIS-WEEK-10.md`：第 10 讲任务合同、转型关键问题、项目调研与阶段性架构材料登记、场景阶段门、案例脚本和视觉 QA 门槛。
- `MATERIALS-ANALYSIS-WEEK-12.md`：第 12 讲大模型平台架构的材料登记、论文主线、结果/结论页映射和视觉 QA 门槛。
- `MATERIALS-ANALYSIS-WEEK-13.md`：第 13 讲 RCA Agent 开发实战的材料登记、任务合同、论文结果、实验设计和视觉 QA 门槛。
- `MATERIALS-ANALYSIS-WEEK-14.md`：第 14 讲流程编排的材料登记、StateFlow/TapeAgents/WorkArena++ 结果、Antithesis/Clockwork 工业界案例、引用边界和视觉 QA 门槛。
- `MATERIALS-ANALYSIS-WEEK-15.md`：第 15 讲对象档案、实体对齐、关系构建、AI Native 可观测性、近期 SIGCOMM/NSDI 论文证据与图像使用规则。
- `MATERIALS-ANALYSIS-WEEK-16.md`：第 16 讲任务边界、事件处理链、论文证据与结果、会议专题、案例、实验及图像使用规则。
- `MATERIALS-ANALYSIS-WEEK-17.md`：第 17 讲调查任务、关键问题、论文证据/结果/局限、证据分辨率阶梯、贯穿案例、实验设计、图片采用和视觉 QA 登记。
- `visuals/course-knowledge-graph.svg/png/pdf`：课程六层知识图谱与 17 周递进路径。
- `visuals/course-poster.svg/png/pdf`：课程宣传海报，适合公众号、课程介绍页和打印使用。
- `visuals/course-knowledge-graph-v2.svg/png/pdf`：分层点—边知识图谱；显式标注系统对象、观测证据、诊断控制、可验证产物及反馈迭代关系。
- `visuals/course-poster-v2.svg/png/pdf`：信息密度更高的课程宣传海报；包含课程规模、五个生产问题、六条能力主线、17 周路线、研究案例与技术栈。
- `visuals/course-knowledge-graph-master-v3.svg/png/pdf`：教学主图版；六大知识域、48 个核心节点、17 周学习路径及论文/系统案例锚点，适合 A0 打印或课堂投影。
- `visuals/course-knowledge-graph-ontology-v4.svg/png/pdf`：Ontology 风格主图；以 Model、Serving Runtime、Compute Fabric、Agent Workflow、Evidence/Event、Policy/SLO、Investigation、Outcome/Memory 为中心对象，加入图标、关系边、状态标签、行动轨道和 17 周映射。
- `visuals/course-knowledge-graph-course-v5.svg/png/pdf`：课程内容校正版；保留对象关系、图标和行动轨道的视觉语言，但标题恢复为“面向 AI 原生系统的智能运维”，并明确展示可观测性、AI 原生系统对象、AgentOps、安全闭环、17 周路线及论文专题。
- `visuals/course-knowledge-graph-true-v6.svg/png/pdf`：Neo4j 风格实体—关系图；节点表示课程实体，边表示 calls、trains、deployed_as、observes、forms、diagnoses、verifies、learns_from 等关系，颜色区分系统/模型、运行时/基础设施、证据/事件、诊断和治理/动作。
- `visuals/course-knowledge-graph-neo4j-v7.svg/png/pdf`：Neo4j 风格交付命名版；采用真实网络图结构，适合继续导入图数据库或作为课程宣传主图。
- `visuals/course-knowledge-graph-concepts-v8.svg/png/pdf`：课程概念关系图最终版；节点是 7 个知识域中的可讲授概念/方法/案例，中心主线为“系统概念 → 观测证据 → 检测与定位 → 因果诊断 → Agent 化运维 → 运行时治理 → 验证与知识闭环”，边显式区分先修、观测、检测、诊断、治理、验证、沉淀和案例关系。
- `visuals/course-knowledge-graph-neo4j-v8.svg/png/pdf`：同一张课程概念关系图的 Neo4j 风格命名版，便于后续导入图数据库或在课程材料中引用。
- `visuals/course-knowledge-graph-entity-v10.svg/png/pdf`：参考高级分布式系统实体关系图重排的最终版；采用中心课程实体、周边知识实体/方法/证据/治理节点和 17 周覆盖条，补齐训练、推理、RAG、多智能体、Serving、GPU/网络、事件记忆、评测回放和平台治理等知识点。
- `visuals/course-knowledge-graph-neo4j-v10.svg/png/pdf`：v10 实体关系图的 Neo4j 风格命名版。
- `visuals/course-knowledge-graph-graphviz-v11.dot`：Graphviz 节点、边和关系类型源文件；后续修改关系时从该文件重新生成，避免手工 SVG 箭头断裂。
- `visuals/course-knowledge-graph-graphviz-v11.svg/png/pdf`：Graphviz 第一阶段实体关系图，先用于检查节点覆盖、关系语义和箭头完整性，再进行视觉集成。
- `visuals/course-knowledge-graph-graphviz-v12.dot`：增强说明版 Graphviz 源文件；为每个知识域增加“要回答的问题”、为关键节点增加教学解释，并加入课程资料仓库地址。
- `visuals/course-knowledge-graph-graphviz-v12.svg/png/pdf`：增强说明版课程知识图谱，保持自动布局和完整箭头。
- `visuals/course-knowledge-graph-graphviz-v15.dot`：紧凑上下分层版 Graphviz 源文件；相较 v12 减少横向跨度，适合课程海报、投影和打印。
- `visuals/course-knowledge-graph-graphviz-v15.svg/png/pdf`：当前推荐的紧凑版课程知识图谱。
- `visuals/course-poster-light-v6.svg/png/pdf`：更新后的浅色课程海报；加入课程知识图谱主线和 GitHub 课程资料仓库地址。
- `visuals/course-poster-light-v8.svg/png/pdf`：精简宣传版海报；删除长段说明、论文列表和技术栈列表，保留标题、主视觉、课程数据、六个能力关键词、17 周路线、成果和 GitHub 地址。
- `visuals/course-poster-light-v9.svg/png/pdf`：精简宣传版图标增强版；在六个能力关键词卡片中加入 GPU、可观测、诊断、Agent、对象和调查线性图标，并保留统一浅蓝主视觉窗格。
- `visuals/course-poster-multiagent-hero-cropped.png`：裁掉原始多智能体素材的灰色外框，用于与海报主视觉背景融合。
- `visuals/course-poster-light-v4.svg/png/pdf`：浅色研究型海报；多智能体图片与浅色背景统一，课程内容覆盖、六大能力模块、17 周路线、研究案例和交付成果作为主体信息。
- `visuals/course-poster-v3.svg/png/pdf`：海报版；加入大模型—多智能体主视觉、四类 Agent 角色说明、五个生产问题、六条能力主线、研究案例、技术栈与可交付成果。
- `visuals/course-poster-multiagent-hero.png`：从课程材料中独立裁取的多智能体插图，仅作为海报主视觉素材，不使用完整第三方 PPT 页面。

## 编译

```bash
xelatex -interaction=nonstopmode -halt-on-error AI-Native-AIOps-2026-Week-01.tex
xelatex -interaction=nonstopmode -halt-on-error AI-Native-AIOps-2026-Week-01.tex
```

将文件名替换为 `Week-02`、`Week-03`、`Week-04`、`Week-05`、`Week-06`、`Week-07`、`Week-08`、`Week-09`、`Week-10`、`Week-11`、`Week-12`、`Week-13`、`Week-14`、`Week-15`、`Week-16` 或 `Week-17` 可编译对应讲次；建议连续运行两次 XeLaTeX。

推荐使用 XeLaTeX。主题依赖系统字体 `Heiti SC`、`STSong`、`Times New Roman` 和 `Helvetica Neue`。

## 引用说明

- 课程结构以 2026-07-04 修订版课程大纲为准。
- 主讲人研究信息来自中山大学计算机学院官方主页和对应论文；正文方法页按论文或系统名称组织。
- TELLER、AgentChaos 和 AI 系统六层图保留论文出处，仅用于教学。
- 训练并行与 All-Reduce、连续批处理、PagedAttention、vLLM、P/D 解耦、llm-d、RAG、Agent 与 MCP 页面只裁取本地公开材料中的核心图表，不使用整页课件截图；每页均补充中文解释并标明文件和页码。
- `ai-infra-engineer-learning-main` 用于补充训练、推理与 LLM 基础设施的工程解释。
- 企业案例均按脱敏教学案例组织；内部材料文件名不出现在课件正文。
- 第 3 讲深度使用 TELLER、ByteRobust、Minder、AgentTracer、OpsLoop 和 AgenticSRE 材料；论文内容按“问题—机制—证据—实验—边界”展开。
- 第 4 讲深度使用 SwissLog、TraStrainer、Mint、ZeroTracer、TELLER、AgentTracer 和 AgenticSRE 材料；并按 2026 年官方文档校正 Promtail EOL、Loki OTLP、Jaeger v2 和 OpenTelemetry Logs 状态。
- 第 5 讲深度使用 vLLM、DCGM、PagedAttention、DistServe、TELLER、METIS、Langfuse、OpenTelemetry GenAI、AgentTracer 和 AgenticSRE 材料；把用户 SLO、Token/成本、推理运行时、GPU 和 RAG/Agent Outcome 串成统一调用链。
- 第 6 讲深度使用 Minder、SLA-VAE、ShareAD、MOTSAD、AlertGuardian、TranAD 和 Anomaly Transformer；以稳健统计、Isolation Forest、Prophet、深度模型、区间/事件评测和 Alertmanager 告警治理组成完整教学链路。
- 第 7 讲深度使用 MicroRank、Nezha、ChangeRCA、HotSpot、CauseLens 和 TELLER；把调用链、维度贡献、事件图、变更证据与实验 2 组织成“候选—路径—证据—反证—动作”的诊断链路。HotSpot 的公式和图为课程重绘，未虚构论文未核实的实验数字。
- 第 8 讲深度使用 CauseInfer、CauseLens、LLMRCA、AI 系统故障综述、AgentChaos 和 TELLER；以“相关—时间—结构—干预—反事实”为因果证据阶梯，并用缓存 TTL、RAG 旧文档和 Agent 截断响应三个案例贯穿方法选择、反证与安全验证。
- 第 9 讲深度使用 OpsLens、WeRCA、AlertGuardian、AgentTracer、ReAct、StateFlow、TapeAgents、SWE-agent、WorkArena++ 以及陈鹏飞教授项目材料中的 AgenticSRE/OpsLoop/网络分区/KV Cache 案例；按“问答—查询—巡检—诊断—SOP—审批—受控执行—复盘”的能力阶梯组织内容。
- 第 9 讲中的论文架构图均从原论文页面独立裁切；项目 PPT 仅提取内嵌 UI/架构图片，不使用整页第三方 PPT 截图。论文、项目阶段性探索和教学重绘分别标注，数值结果保留实验条件与外部有效性限制。
- 第 10 讲深度使用陈鹏飞教授项目材料中的五行业调研、电商大促级联故障、运维演进、维护—测试—知识反馈、OpsLoop/OpsEval 与工具资产材料，并结合 `Enterprise Trends for Generative AI`、`agentworkflows` 和企业 Agent 背景课件讨论转型阶段门。
- 第 10 讲将调研数字、项目架构和界面全部标注为项目材料/阶段性探索；重点不在复述数字，而在讲清大型客户如何用基线、数据契约、平台治理、组织协同和持续运营把工具试点变成能力体系。
- 所有来自论文或项目 PPT 的图片均为独立单图、实验图或软件界面截图，不使用整页 PPT 截图。
- 第 11 讲将平台算法拆成“问题—直觉—公式/契约—案例—边界”连续页，并用 Minder、Nezha、ChangeRCA、AlertGuardian、TELLER 等论文把训练集群、告警生命周期、变更证据和 LLM 推理跨层诊断串到统一的 Evidence Bundle 接口。
- 第 11 讲正文不出现个人姓名或项目文件名来源字样；课程案例界面只作为独立裁切和教学重绘，论文来源在页脚按论文题名、会议和图号引用。
- 第 12 讲把 DistServe、PagedAttention、METIS、Mint、LLMRCA 和 AgentChaos 均拆成机制页、结果页、解释/边界页和平台结论页；结果数字保留论文实验条件，不把局部结果外推为普遍结论。第 12 讲正文不出现个人姓名或具体项目文件名，外部课件只抽取独立图片或内容，不使用整页第三方 PPT 截图。
- 第 12 讲新增 StriaTrace 作为在线 LLM 推理的首次完整讲解：关键同步点、关键路径和异常时细追解决 TTFT/TPOT 稀有 spike；第 17 讲仅复用其作为 Agent 调查工具，避免重复讲运行时架构。
- 第 13 讲把 RCA Agent 落到 Task Envelope、状态机、工具 schema、Evidence Bundle、Hypothesis Store、Verifier、HITL、ActionStack 和终态 Oracle；用 WeRCA、LLMRCA、AgentChaos、OpsLens 和 AgentTracer 的条件化结果说明方法有效性与外部边界。第 13 讲正文不出现个人姓名或具体项目文件名，课程案例只作为独立界面裁切和教学重绘。
- 第 14 讲把自然语言请求编译为 Intent Contract 和 Workflow DSL，按显式状态、Error/Verify、Tape/Trace、Approval、Rollback、Oracle 组织流程；StateFlow、TapeAgents、WorkArena++ 分别给出机制、结果、解释和边界。Antithesis 用于讲确定性模拟/故障注入/反例回放，Clockwork 用于讲 GPU 准入/放置/执行/遥测/再规划；两页只采用官网公开产品定位，不虚构性能数字。第 14 讲正文不出现个人姓名或具体项目文件名，也不使用完整第三方 PPT 页面截图。
- 第 15 讲在“可观测性与 Profiling”中完整讲解 Neutrino 的 assembly-level probe、对象归属、结果与开销；在 AI 集群论文专题中加入 What-if Straggler 与 FLARE，并保留 Aegis/网络方法的对象图落点。第 17 讲只说明 Agent 在什么证据条件下调用这些工具。
- 第 16 讲把通知流逐层编译为 Canonical Event、Episode 和对象级事件记忆，明确区分 Merge、Link 与 RCA；COLA、iPACK、Oasis、ESRO、AlertGuardian 均给出机制、结果、解释和失效边界。NSDI 2024--2026、OSDI 2025、SIGCOMM 2024--2025 的论文被转译为 rank/collective、恢复状态机、GPU kernel、RNIC/path、供电/散热等事件字段；正文不使用完整第三方 PPT 页面截图，也不引入课程项目执行汇报内容。
- 第 17 讲把 RCA 表述为有对象、时间、权限、预算和停止条件的序贯调查；按服务阶段、训练步骤、rank/collective、GPU kernel、网络 path 的证据分辨率组织 OSDI/NSDI 论文，而不是集中罗列论文。所有论文图均为独立图，结果页保留数据集、指标和边界；正文不使用完整第三方 PPT 页面，也不引入课程项目执行汇报内容。
- 课程概念关系图的模型辅助分析记录见 `MODEL-ASSISTED-GRAPH-ANALYSIS-2026-08-23.md`；DeepSeek 与 Qwen 的建议均被综合为 7 个知识域、1 条课程主线和 8 类关系语义。
