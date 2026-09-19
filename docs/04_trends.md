# 技术迭代怎样改变市场规模

[返回学习地图](../README.md)

## 用模型变量理解趋势

| 技术或需求变化 | 对客户有什么用 | 哪个模型变量会变 | 需要什么证据 |
|---|---|---|---|
| 400G向800G及1.6T升级 | 单连接搬运更多数据 | 端口速度、每代ASP、代际份额 | 各速率端口出货与客户认证 |
| 51.2T向102.4T ASIC升级 | 容量或端口基数增加 | 每芯片端口数、拓扑层级、ASIC数 | 完整端口配置及BOM |
| Ethernet在AI后端扩展 | 更广生态与系统选择 | 以太网部署量份额 | 按相同工作负载／单位拆分，不能拿收入占比代替 |
| scale-up域扩大 | 更多加速器紧密协同 | 每计算域交换数、协议份额、连接距离 | 计算域设计、协议和软件实现 |
| 铜缆、AEC、可插拔光、CPO并存 | 在距离、功耗、成本、维修间选择 | 光化比例、每链路器件数、BOM边界 | 分距离及架构渗透率 |
| 推理和agentic应用扩大 | 支持数据准备、缓存和多个服务协作 | CPU／存储端点、前端网络配置 | 分应用服务器及网络架构 |
| 电力与散热成为约束 | 在同一电力预算下多完成任务 | 投运时间、部署量、系统功耗和设备选择 | 已投运MW、设计功率、认证及交付 |

## 带宽翻倍不等于芯片颗数翻倍

固定速率下，交换容量更大可能让每颗芯片支持更多端口，减少交换层级。端口速率同时翻倍时，可用端口数可能不变。收入取决于颗数、代际混合和ASP三者。高端ASIC可以更贵，同时每GPU所需芯片颗数更少；$/Tbps下降与市场收入增长也能同时出现。

本手册将51.2T、102.4T作为分代观察指标。[Teralynx 10][S05] [T100][S06] [Tomahawk 6][S13] 具体端口、封装、功耗与价格须按SKU和系统配置确认。

## 协议竞争分两层

AI scale-out长期关注Ethernet与InfiniBand的选择。以太网AI方案还需要RDMA、拥塞控制、负载均衡、网卡和交换机协同，单有800G端口并不能保证AI性能。[NVIDIA Spectrum-X][S15]

Scale-up则涉及NVLink、PCIe、UALink及不同以太网实现。协议语义、内存访问和软件生态不同，不能把各类switch当作完全可替代的零件。UEC的1.0于2025年6月发布，1.0.1是修订版本；UALink 200G 1.0说明其加速器scale-up定位。标准发布不等于量产部署，也不代表所有设备立即互通。[UEC][S22] [UALink][S23]

Marvell与NVIDIA开展NVLink Fusion合作说明生态关系可能同时包含合作与竞争。不要用“开放协议必胜”或“某厂商封闭所以无机会”直接设置终局份额。[合作公告][S27]

## 光互连的机会与替代效应

机柜内短距离可采用被动铜或AEC，更远距离通常增加光互连需求。高速率使电信号完整性更难，推动光器件靠近芯片。CPO把光引擎与交换芯片更紧密集成，有潜力降低电连接功耗，但改变可维护性、封装和供应责任。

对Marvell要同时问：新增多少连接？每条连接采用什么介质？是否仍需要独立DSP？哪些功能已集成到封装中？**不能同时把CPO内光引擎收入、被替代的可插拔模块收入和其中DSP收入都算作新增市场。**[T100封装选择][S06] [PAM4产品][S10]

## 新工作负载会扩大前端需求

Dell’Oro在2026年8月讨论推理与agentic AI带来的CPU、数据移动和缓存网络需求，说明AI影响不局限于训练后端。[机构展望][S21] 研究上应把训练、分布式推理、单机推理及配套通用服务器分开，访谈后确定连接强度，不固定套用某个“GPU:CPU比例”。

## 路线图的证据等级

建议按“标准／研发 → 发布 → 送样 → 认证 → 量产 → 客户大规模部署”标记每一代产品。T100公告中的节电或领先时延是特定厂商比较，须问清负载、端口配置和测试方法后才进入客户经济性模型。Astera官网已列320 lane产品，也说明不能继续无条件沿用几个月前发布稿中的“行业最高lane数”。[T100][S06] [Astera][S16]

预测至少给出基准、加速、延迟三种采用路径，并说明改变的是认证和爬坡年份、端口速度组合还是部署总量，而不是对总市场随意加减一个百分比。

[S05]: https://www.marvell.com/company/newsroom/marvell-teralynx-512t-ethernet-switch-enters-volume-production-for-global-ai-cloud-deployments.html
[S06]: https://www.marvell.com/company/newsroom/marvell-announces-102-4-tbps-ai-cloud-data-center-switch.html
[S10]: https://www.marvell.com/products/pam-dsp.html
[S13]: https://investors.broadcom.com/news-releases/news-release-details/broadcom-now-shipping-worlds-first-1024-tbps-switch-production
[S15]: https://www.nvidia.com/en-us/networking/spectrumx/
[S16]: https://www.asteralabs.com/products/scorpio-smart-fabric-switch/
[S21]: https://www.delloro.com/news/agentic-ai-and-inference-to-supercharge-front-end-networks-growth/
[S22]: https://ultraethernet.org/uec-1-0-spec
[S23]: https://ualinkconsortium.org/faq/
[S27]: https://investor.marvell.com/sec-filings/all-sec-filings/content/0001193125-26-134462/d113606dex991.htm
