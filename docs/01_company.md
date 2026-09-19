# Marvell是什么公司及如何读它的财报

[返回学习地图](../README.md)

## 商业模式

Marvell是无晶圆厂半导体设计公司：核心工作是芯片设计、IP、软件与客户协同，生产依靠外部制造及封装测试体系。通用商用芯片由多家设备厂采用，定制ASIC则围绕特定客户需求设计。项目成功通常要经历选型、设计导入、验证和量产，客户宣布合作不等于当期芯片收入。[年报业务及制造章节][S01]

“ASIC”本身是专用集成电路，不等于“为单一云厂商定制”。Teralynx也属于ASIC，但可作为merchant产品销售。Custom ASIC是另一种合作和商业模式。

## 财务读数

以下单位为**百万美元**。FY为Marvell财年，不能直接与自然年市场数据横向相除。

| 指标 | FY2025全年 | FY2026全年 | FY2027 Q2单季 |
|---|---:|---:|---:|
| 期末 | 2025-02-01 | 2026-01-31 | 2026-08-01 |
| 公司收入 | 5,767.3 | 8,194.6 | 2,739.3 |
| 数据中心收入 | 4,164.2 | 6,100.3 | 2,171.5 |
| 数据中心占比，按公司取整 | 72% | 74% | 79% |
| 其他收入口径 | 其余终端市场重列合计 | Communications and other 2,094.3 | Communications and other 567.8 |

年度数来自[10-K收入表][S01]，季度来自[最新业绩收入趋势表][S03]。FY2026公司收入同比增长42.1%；最新单季收入同比约37%，数据中心同比约46%。增速属于不同时间窗口。

盈利要区分口径。FY2026 GAAP净利润约26.70亿美元，non-GAAP约24.66亿美元；全年GAAP毛利率51.0%。该年利润包含出售汽车以太网业务的一次性收益，不能把净利跳升全归因于交换业务。FY2027 Q2 GAAP毛利率53.1%、non-GAAP 58.9%，GAAP净利润3.080亿美元。[年度业绩][S02] [季度业绩][S03]

## 财报能告诉你什么

- 数据中心已经是公司研究重点，单看传统企业交换产品会漏掉主要增长逻辑。
- 自FY2026 Q4，终端市场披露合并为Data center和Communications and other，前者范围未变。不能把旧的enterprise networking条目直接当作数据中心交换收入。[分类变化][S02]
- 年报为一个可报告分部，终端市场拆分不等于按产品披露。公开文件没有给出可直接使用的Teralynx收入、ASP和出货量。[10-K][S01]

**研究判断：财报用于确定方向、检验数量级和观察经营周期。交换ASIC市场仍要另建模型。**

## 产品组合怎样连成一体

| 功能 | 产品或方向 | 终端价值 |
|---|---|---|
| 计算 | Custom ASIC、OCTEON DPU | 针对客户工作负载计算或卸载基础设施任务 |
| 交换 | Teralynx、部分Prestera、Structera S | 在网络或设备之间选择数据路径 |
| 互连 | PAM4 DSP、coherent DSP、Alaska PHY/retimer | 让高速信号可靠地跨铜缆、光纤或板级走线传播 |
| 存储与内存 | SSD/HDD控制器、Fibre Channel、CXL产品 | 访问、组织或扩展数据存储和内存 |

按[官网产品目录][S29]概括；不同功能不能用同一市场分母。

## 2026年值得注意的范围变化

Celestial AI和XConn分别于2026年2月2日、2月10日完成收购：前者扩展光互连，后者扩展PCIe/CXL交换。因此它们在FY2026期末之后，不能把收购后产品倒算进FY2026全年的可比收入。[年报期后事项][S01]

2026年3月31日，Marvell与NVIDIA宣布NVLink Fusion合作，NVIDIA投资20亿美元。两家公司在部分领域合作，同时在其他产品上竞争。不能据此认定Marvell交换芯片独家进入NVIDIA系统。[正式公告][S27]

2026年4月22日公告收购Polariton，继续扩展光调制技术。它说明研发方向，不能单独证明某个光产品市场已经量产兑现。[公告][S28]

## 读财报时的四个禁区

1. 不用公司全部Data center收入代表交换芯片收入。
2. 不用发货目的地代表最终部署地；制造链和分销会改变地域分布。
3. 不把设计定点、送样、订单和确认收入放在同一列。
4. 不把一季度乘四称为全年实际，不把管理层指引称为已实现收入。

下一步：[产品在系统里具体做什么](02_products.md)。

[S01]: https://investor.marvell.com/sec-filings/all-sec-filings/content/0001835632-26-000011/mrvl-20260131.htm
[S02]: https://investor.marvell.com/news-events/press-releases/detail/1011/marvell-technology-inc-reports-fourth-quarter-and-fiscal-year-2026-financial-results
[S03]: https://investor.marvell.com/news-events/press-releases/detail/1031/marvell-technology-inc-reports-second-quarter-of-fiscal-year-2027-financial-results
[S27]: https://investor.marvell.com/sec-filings/all-sec-filings/content/0001193125-26-134462/d113606dex991.htm
[S28]: https://www.marvell.com/company/newsroom/marvell-acquires-polariton-advancing-future-of-optical-connectivity.html
[S29]: https://www.marvell.com/
