# 证据台账与仍未解决的问题

[返回学习地图](../README.md) · [完整来源](../docs/09_sources.md)

公司与市场事实核查日2026-09-19；E21–E23芯片内部与统计边界说明于2026-09-20补充。本表保留会影响研究结论的关键口径，不是原文转载。

| ID | 主张/数值 | 时间与口径 | 性质／来源 | 使用限制 |
|---|---|---|---|---|
| E01 | Marvell FY2026收入8,194.6百万美元 | 财年止2026-01-31 | 披露 [S01][S01] | 非自然年、非交换业务 |
| E02 | 同年数据中心6,100.3百万美元 | 公司终端市场 | 披露 [S01][S01] | 含定制、互连、存储等 |
| E03 | 最新单季收入2,739.3百万美元、数据中心2,171.5百万美元 | FY2027 Q2，止2026-08-01 | 披露 [S03][S03] | 不能当2027自然年数据 |
| E04 | 数据中心占比约79% | 同上，公司取整 | 披露 [S03][S03] | 不是AI交换收入比例 |
| E05 | Teralynx 10为51.2T且已公告量产 | 2024-07-25 | 厂商 [S05][S05] | 不证明所有SKU供货状态 |
| E06 | T100为102.4T，公告当季送样 | 2026-06-01 | 厂商 [S06][S06] | 送样非量产，性能比较待验证 |
| E07 | PCIe 60260为260 lane | 2026-03发布 | 厂商 [S08][S08] [S30][S30] | 256数据+4管理；不是260网络端口 |
| E08 | Structera 30260面向CXL内存池 | 2026-03发布资料 | 厂商 [S09][S09] | 不归入以太网整机 |
| E09 | Tomahawk 6公告量产 | 2026-03-12 | 厂商 [S13][S13] | 有产品不等于可推市占率 |
| E10 | G300为102.4T | 2026-02-10 | 厂商 [S14][S14] | 公告系统可用目标需查实际 |
| E11 | Astera产品页列320 lane Scorpio | 截止日动态页 | 厂商 [S16][S16] | 不沿用旧版“最高lane”宣传作事实 |
| E12 | 2025数据中心以太网整机325亿美元 | 全球、自然年 | IDC实际估计 [S17][S17] | 不是芯片，不含所有协议 |
| E13 | 2026 Q2数据中心以太网整机123亿美元 | 全球、单季 | IDC实际估计 [S18][S18] | 不能直接称全年实际 |
| E14 | 800G占41.2% | 2026 Q2、上述收入 | IDC估计 [S18][S18] | 非端口或GPU数量比例 |
| E15 | NVIDIA/Arista/Cisco分别20.4/18.7/18.2% | 2026 Q2数据中心以太网收入 | IDC估计 [S18][S18] | 非全以太网、非ASIC份额 |
| E16 | 以太网约占三分之二 | 2026 Q1 AI集群后端交换销售 | Dell’Oro估计 [S19][S19] | 非全球所有DC、非部署量份额 |
| E17 | AI后端2030超过1,000亿美元 | 含scale-up/out/across | Dell’Oro预测 [S20][S20] | 非已实现、不可当merchant ASIC TAM |
| E18 | GB300 NVL72 72 GPU/机柜、最高142kW | 指定官方参考配置 | 原始资料 [S24][S24] | 不是通用功耗换算系数 |
| E19 | 800VDC混合与行级路线 | 2026-08官方更新 | 厂商路线 [S25][S25] | 目标年不等于部署率 |
| E20 | NVIDIA与Marvell合作及20亿美元投资 | 2026-03-31 | 正式公告 [S27][S27] | 不推出独家供货或已量产份额 |
| E21 | Teralynx 10简报列有集成SerDes、PCS/FEC、MAC、转发、缓存和遥测等模块 | 2023-03简报第1页；2026-09-20复核 | 厂商产品框图 [S32][S32] | 集成功能不等于多颗单独销售的芯片；不据框图推模块成本或实测排名 |
| E22 | PHY可以表示功能边界，Marvell也销售独立PHY／retimer／gearbox产品 | 2026-09-20 | 厂商接口说明及产品目录 [S33][S33] [S11][S11] | 每端口外置器件数量须按实际物料清单确认；不默认1:1 |
| E23 | 缓存吸收短暂突发，但不增加拥塞出口带宽，长队列会增加等待 | 原理解释；2026-09-20核查 | 设备厂商技术白皮书 [S35][S35] | 不据缓存MB单独判断性能优劣；需同流量、配置与时延测试 |

## 仍未验证

| 问题 | 为什么关键 | 下一动作 |
|---|---|---|
| 客户所说switch具体产品与地域 | 决定全部模型边界 | 首次会议确认 |
| 交换ASIC分代净ASP | 决定收入规模 | 芯片/OEM/采购多方验证 |
| Marvell及竞争者merchant ASIC份额 | 整机份额不可代替 | SKU映射与出货访谈 |
| 每类AI平台端口/BOM和共网 | 决定每GPU芯片含量 | 运营方+OEM配置核对 |
| T100、PCIe6、CXL新产品的量产/认证节奏 | 决定可服务市场的时间 | 供货确认、客户认证证据 |
| 部署量和以太网采用量份额 | 不能以网络销售额比例代替 | 分架构设备出货与运营方验证 |
| 800VDC笔记内的金额、39GW与年份预测 | 多处为同源转述 | 有权限的原始研究核查；不进入基准模型 |
| 可争取份额与客户定点 | 不能从技术支持推出订单 | 客户项目与采购开放程度验证 |

本手册未编造这些缺失数据，配套模型只使用显式演示假设。

[S01]: https://investor.marvell.com/sec-filings/all-sec-filings/content/0001835632-26-000011/mrvl-20260131.htm
[S03]: https://investor.marvell.com/news-events/press-releases/detail/1031/marvell-technology-inc-reports-second-quarter-of-fiscal-year-2027-financial-results
[S05]: https://www.marvell.com/company/newsroom/marvell-teralynx-512t-ethernet-switch-enters-volume-production-for-global-ai-cloud-deployments.html
[S06]: https://www.marvell.com/company/newsroom/marvell-announces-102-4-tbps-ai-cloud-data-center-switch.html
[S08]: https://www.marvell.com/company/newsroom/marvell-260-lane-pcie-6-switch-ai-data-center-scale-up.html
[S09]: https://www.marvell.com/blogs/structera-s-scaling-the-ai-memory-wall-with-cxl-switching.html
[S13]: https://investors.broadcom.com/news-releases/news-release-details/broadcom-now-shipping-worlds-first-1024-tbps-switch-production
[S14]: https://blogs.cisco.com/sp/cisco-silicon-one-g300-the-next-wave-of-ai-innovation
[S16]: https://www.asteralabs.com/products/scorpio-smart-fabric-switch/
[S17]: https://www.idc.com/resource-center/blog/ethernet-switch-market-size-and-growth-datacenter-segment-surges-60-in-q4-as-ai-workloads-expand/
[S18]: https://www.idc.com/resource-center/blog/ethernet-switch-market-surges-43-4-to-18-9b-in-2q26-as-ai-infrastructure-demand-drives-record-datacenter-spending/
[S19]: https://www.delloro.com/news/ethernet-extends-lead-in-ai-scale-out-networks-despite-strong-infiniband-rebound/
[S20]: https://www.delloro.com/news/ai-back-end-switch-market-will-push-past-100-billion-by-2030/
[S24]: https://docs.nvidia.com/enterprise-reference-architectures/nvl72-ai-factory/latest/components.html
[S25]: https://blogs.nvidia.com/blog/800-vdc-power-architecture-ai-factory/
[S27]: https://investor.marvell.com/sec-filings/all-sec-filings/content/0001193125-26-134462/d113606dex991.htm
[S30]: https://www.marvell.com/blogs/pcie-switching-ai-scale-up-networks.html
[S11]: https://www.marvell.com/products/ethernet-phys.html
[S32]: https://www.marvell.com/content/dam/marvell/en/public-collateral/switching/marvell-teralynx-10-data-center-ethernet-switch-product-brief.pdf
[S33]: https://www.synopsys.com/articles/integrated-400g-800g-ethernet-ip.html
[S35]: https://www.cisco.com/c/en/us/products/collateral/switches/nexus-9000-series-switches/white-paper-c11-738488.html
