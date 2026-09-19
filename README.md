# Marvell 数据中心交换与互连研究手册

这份中文手册用于快速建立行业知识、与 Marvell 确认研究需求，并设计能用桌面研究和访谈完成的市场规模项目。**资料截止 2026 年 9 月 19 日。**

**先抓住主线：Marvell 是数据基础设施半导体供应商。客户口中的“交换机”可能指以太网交换 ASIC，也可能包括 PCIe/CXL 交换或周边互连。先确认产品边界，再测算。** 本手册建议以数据中心以太网交换 ASIC 为主项目，以整机市场为需求参照，把其他器件做成可选模块。[公司产品分类][S04]

## 从哪里开始

| 你的时间或目的 | 推荐阅读 | 读完应能做到 |
|---|---|---|
| 只有30分钟 | [速读](docs/00_quick_start.md) → [首次客户会议](docs/08_client_meeting.md) | 讲清公司定位，提出决定项目范围的问题 |
| 准备半天系统学习 | [公司与财报](docs/01_company.md) → [产品与工作原理](docs/02_products.md) → [产业链与格局](docs/03_industry.md) → [技术趋势](docs/04_trends.md) | 分清不同网络、客户和竞争者 |
| 把已有知识接起来 | [六份电力散热笔记整合](docs/05_notes_bridge.md) | 理解电力约束如何影响网络需求与交付 |
| 准备研究方案与报价 | [市场规模方法](docs/06_market_sizing.md) → [访谈与执行计划](docs/07_research_plan.md) | 确定模型、样本、数据缺口与交付标准 |
| 开始动手测算 | [模型说明](models/README.md) → [下载Excel演示模型](models/market_sizing_demo.xlsx) | 修改假设，查看端口、设备、ASIC与收入如何联动 |
| 查证或继续补资料 | [来源目录](docs/09_sources.md) · [证据台账](research/evidence_register.md) · [待采数据](research/data_request.md) · [术语表](docs/10_glossary.md) | 找到原始口径，避免把预测当事实 |

## 当前最重要的四个结论

1. **公司规模不等于交换产品规模。** Marvell FY2026 全年收入81.946亿美元，其中数据中心61.003亿美元；最新FY2027 Q2数据中心占比约79%。数据中心收入包含多种产品，不能据此反推Teralynx收入。[年报][S01] [季度业绩][S03]
2. **市场已经很大，但整机与芯片不能混算。** IDC估计2025年全球数据中心以太网交换整机市场为325亿美元。这个数可以校验需求，不能作为Marvell交换ASIC的TAM。[IDC][S17]
3. **网络升级的价值来自让昂贵的算力少等待。** 原始带宽之外，拥塞、时延、可靠性、软件和功耗都会影响采购。以太网scale-out、scale-up和光互连应分别分析。
4. **建议从数量推收入。** 新增及替换的计算设备 → 各类网络连接 → 交换机和ASIC数量 → 分代实际ASP。再筛选merchant市场、Marvell技术可服务范围和可争取份额。

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
