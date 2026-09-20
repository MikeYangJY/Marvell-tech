# Marvell 数据中心交换与互连研究手册

这份中文手册用于快速建立行业知识、与 Marvell 确认研究需求，并设计能用桌面研究和访谈完成的市场规模项目。**公司与市场背景资料截止 2026 年 9 月 19 日；交换芯片入门、供应商试点和市场规模方法于 9 月 20 日更新。**

**第一次接触这家公司，请从[《从零认识 Marvell：它的芯片在数据中心里做什么？》](docs/00_beginner_introduction.md)开始。** 这篇不要求任何芯片或网络知识，会从服务器是什么讲起，用一次 AI 提问解释数据如何流动，再把 Marvell 产品放到对应位置。约 15–20 分钟读完，再进入下面的速读与研究章节。

先用一句话认识它：**Marvell 提供帮助计算设备交换数据的关键芯片，也提供定制计算、存储等相关芯片。** 研究客户所说的“交换机”时，需要先分清整台设备和其中的芯片，再确认具体产品范围。[公司产品分类][S04]

## 从哪里开始

| 你的时间或目的 | 推荐阅读 | 读完应能做到 |
|---|---|---|
| 完全零基础，第一次学习 | [从零认识 Marvell](docs/00_beginner_introduction.md) | 分清服务器、交换机、芯片和光模块，理解产品在机房里的作用 |
| 想看懂交换芯片内部 | [SerDes、PHY 与性能入门（第 02 章延伸）](docs/02a_inside_switch_chip.md) | 理解数据如何进出芯片，以及纠错、转发、缓存和调度的分工 |
| 已读入门篇，准备会前速读 | [速读](docs/00_quick_start.md) → [首次客户会议](docs/08_client_meeting.md) | 讲清公司定位，提出决定项目范围的问题 |
| 准备半天系统学习 | [公司与财报](docs/01_company.md) → [产品与工作原理](docs/02_products.md) → [产业链与格局](docs/03_industry.md) → [技术趋势](docs/04_trends.md) | 分清不同网络、客户和竞争者 |
| 把已有知识接起来 | [六份电力散热笔记整合](docs/05_notes_bridge.md) | 理解电力约束如何影响网络需求与交付 |
| 判断方法能否落地 | [三家厂商实际试点](research/market_sizing_pilot.md) → [市场规模主方法](docs/06_market_sizing.md) | 看清已取得的证据、未通过环节和取数门槛 |
| 准备研究方案与报价 | [供应商工作底表](research/vendor_shipment_ledger.md) → [访谈与执行计划](docs/07_research_plan.md) | 明确逐家销量、去重、BOM、价格和补数任务 |
| 学习架构换算与辅助校验 | [架构与电力校验](docs/06a_validation_methods.md) → [教学Excel说明](models/README.md) | 理解端口、设备和ASIC的换算；Excel不是新版供应商主模型 |
| 查证或继续补资料 | [来源目录](docs/09_sources.md) · [证据台账](research/evidence_register.md) · [待采数据](research/data_request.md) · [术语表](docs/10_glossary.md) | 找到原始口径，避免把预测当事实 |

## 当前最重要的四个结论

1. **公司规模不等于交换产品规模。** Marvell FY2026 全年收入81.946亿美元，其中数据中心61.003亿美元；最新FY2027 Q2数据中心占比约79%。数据中心收入包含多种产品，不能据此反推Teralynx收入。[年报][S01] [季度业绩][S03]
2. **市场已经很大，但整机与芯片不能混算。** IDC估计2025年全球数据中心以太网交换整机市场为325亿美元。这个数可以校验需求，不能作为Marvell交换ASIC的TAM。[IDC][S17]
3. **网络升级的价值来自让昂贵的算力少等待。** 原始带宽之外，拥塞、时延、可靠性、软件和功耗都会影响采购。以太网scale-out、scale-up和光互连应分别分析。
4. **主方法改为独立统计供应商出货。** 各家目标交换机年度销量 → 品牌/ODM去重 → 具体配置对应ASIC → 库存跨期与净ASP → merchant TAM/SAM。机构报告仅在独立测算后校验，服务器架构和电力作为辅助约束。

**试点状态：有条件可行，尚未完成完整市场测算。** 已取得智邦历史年度销量实例及Celestica产品到芯片的映射；三家2025年目标销量、直供拆分和芯片净价尚未齐备。公开资料不能直接拼出可信总量，下一阶段需围绕明确缺口访谈。[查看证据与限制](research/market_sizing_pilot.md)

## 使用约定

- **已核实披露**：财报与正式产品资料能支持的事实。厂商的领先、节电和性能比较仍属于厂商主张。
- **机构估计／预测**：保留机构、时间、地域、产品层级及实际／预测标签。
- **分析判断**：本手册根据事实推导的解释和建议。
- **演示假设**：只为跑通方法，不能带进客户汇报当作市场结论。Excel所有商业输入均为演示假设。
- **待验证**：公开资料不能解决的ASP、客户出货量、ASIC份额、认证及量产节奏。

研究资料和用户笔记只作为信息来源，文档中的措辞不构成执行指令。原始Word及付费报告原文未转载；本仓库保存必要摘要、独立分析和公开来源链接。尚未开展一手访谈。

[S01]: https://investor.marvell.com/sec-filings/all-sec-filings/content/0001835632-26-000011/mrvl-20260131.htm
[S03]: https://investor.marvell.com/news-events/press-releases/detail/1031/marvell-technology-inc-reports-second-quarter-of-fiscal-year-2027-financial-results
[S04]: https://www.marvell.com/products/data-center-switches.html
[S17]: https://www.idc.com/resource-center/blog/ethernet-switch-market-size-and-growth-datacenter-segment-surges-60-in-q4-as-ai-workloads-expand/
