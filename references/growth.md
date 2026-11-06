# 增长与用户分析方法

只在问题和数据匹配时使用；指标口径、分母、观察周期、样本范围和不确定性须明确。增长路径不一定是线性漏斗。

## AARRR / AAARRR 用户增长框架
- 适用：识别从认知到使用、留存与商业化的障碍。
- 做法：AARRR 五类为 Acquisition 获客、Activation 激活、Retention 留存、Referral 推荐、Revenue 收入；AAARRR 是部分实践者增加 Awareness 认知的六阶段变体，先明确版本。为各阶段定义人群、事件和时间窗口，分析转化与流失，对最重要障碍设计实验。
- 边界：阶段顺序可因商业模式不同而改变，不是所有产品都依赖推荐；认知不等于获客，曝光和去重人数不能混用。单看漏斗不证明原因。
- 来源：[Pirate Metrics 方法介绍](https://mcgaw.io/wp-content/uploads/2016/04/PirateMetrics_Final.pdf)；[AAARRR 六阶段实践示例](https://www.reddit.com/r/growth/comments/1qdqymw/growth_marketing_series_lesson_1_growth_funnel/)。

## 转化漏斗分析
- 适用：定位用户多步骤流程的流失。
- 做法：定义人群、事件顺序、观察窗口和去重口径；逐层计算转化与流失，比较渠道、设备或群组；提出需进一步验证的假设。
- 边界：事件漏报和多路径行为可扭曲结果；低转化不自动意味着该环节是根因。
- 参考：[a16z 市场平台指标](https://a16z.com/13-metrics-for-marketplace-companies/)。

## Cohort 分群留存
- 适用：判断不同批次或渠道的用户是否持续获得价值。
- 做法：按首次使用或付费时间分群；定义留存行为、周期及分母，比较同龄群组的留存曲线，并检查人群、渠道和季节性变化。
- 边界：群组构成不同可能造成偏差；相关趋势不能单独证明因果或网络效应。
- 来源：[a16z — User retention cohorts](https://a16z.com/13-metrics-for-marketplace-companies/)。

## 核心行为留存
- 适用：登录和打开量不能体现用户是否得到价值。
- 做法：定义直接关联用户价值的核心行为，例如完成预订；按同期群组衡量重复执行比例，并对照业务结果。
- 边界：行为只是价值代理指标，不能只因频率上升就断定体验或收入改善。
- 来源：[a16z — Core action retention](https://a16z.com/13-metrics-for-marketplace-companies/)。

## 北极星指标与输入指标
- 适用：团队指标分散，缺少围绕用户价值的共同方向。
- 做法：定义反映用户获得价值、与长期业务相关的指标；列出少量可影响输入指标及其假设，验证与结果的关系，同时设置质量或风险护栏。
- 边界：单一指标不能覆盖所有目标；不能把指标树的关联视为已证实的因果关系。
- 来源：[Amplitude — North Star Framework](https://amplitude.com/books/north-star/about-north-star-framework)。

## PMF 用户失望度调查
- 适用：探索活跃用户对现有产品的依赖程度和价值所在。
- 做法：面向定义清楚的真实用户询问若产品不可用会多失望，按群体分析理由和需求，并结合留存、付费与行为证据。
- 边界：Superhuman 的案例使用 40% 作为经验参考，不是普遍通过线；选择偏差、样本规模、活跃用户覆盖及问法会影响结论，不能单凭分数证明 PMF。
- 来源：[First Round — Superhuman PMF](https://review.firstround.com/how-superhuman-built-an-engine-to-find-product-market-fit/)。

## 双边市场流动性与网络效应
- 适用：交易平台需要判断供需是否能有效匹配。
- 做法：分地区和群体衡量匹配成功、等待、成交与核心行为留存；比较供需变化和不同时点群组，提出网络效应的可检验假设。
- 边界：用户增长和留存上升不自动证明网络效应；地域密度、品类和供需结构均会改变结论。
- 来源：[a16z — 13 Metrics for Marketplace Companies](https://a16z.com/13-metrics-for-marketplace-companies/)。

## 早期手工服务用户
- 适用：产品初期尚未理解需求或找到可重复的价值交付路径。
- 做法：主动招募少量目标用户，手工协助完成关键任务，记录行为、障碍和真实反馈；识别重复需求后再决定产品化或自动化。
- 边界：个别热情用户不代表市场；人工服务不可持续时要测算成本，也不能把“不可规模化”当作长期经营原则。
- 来源：[Y Combinator — Do things that don't scale](https://www.ycombinator.com/library/96-do-things-that-dont-scale)。
