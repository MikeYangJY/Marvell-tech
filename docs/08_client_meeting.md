# 首次客户沟通提纲

[返回学习地图](../README.md)

## 这次会议要达成什么

用45分钟确认一个能报价、能执行的研究范围：**业务决策、产品边界、网络用途、地区、年份、计价层级、交付方式、可获得资料。** 首次沟通不必争论一个尚无可靠分母的TAM数值。

## 建议开场

“我们想先确认这次研究聚焦Teralynx以太网交换芯片，还是还包括PCIe/CXL及互连器件。对于以太网交换，我们建议逐家核实整机厂商年度出货，去掉品牌与ODM重复，再映射芯片和净成交价。我们已经做了公开资料试点：型号对应可以查到，但年度销量和直供拆分仍需访谈。因此先完成小范围取数验证，再确定全球交付范围；外部机构报告只作独立结果的事后校验。”

英文版本：

“We propose to build an independent shipment estimate by equipment supplier and product family, remove OEM/ODM overlaps, and map configurations to switch silicon and net prices. Our desktop pilot verified some source data and product mappings, but annual shipment and direct-sales splits still require targeted interviews. We would validate data access before committing to global coverage, and use external market reports only as a subsequent cross-check. First, we would like to confirm whether the scope is Teralynx Ethernet silicon or also includes PCIe/CXL and adjacent interconnect products.”

## 45分钟议程

| 时间 | 讨论 | 要记录的答案 |
|---|---|---|
| 0—5分钟 | 本项目支持什么决策 | 产品规划／客户／区域／销售目标，主要使用者 |
| 5—15分钟 | 产品、网络和计价范围 | SKU、ASIC/整机、前后端、scale-up、是否含光 |
| 15—25分钟 | 地区、时间和拆分深度 | 部署地/采购地、基年、预测期、客户类别 |
| 25—35分钟 | 方法和可用资料 | 既有估计、BOM样例、公开/保密边界、访谈渠道 |
| 35—45分钟 | 交付与下一步 | 验收口径、节奏、负责人、范围确认日期 |

## 决定项目范围的十个问题

1. 您希望研究结果改变哪一个具体决策？
2. 主导产品团队及希望纳入的SKU是什么？
3. 需要整机台数/收入、芯片颗数/收入、端口量还是容量？哪些是主要输出？
4. 前端、AI后端、scale-up、管理网络与DCI分别是否包含？
5. 只看merchant市场，还是也要评估内部自研/系统自用芯片的潜在替代机会？
6. 全球还是指定地区？地域按最终部署地点还是采购/制造地点？
7. 是否同意2025实际基年、2026在年估计、2027—2030预测？
8. 工作负载、速度、客户类型和竞争者需要拆到多细？
9. 哪些已有数据或假设希望我们挑战？能否支持验证年度产品族销量、ODM直供拆分、匿名BOM、净价与库存？客户提供的数据将单独标记来源，不当作我们的独立发现。
10. 最终使用者如何判断研究有用：规模精度、客户机会、技术路线还是销量/价格预测？

## 可供客户选择的工作包

| 工作包 | 内容 | 增加的价值及工作量 |
|---|---|---|
| A 核心范围 | 数据中心以太网交换ASIC，前端+AI scale-out，merchant TAM/SAM | 最直接对应Teralynx；先把口径和BOM做扎实 |
| B 扩展互连 | A + 光DSP、AEC/retimer、DCI | 需增加光铜链路距离分层和模块供应链访谈 |
| C 扩展scale-up | A + PCIe/CXL及相关scale-up方案 | 需增加协议/计算域/内存池BOM和平台认证研究 |

这些是范围选项，尚非承诺报价。先定每个模块的输出，再估算访谈量、数据库费用与交付时间。

## 会后应形成的范围确认单

| 字段 | 待客户确认 |
|---|---|
| 业务决策与主要使用者 | 待填 |
| 纳入/排除产品与SKU | 待填 |
| 网络边界及共网处理 | 待填 |
| 收入口径与merchant/captive定义 | 待填 |
| 地域与时间 | 待填 |
| 必需拆分维度 | 待填 |
| 输入资料、权限和访谈渠道 | 待填 |
| 交付物、阶段会议及验收标准 | 待填 |

## 三个容易误答的问题

“市场是不是325亿美元？”——这是IDC对2025年全球数据中心以太网整机市场的估计，可以参考，但芯片市场必须向下拆BOM和外购比例。[IDC][S17]

“102.4T一定把市场翻倍吗？”——要同时看端口速度、芯片颗数、价格和网络层级，容量翻倍不是收入翻倍。

“800VDC会带来多少交换机？”——它影响可部署算力与时间，交换机数量还取决于端点、端口和拓扑。我们会把电力约束作为校验，不直接做一比一换算。

这份提纲尚未发送给Marvell或任何外部人员。

[S17]: https://www.idc.com/resource-center/blog/ethernet-switch-market-size-and-growth-datacenter-segment-surges-60-in-q4-as-ai-workloads-expand/
