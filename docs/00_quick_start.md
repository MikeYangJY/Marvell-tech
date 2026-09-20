# 30分钟建立基本认识

[返回学习地图](../README.md)

**本篇用于入门后的会前复习。** 如果还不清楚服务器、交换机和芯片的区别，请先读[《从零认识 Marvell》](00_beginner_introduction.md)，再回来读这一篇。

## 一句话理解Marvell

Marvell Technology在纳斯达克上市，代码MRVL。它设计把数据搬动、处理、存储和保护起来的芯片，主要收入来自数据中心。研究这家公司，要把自己放在“芯片供应商怎样帮助客户搭建计算基础设施”的位置。[财报][S03] [官网][S29]

终端客户可能说“我要800G交换机”，整机厂家设计交换设备，芯片供应商提供里面的交换ASIC。Marvell Teralynx属于最后这一层。Marvell也卖光模块中的信号处理芯片，所以即使交换ASIC来自另一家公司，链路里仍可能有Marvell器件；具体组合须以BOM验证。

## 五个先分清的概念

| 概念 | 通俗理解 | 和项目的关系 |
|---|---|---|
| 交换机整机 | 有外壳、接口、电源、软件的网络设备 | 下游需求参照，收入含多种成本和整机价值 |
| 交换ASIC | 决定数据包从哪个端口出去的专用芯片 | Teralynx最直接的研究对象 |
| NIC网卡 | 让服务器或GPU系统接入网络 | 决定连接数和单连接速度的重要输入 |
| 光模块／AEC | 承载两端之间的高速链路 | 内含DSP或retimer等器件，需独立测算 |
| 电气开关设备switchgear | 分配、隔离和保护电力 | 与网络交换机是不同市场；对应你原来的电力笔记 |

## 为什么AI需要更强的网络

训练大模型时，多块GPU往往要交换中间结果、梯度或参数。一块GPU等数据，其他设备也可能被拖慢。推理也不只有单卡工作：模型分片、专家路由和缓存搬运都会产生通信。网络采购因此要看“有效任务完成速度”，不能只比端口标称速率。

一个实用区分是：**scale-up让一组加速器紧密合作；scale-out把更多计算节点或计算域连成大集群；前端网络把任务、数据和服务送进送出；DCI跨数据中心传输。** 这些是用途划分，不是严格的机柜内外边界。同一机柜也可以包含多张网络。

## 客户可能真正想研究什么

| 假设范围 | 对应Marvell产品 | 首次沟通确认什么 |
|---|---|---|
| 数据中心以太网交换ASIC | Teralynx | 前端、AI后端都包括吗？是否只看merchant芯片？ |
| AI scale-up交换 | Teralynx相关方案、Structera S等 | 协议、具体SKU、计算域和客户架构是什么？ |
| 交换机周边互连半导体 | Ara/Nova/Spica、Alaska等 | 是算DSP/retimer，还是模块、线缆或整体价值？ |
| 更广的数据中心产品机会 | Custom ASIC、CXL、存储等 | 要另立模块，不能沿用一个交换机分母 |

这些是项目范围假设，尚未获得Marvell确认。[产品分类][S04] [光DSP][S10] [PHY][S11]

## 第一次会上最值得问的六句话

1. 这次研究支持产品规划、区域进入、客户拓展，还是销售目标？
2. 您说的switch具体是哪些产品线和SKU？最终要整机、芯片还是整体网络支出？
3. front-end、back-end scale-out、scale-up、DCI分别是否纳入？
4. 范围是全球还是某个地区，按部署地还是采购地统计，预测到哪年？
5. 是否包含客户自研、NVIDIA/Cisco内部供货，以及InfiniBand/NVLink等替代方案？
6. 能否提供现有市场定义、关键假设区间和可访谈的客户／生态类型？

## 你应能口头讲出的研究逻辑

“我们先逐家核实设备厂商的年度数据中心交换机出货，去掉品牌厂与ODM重复，再按具体配置查芯片颗数、型号和成交净价。公开资料不够的地方用针对性访谈补齐；机构报告只在独立计算后校验。最终分别给出总需求、商用芯片市场和Marvell可服务机会；缺资料的部分明确保留，不假装已经算全。”

实际桌面试点及其限制见[三家厂商试点](../research/market_sizing_pilot.md)，完整步骤见[第06章](06_market_sizing.md)。

[S03]: https://investor.marvell.com/news-events/press-releases/detail/1031/marvell-technology-inc-reports-second-quarter-of-fiscal-year-2027-financial-results
[S04]: https://www.marvell.com/products/data-center-switches.html
[S10]: https://www.marvell.com/products/pam-dsp.html
[S11]: https://www.marvell.com/products/ethernet-phys.html
[S29]: https://www.marvell.com/
