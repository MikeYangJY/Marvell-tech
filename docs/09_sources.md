# 来源目录与阅读优先级

[返回学习地图](../README.md)

原版公开来源访问核查日为2026-09-19；2026-09-20为交换芯片内部原理新增S32–S39，并复核S11。动态网页记录访问日，不猜测发布日期。第一手资料优先用于公司、产品和技术事实；市场数字使用研究机构自己的公开摘要。没有声称读过其付费底表。

## 优先读这六类

1. S04/S05/S06：先看Marvell交换产品及量产/送样差别。
2. S03再读S01/S02：从最新季度到年度，理解公司规模与披露边界。
3. S24：用真实系统把GPU、NVSwitch、NIC与功率连起来。
4. S17/S18/S19：建立市场数量级并识别统计范围差别。
5. S13/S14/S15/S16：比较同层产品与系统，不做跨层排名。
6. S25配合用户笔记：更新电力路线，并保留目标与已实现的区别。

## 公开来源

| 编号 | 来源 | 日期 | 本手册用途与性质 |
|---|---|---|---|
| S01 | [Marvell FY2026 Form 10-K](https://investor.marvell.com/sec-filings/all-sec-filings/content/0001835632-26-000011/mrvl-20260131.htm) | 2026-03-11 | 公司业务、年度收入、终端市场、并购、地域口径；原始披露 |
| S02 | [Marvell FY2026 年度及第四季度业绩](https://investor.marvell.com/news-events/press-releases/detail/1011/marvell-technology-inc-reports-fourth-quarter-and-fiscal-year-2026-financial-results) | 2026-03-05 | 全年财务指标及终端市场分类变化；原始披露 |
| S03 | [Marvell FY2027 第二季度业绩](https://investor.marvell.com/news-events/press-releases/detail/1031/marvell-technology-inc-reports-second-quarter-of-fiscal-year-2027-financial-results) | 2026-08-27 | 截至2026-08-01季度财务与终端市场数据；原始披露 |
| S04 | [Marvell 数据中心交换产品页](https://www.marvell.com/products/data-center-switches.html) | 动态页面 | 以太网、管理网络与PCIe产品分类；厂商产品资料 |
| S05 | [Teralynx 10 量产公告](https://www.marvell.com/company/newsroom/marvell-teralynx-512t-ethernet-switch-enters-volume-production-for-global-ai-cloud-deployments.html) | 2024-07-25 | 51.2T产品量产状态；厂商披露 |
| S06 | [Teralynx T100 发布公告](https://www.marvell.com/company/newsroom/marvell-announces-102-4-tbps-ai-cloud-data-center-switch.html) | 2026-06-01 | 102.4T、3nm及送样计划；性能优势属于厂商主张 |
| S07 | [Teralynx T100 技术说明](https://www.marvell.com/blogs/teralynx-t100-performance-connectivity.html) | 2026-07-28 | 架构与时延设计；厂商解释，不能替代独立测试 |
| S08 | [Structera S 60260 PCIe 6.0 发布公告](https://www.marvell.com/company/newsroom/marvell-260-lane-pcie-6-switch-ai-data-center-scale-up.html) | 2026-03-17 | 260 lane及Q3 2026送样计划；原始产品公告 |
| S09 | [Structera S CXL 内存交换技术说明](https://www.marvell.com/blogs/structera-s-scaling-the-ai-memory-wall-with-cxl-switching.html) | 2026-03-17 | 30260与CXL内存池定位；厂商资料 |
| S10 | [Marvell PAM4 Optical DSP 产品页](https://www.marvell.com/products/pam-dsp.html) | 动态页面 | Ara、Nova、Spica产品与光模块应用 |
| S11 | [Marvell Ethernet PHY 产品页](https://www.marvell.com/products/ethernet-phys.html) | 动态页面 | Alaska A用于AEC的DSP及产品速率 |
| S12 | [Marvell Coherent DSP 产品页](https://www.marvell.com/products/coherent-dsp.html) | 动态页面 | Orion、Canopus、Deneb及DCI定位 |
| S13 | [Broadcom Tomahawk 6 量产公告](https://investors.broadcom.com/news-releases/news-release-details/broadcom-now-shipping-worlds-first-1024-tbps-switch-production) | 2026-03-12 | 102.4T量产与高radix；厂商公告 |
| S14 | [Cisco Silicon One G300 技术说明](https://blogs.cisco.com/sp/cisco-silicon-one-g300-the-next-wave-of-ai-innovation) | 2026-02-10 | 102.4T、1.6T及系统上市目标；厂商公告 |
| S15 | [NVIDIA Spectrum-X 产品页](https://www.nvidia.com/en-us/networking/spectrumx/) | 动态页面 | 以太网交换机、SuperNIC与软件的系统方案 |
| S16 | [Astera Labs Scorpio 产品页](https://www.asteralabs.com/products/scorpio-smart-fabric-switch/) | 动态页面 | PCIe与scale-up交换产品，当前列有320 lane；不等于份额证据 |
| S17 | [IDC 2025全年及第四季度以太网交换市场](https://www.idc.com/resource-center/blog/ethernet-switch-market-size-and-growth-datacenter-segment-surges-60-in-q4-as-ai-workloads-expand/) | 2026-03-18 | 公开摘要，整机市场实际估计；不是交换ASIC收入 |
| S18 | [IDC 2026第二季度以太网交换市场](https://www.idc.com/resource-center/blog/ethernet-switch-market-surges-43-4-to-18-9b-in-2q26-as-ai-infrastructure-demand-drives-record-datacenter-spending/) | 2026-09-11 | 最新季度整机市场、速率结构和品牌份额公开摘要 |
| S19 | [Dell’Oro AI后端以太网与InfiniBand](https://www.delloro.com/news/ethernet-extends-lead-in-ai-scale-out-networks-despite-strong-infiniband-rebound/) | 2026-06-02 | 1Q2026 AI后端市场，ODM与品牌口径和IDC不同 |
| S20 | [Dell’Oro AI后端2030预测](https://www.delloro.com/news/ai-back-end-switch-market-will-push-past-100-billion-by-2030/) | 2026-02-04 | 覆盖scale-up/out/across的预测，不是以太网ASIC TAM |
| S21 | [Dell’Oro 推理对前端网络的影响](https://www.delloro.com/news/agentic-ai-and-inference-to-supercharge-front-end-networks-growth/) | 2026-08-13 | 工作负载变化与前端网络展望；机构预测 |
| S22 | [UEC 1.0.1 发布说明](https://ultraethernet.org/uec-1-0-spec) | 2025-09-05 | 1.0发布于2025-06-11；1.0.1为编辑性修正 |
| S23 | [UALink 200G 1.0 FAQ](https://ualinkconsortium.org/faq/) | 动态页面 | scale-up和内存语义定位；不据此宣称最新版号 |
| S24 | [NVIDIA GB300 NVL72 系统组件参考架构](https://docs.nvidia.com/enterprise-reference-architectures/nvl72-ai-factory/latest/components.html) | 动态版本 latest | 72 GPU、142kW上限、NVSwitch与网卡；特定配置 |
| S25 | [NVIDIA 800VDC 路线更新](https://blogs.nvidia.com/blog/800-vdc-power-architecture-ai-factory/) | 2026-08-11 | 混合改造、power rack与row power center路线；目标不是实现率 |
| S26 | [NVIDIA 800VDC 架构主页](https://www.nvidia.com/en-us/data-center/technologies/800-vdc-architecture/) | 动态页面 | 800VDC定位与官方白皮书入口 |
| S27 | [NVIDIA 与 Marvell NVLink Fusion 合作](https://investor.marvell.com/sec-filings/all-sec-filings/content/0001193125-26-134462/d113606dex991.htm) | 2026-03-31 | 合作范围与20亿美元投资；不能推出独家供货关系 |
| S28 | [Marvell 收购 Polariton](https://www.marvell.com/company/newsroom/marvell-acquires-polariton-advancing-future-of-optical-connectivity.html) | 2026-04-22 | 光调制技术扩展；不能直接推收入规模 |
| S29 | [Marvell 公司官网](https://www.marvell.com/) | 动态页面 | 公司产品组合与官方入口 |
| S30 | [Marvell PCIe scale-up 技术说明](https://www.marvell.com/blogs/pcie-switching-ai-scale-up-networks.html) | 2026-05-21 | 260 lane含256数据lane和4管理lane |
| S31 | [Marvell Alaska P 产品资料入口](https://www.marvell.com/company/media-kit/marvell-alaska-p-pcie-retimer.html) | 动态页面 | PCIe/CXL retimer定位 |
| S32 | [Marvell Teralynx 10 产品简报](https://www.marvell.com/content/dam/marvell/en/public-collateral/switching/marvell-teralynx-10-data-center-ethernet-switch-product-brief.pdf) | 2023-03修订；2026-09-20核查 | 第1页功能框图，证明SerDes、PCS/FEC、MAC、缓存和转发等模块的集成；不据旧简报判断最新供货 |
| S33 | [Synopsys：400G/800G Ethernet MAC、PCS与PHY集成](https://www.synopsys.com/articles/integrated-400g-800g-ethernet-ip.html) | 动态页面；2026-09-20核查 | 接口分工、lane组合与芯片集成方式；不作为最新标准版本或市场规模依据 |
| S34 | [MathWorks：SerDes时钟恢复模型](https://www.mathworks.com/help/serdes/ug/model-clock-recovery-loops.html) | 动态文档；2026-09-20核查 | 均衡与CDR配合的原理；不代表Teralynx具体电路 |
| S35 | [Cisco：数据中心交换机智能缓存管理](https://www.cisco.com/c/en/us/products/collateral/switches/nexus-9000-series-switches/white-paper-c11-738488.html) | 2017-06-06更新；2026-09-20核查 | 缓存、突发和排队的基础原理；不把Cisco产品实现套到Marvell |
| S36 | [AMD：Ethernet MAC Receiver](https://docs.amd.com/r/en-US/am011-versal-acap-trm/MAC-Receiver) | 动态文档；2026-09-20核查 | MAC接收帧检查与FCS；用于功能解释 |
| S37 | [Teledyne LeCroy Xena：112G SerDes自动协商与链路训练](https://cdn.teledynelecroy.com/files/whitepapers/an-lt-testing-for-112g-serdes.pdf) | 文档未采用搜索引擎推测日期；2026-09-20核查 | 第3–4页解释PAM4、FEC及112G名称与106.25Gb/s线路速率；不采用其历史“当前最高”表述 |
| S38 | [剑桥大学研究仓储：FEC Killed The Cut-Through Switch](https://www.repository.cam.ac.uk/items/db710919-ddb6-49d2-bf3f-eb7fe5c7f05f) | 研究仓储页面；2026-09-20核查 | 纠错与转发时延的关系；不从论文标题推出当代交换机没有直通模式 |
| S39 | [AMD：PCS、PMA与PMD](https://docs.amd.com/r/en-US/pg051-tri-mode-eth-mac/PCS-PMA-and-PMD) | 动态文档；2026-09-20核查 | 以太网物理层功能分层；不同速率代际的具体实现另核 |

## 用户提供的六份笔记

| 编号 | 文件名 | 处理方式 |
|---|---|---|
| U01 | 01_Data_Center_Power_and_Electrical_Infra_Basics.docx | 提取正文和表格，整合供电层级和容量概念 |
| U02 | 02_Data_Center_Cooling_System_Basics (Semi).docx | 整合冷却逻辑，保留2025报告的边界 |
| U03 | 03_Why_AI_Data_Center_Are_Moving_to_800VDC (Personal).docx | 整合因果链，核查所列NVIDIA公开资料 |
| U04 | 04_NVIDIA_800VDC_Architecture_Key_Notes.docx | 保留架构启发，标记未充分溯源的个人备注与算术限定 |
| U05 | 05_SemiAnalysis_800VDC_Transition_Notes.docx | 四阶段为机构分析框架，预测未独立核实 |
| U06 | 06_Oxcap_800VDC_Notes.docx | 提炼分母和多架构逻辑，识别对U05同源资料的转引 |

未把六份笔记中的预测数当作六份独立证据。已核查的是用户提供笔记及上述可访问公开资料；未获取或转载完整付费报告。

## 更新时的规则

更新财报、产品量产状态和市场季度数据时，同步改证据台账，保留原统计期。新增来源需说明是独立证据还是转述。下一次客户会议前优先复核T100/Structera量产、ASP区间、IDC/Dell’Oro底表定义。2026年10月6日Marvell投资者日为已公告的未来事件，本版未将其尚未发布内容纳入结论。[当前业绩公告][S03]

[S03]: https://investor.marvell.com/news-events/press-releases/detail/1031/marvell-technology-inc-reports-second-quarter-of-fiscal-year-2027-financial-results
