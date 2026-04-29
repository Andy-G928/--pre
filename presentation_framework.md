# 汇报框架：Should Platforms Be Allowed to Sell on Their Own Marketplaces?

## 0. 总体汇报逻辑

这篇文章最好按“理论故事线”来讲，而不是按论文页数来分。建议主线是：

现实争议 → 研究问题 → 基准模型 → 三种经营模式均衡 → dual mode 的 price squeeze 机制 → 禁止 dual mode 的福利后果 → 加入 imitation 和 self-preferring → 比较结构性禁令与行为监管 → 总结政策含义。

整个汇报的核心观点可以先告诉听众：

平台同时做 marketplace 和 seller 并不必然降低消费者剩余或社会福利。Dual mode 可能通过价格竞争和交易便利带来效率收益。真正的问题是平台可能利用 marketplace 权力进行 product imitation 和 self-preferring。因此，文章认为行为监管通常优于直接禁止 dual mode。

## 0.1 数学结果的讲法要求

每次 slides 中出现公式、lemma、proposition 或阈值条件时，都要紧跟一句经济学直觉。不要只展示数学表达式。建议采用固定顺序：

1. 先说明这个数学结果在回答什么问题。
2. 再解释公式中左右两边分别代表什么经济力量。
3. 最后给出口头直觉：这个条件为什么会让平台、卖家或消费者做出相应选择。

例如，讲 $\tau\leq b$ 时，不要只说“平台佣金受到约束”，而要说：$b$ 是平台交易便利带来的增量价值；如果佣金超过 $b$，第三方卖家就会利用平台让消费者发现产品，然后把交易引到站外，因此平台最多只能抽取消费者从平台交易中获得的便利收益。

## Presenter 1：Motivation, Research Question, and Roadmap

### 1.1 这一部分的目标

第一位汇报人负责“把问题立起来”。听众需要先明白：为什么平台自营是一个严肃的微观理论问题，为什么不能只凭直觉判断“平台既当裁判又当运动员一定不好”。

### 1.2 现实背景

可用以下例子开场：

- Amazon 既运营 marketplace，也销售 Amazon Basics 等自营产品。
- Apple App Store、Google Play、Microsoft Store 等既分发第三方应用，也销售或推广自己的应用和服务。
- 京东、Walmart、Target 等零售平台也有类似双重身份。

这类平台的共同点是：它们既是交易基础设施，又是交易参与者。文章称这种模式为 dual mode。

### 1.3 监管担忧

监管者担心的不是平台卖自己的产品本身，而是平台可能利用 marketplace 权力扭曲竞争：

1. Product imitation：平台观察第三方卖家的销售、价格、搜索、退货等数据后，模仿成功产品。
2. Self-preferring：平台通过搜索排序、推荐、Buy Box 或默认展示规则，把消费者导向自营产品。
3. Entry deterrence 或 innovation distortion：第三方卖家预期会被模仿或被压制，因此减少创新投入。

### 1.4 文章的研究问题

建议在 slides 上明确写出三个问题：

1. 如果禁止平台采用 dual mode，消费者剩余和社会福利是否一定上升？
2. 禁令实施后，平台会内生选择 seller mode 还是 marketplace mode？
3. 相比直接禁止 dual mode，针对 product imitation 和 self-preferring 的行为监管是否更有效？

### 1.5 文章贡献

可以概括为四点：

- 建立一个可求解的理论模型，比较 marketplace mode、seller mode 和 dual mode。
- 说明 dual mode 下平台自营产品可能通过 price squeeze 压低第三方卖家价格。
- 证明禁止 dual mode 可能降低消费者剩余和社会福利，尤其在平台自营效率较高时。
- 说明针对 imitation 和 self-preferring 的 behavioral remedies 通常比 structural ban 更好。

### 1.6 汇报路线

建议第一位最后给出五人分工路线：

1. Motivation and research question。
2. Baseline model setup。
3. Baseline equilibrium and price squeeze。
4. Ban on dual mode and welfare implications。
5. Product imitation, self-preferring, and policy comparison。

## Presenter 2：Baseline Model Setup

### 2.1 这一部分的目标

第二位汇报人要把模型完整搭起来。后面所有命题都依赖这一部分，因此不能只讲文字直觉，必须清楚说明参与者、效用、变量、渠道、平台模式和 timing。

### 2.2 参与者与产品

市场中有四类对象：

1. Platform $M$：
   - 可以运营 marketplace。
   - 也可以销售自己的产品。
   - 如果运营 marketplace，可以向第三方卖家收取单位交易佣金 $\tau$。

2. Innovative seller $S$：
   - 拥有比 fringe sellers 更好的产品。
   - 可以选择创新水平 $\Delta$。
   - 产品价值为 $\nu+\Delta$。

3. Fringe sellers：
   - 至少有两个，产品同质，竞争充分。
   - 产品价值为 $\nu$。
   - 边际成本归一化为 0。
   - Bertrand competition 使其直接渠道价格为 0；若在平台销售，价格等于佣金 $\tau$。

4. Consumers：
   - 连续统，测度为 1。
   - 每个消费者最多购买一单位产品。
   - 消费者异质性来自外部选项 $\nu_o$，其分布为 $G$，密度为 $g$。

### 2.3 产品价值和关键参数

需要重点解释以下符号：

- Fringe product value：$\nu$。
- Innovative seller value：$\nu+\Delta$。
- Platform product value：$\nu+\sigma$。
- Platform convenience benefit：$b>0$。
- Outside option：$\nu_o \sim G$。
- Platform commission：$\tau$。
- Innovation cost：$K(\Delta)$。

其中 $\sigma$ 是非常关键的参数：

- $\sigma>0$：平台自营产品比 fringe sellers 更有效率或更有价值。
- $\sigma<0$：第三方/小卖家在该品类上比平台更有优势。

注意 $\sigma$ 可以理解为质量优势，也可以理解为成本优势。文章中更现实、更重要的情形是 $\sigma>0$，例如大型平台有物流、规模、信誉或系统整合优势。

### 2.4 Innovation

$S$ 选择创新水平 $\Delta \geq \Delta^l$，创新成本为 $K(\Delta)$。其中：

- $\Delta^l$ 是最低创新水平。
- $K(\Delta^l)=0$。
- $K(\Delta)$ increasing and convex。

文章定义最高可能出现的创新水平 $\bar{\Delta}$：

$$
K'(\bar{\Delta}) = G(\nu+\sigma+b).
$$

经济学直觉：

- 左边 $K'(\bar{\Delta})$ 是提高创新水平的边际成本。
- 右边 $G(\nu+\sigma+b)$ 可以理解为高创新在最大相关需求规模下带来的边际收益。
- 因此 $\bar{\Delta}$ 是模型中“最强创新激励”对应的创新水平。后文比较不同平台模式时，一个核心问题就是：哪种模式能让 $S$ 选择 $\bar{\Delta}$，哪种模式只会让 $S$ 停留在最低创新 $\Delta^l$。

### 2.5 Product Discovery

这是模型最重要的设定之一：

- 消费者一开始知道 fringe sellers 和平台自营产品。
- 消费者一开始不知道创新卖家 $S$ 的产品。
- 只有当 $S$ 出现在平台 marketplace 上，消费者才会发现 $S$。

因此，平台不是普通销售渠道，而是 discovery channel。禁止平台采用某种模式，可能会改变消费者能否发现 $S$。

### 2.6 三种平台模式

需要清楚区分：

1. Marketplace mode：
   - $M$ 只做 marketplace。
   - $S$ 和 fringe sellers 可以在平台卖。
   - $M$ 收佣金 $\tau$。

2. Seller mode：
   - $M$ 只卖自己的产品。
   - $S$ 不在平台上被发现。

3. Dual mode：
   - $M$ 同时运营 marketplace 和销售自营产品。
   - $S$ 可以入驻平台。
   - $M$ 的自营产品与 $S$ 在平台上竞争。

### 2.7 Timing

基准模型 timing：

1. $M$ 选择经营模式，并在 marketplace 或 dual mode 下设定佣金 $\tau$。
2. $S$ 决定是否参加平台，并选择创新水平 $\Delta$。
3. $S$、$M$ 和其他卖家同时定价。
4. 消费者在观察可得产品后作出购买决策。

解概念是 Subgame Perfect Nash Equilibrium。文章还使用 equilibrium selection rule：若一个子博弈有多个均衡，先选择 $M$ 更喜欢的；若 $M$ 无差异，再选择 $S$ 更喜欢的；排除依赖弱劣策略的均衡。

### 2.8 关键约束和假设

文章使用如下假设来保证价格由竞争约束决定：

$$
\max\{b,b+\sigma,\bar{\Delta}\}<\frac{G(\nu)}{g(\nu)}.
$$

经济学直觉：

- 右边 $\frac{G(\nu)}{g(\nu)}$ 类似需求系统中的 inverse hazard rate，刻画需求对价格变化的敏感程度。
- 这个假设保证相关产品优势和平台便利收益没有大到让垄断定价逻辑主导。
- 因此均衡价格主要由竞争约束决定，而不是由内部最优垄断价格决定。这样文章可以把注意力集中在平台模式、佣金、发现机制和 price squeeze 上。

### 2.9 本部分总结

这一部分最后要强调：

模型的核心不是单纯的产品差异，而是平台同时拥有两种权力：交易便利 $b$ 和产品发现能力。正是 discovery 与 commission 的组合，使 dual mode ban 的福利效果变得不直观。

## Presenter 3：Baseline Equilibrium and Price Squeeze

### 3.1 这一部分的目标

第三位汇报人负责基准模型的求解。重点不是把所有代数细节堆上去，而是要按 backward induction 解释三种模式的均衡和 dual mode 的 price squeeze。

建议顺序：

1. Marketplace mode。
2. Seller mode。
3. Dual mode pricing subgame。
4. $S$ 的创新选择。
5. $M$ 的佣金选择。
6. 平台模式比较。

### 3.2 Marketplace Mode

在 marketplace mode 中，$M$ 只收佣金 $\tau$。$S$ 可以设置两个价格：

- inside price：$p_i$，消费者通过平台购买。
- outside price：$p_o$，消费者直接购买。

$S$ 的价格受到 fringe sellers 约束：

$$
p_i \leq \tau+\Delta,\qquad p_o \leq \tau+\Delta-b.
$$

关键逻辑是 showrooming constraint：

- 如果 $\tau \leq b$，$S$ 愿意让消费者通过平台购买。
- 如果 $\tau>b$，$S$ 会借平台让消费者发现产品，然后通过较低站外价格引导消费者直接购买。
- 因此平台无法把佣金设得超过便利收益 $b$。

Proposition 1：

$$
\tau^{mkt}=b,
$$

$S$ 参加平台并选择 $\Delta^{mkt}$，其中

$$
G(\nu)=K'(\Delta^{mkt}).
$$

均衡价格：

$$
p_i^*=b+\Delta^{mkt}.
$$

利润：

$$
\Pi^{mkt}=bG(\nu),\qquad
\pi^{mkt}=\Delta^{mkt}G(\nu)-K(\Delta^{mkt}).
$$

口头直觉：平台把佣金设到 showrooming constraint 的上限 $b$，而 $S$ 的创新边际收益来自交易规模 $G(\nu)$。

更具体地说：

- $\tau^{mkt}=b$ 表示平台最多只能抽取“平台交易便利”的价值。如果佣金更高，$S$ 会让消费者在平台上发现产品后转向直接渠道购买。
- $G(\nu)=K'(\Delta^{mkt})$ 表示 $S$ 的创新边际收益等于创新带来的交易规模收益。
- $p_i^*=b+\Delta^{mkt}$ 表明 $S$ 把平台便利 $b$ 和产品质量优势 $\Delta^{mkt}$ 都体现在平台内价格中，但仍受到 fringe sellers 的竞争约束。

### 3.3 Seller Mode

在 seller mode 中，$M$ 只卖自己的产品。消费者不能通过平台发现 $S$。

$M$ 的定价问题是：

$$
\max_{p_m\leq b+\sigma} p_m G(\nu+b+\sigma-p_m).
$$

由于竞争约束绑定：

$$
p_m^*=b+\sigma.
$$

Proposition 2：

- $M$ sells to all consumers。
- $S$ sells to no one。
- $S$ 选择最低创新 $\Delta^l$。

利润：

$$
\Pi^{sell}=(b+\sigma)G(\nu),\qquad \pi^{sell}=0.
$$

口头直觉：平台在 seller mode 中可以完全占有自己渠道带来的销售收益，但代价是消费者无法发现创新卖家。

更具体地说，$p_m^*=b+\sigma$ 表示平台把交易便利 $b$ 和自营产品相对 fringe sellers 的优势 $\sigma$ 都转化为价格。由于 $S$ 不在平台上出现，消费者无法发现其产品，$S$ 没有销售，也没有进一步创新激励。

### 3.4 Dual Mode：Pricing Subgame

Dual mode 是基准模型最重要的部分。现在平台既收佣金，又销售自营产品。

关注 $\tau\in(\max\{-\sigma,0\},b]$。定价子博弈有两个可能均衡。

#### 情形 1：Semi-seller mode equilibrium

如果

$$
\sigma \geq \Delta,
$$

平台自营产品相对 $S$ 的产品更有价值。均衡为：

$$
p_i^*=\tau,\qquad p_o^*\geq p_i^*-b,\qquad p_m^*=\tau+\sigma-\Delta.
$$

消费者都买 $M$ 的产品，$S$ 赚不到利润。

直觉：这是带垂直差异的 Bertrand 竞争。$M$ 的产品优势足以让它占领市场。

#### 情形 2：Price squeeze equilibrium

如果

$$
\Delta>\sigma,
$$

$S$ 的产品更好。消费者最终可能买 $S$，但 $M$ 的自营产品会约束 $S$ 的价格。

均衡满足：

$$
p_i^*=p_m^*+\Delta-\sigma,
$$

并且

$$
p_m^*\in
\left[
\max\{\tau-\Delta+\sigma,0\},
\tau+\min\{\sigma,0\}
\right].
$$

文章的均衡选择规则选择最低的 $p_m^*$：

$$
p_m^*=\max\{\tau-\Delta+\sigma,0\}.
$$

平台利润为：

$$
\Pi=\tau G(\nu+\sigma+b-p_m^*).
$$

这里的关键是：$M$ 不一定真的卖出自己的产品，但它的自营产品价格会约束 $S$ 的 inside price。$S$ 为了不被 $M$ 抢走消费者，必须降低平台内价格。这就是 price squeeze。

这些条件的经济学直觉如下：

- $p_i^*=p_m^*+\Delta-\sigma$ 是消费者在 $S$ 和 $M$ 之间无差异的条件。$S$ 的产品质量优势是 $\Delta-\sigma$，所以 $S$ 可以比 $M$ 贵这么多，但不能更贵。
- $p_m^*$ 的下界保证 $M$ 不用负价格销售，也保证 $S$ 的平台内价格至少覆盖佣金成本 $\tau$。
- $p_m^*$ 的上界保证 $M$ 的自营产品确实对 $S$ 构成有效竞争约束。
- $\Pi=\tau G(\nu+\sigma+b-p_m^*)$ 表明平台利润来自佣金乘以交易量。平台把 $p_m^*$ 压低，会降低 $S$ 的价格并扩大需求，从而增加佣金收入。

### 3.5 Stage 2：Innovation Constraint

$S$ 的创新选择取决于佣金 $\tau$ 是否太高。

文章定义 $\bar{\tau}$：

$$
(\bar{\Delta}-\sigma-\bar{\tau})G(\nu+b+\sigma)-K(\bar{\Delta})=0.
$$

Lemma 1：

- 如果 $\tau\leq\bar{\tau}$，$S$ 选择高创新 $\Delta=\bar{\Delta}$。
- 如果 $\tau>\bar{\tau}$，$S$ 选择最低创新 $\Delta=\Delta^l$。

口头解释：

佣金越高，$S$ 的净 margin 越低。$\bar{\tau}$ 是 $S$ 愿意进行高创新的最高佣金。它可以被称为 innovation constraint。

更具体地说，定义 $\bar{\tau}$ 的方程是在比较 $S$ 高创新和低创新的收益。第一项 $(\bar{\Delta}-\sigma-\bar{\tau})G(\nu+b+\sigma)$ 是高创新时 $S$ 的净 margin 乘以交易量，第二项 $K(\bar{\Delta})$ 是创新成本。当佣金超过 $\bar{\tau}$，高创新的净收益不足以覆盖成本，$S$ 就退回最低创新 $\Delta^l$。

### 3.6 Stage 1：Commission Choice in Dual Mode

$M$ 的佣金选择同时受到两个约束：

1. Showrooming constraint：

$$
\tau\leq b.
$$

2. Innovation constraint：

$$
\tau\leq \bar{\tau}.
$$

Proposition 3：

如果 $b\leq\bar{\tau}$，或者

$$
\bar{\tau}G(\nu+\sigma+b)
\geq
(b+\max\{\sigma-\Delta^l,0\})G(\nu+\Delta^l),
$$

则

$$
\tau^{dual}=\min\{b,\bar{\tau}\},
$$

$S$ 选择高创新 $\bar{\Delta}$，并通过平台销售。

如果 $b>\bar{\tau}$ 且上述条件不成立，则

$$
\tau^{dual}=b,
$$

$S$ 选择最低创新 $\Delta^l$。此时可能由 $S$ 销售，也可能由 $M$ 销售，取决于 $\Delta^l$ 与 $\sigma$ 的比较。

口头解释：

$M$ 面临一个 trade-off：

- 低佣金可以保护 $S$ 的创新激励，带来更高需求。
- 高佣金可以提高平台每笔交易的抽成，但可能扼杀创新。

因此，Proposition 3 的条件本质上是在比较两种平台盈利方式：

- 遵守 innovation constraint：平台牺牲一部分佣金率，但诱导 $S$ 高创新，从而扩大需求。
- 违反 innovation constraint：平台把佣金设到 showrooming constraint 上限 $b$，获得更高单笔抽成，但 $S$ 创新下降，交易量可能减少。

这也是整篇文章中最重要的经济权衡：平台有时愿意“少抽一点”，因为这能让第三方卖家创新更多、市场变大。

### 3.7 Platform Mode Choice

Corollary 1：

- Marketplace mode 与 seller mode 比较：$\Pi^{mkt}\geq\Pi^{sell}$ 当且仅当 $\sigma\leq0$。
- Dual mode 总是严格优于 marketplace mode。
- 存在阈值 $\underline{\sigma}>0$，使得

$$
\Pi^{dual}>\Pi^{sell}
\quad \text{if and only if}\quad
\sigma<\underline{\sigma}.
$$

解释：

Dual mode 优于 marketplace mode，是因为 price squeeze 让 $S$ 的价格更低，交易量更高，平台佣金收入增加。Dual mode 与 seller mode 的比较则取决于平台自营优势 $\sigma$：如果 $\sigma$ 很大，平台宁愿独占消费者；如果 $\sigma$ 不太大，平台愿意引入 $S$ 并通过佣金获利。

### 3.8 本部分总结

本部分最后要强调：

基准模型的反直觉结果来自 price squeeze。平台自营不一定只是排挤第三方，它也可能压低第三方卖家的价格，提高交易量和消费者剩余。

## Presenter 4：Banning Dual Mode in the Baseline Model

### 4.1 这一部分的目标

第四位汇报人负责讲政策反事实：如果监管禁止 dual mode，会发生什么？重点是平台会内生选择另一个模式，而不是简单地“少卖一种产品”。

### 4.2 禁令的逻辑

禁止 dual mode 后，平台只能在两种模式中选：

- Marketplace mode。
- Seller mode。

根据 Corollary 1：

- 如果 $\sigma>0$，seller mode 相对更有吸引力。
- 如果 $\sigma\leq0$，marketplace mode 相对更有吸引力。

### 4.3 Proposition 4 的核心结论

可以按三类情形讲：

#### 情形 1：$\sigma\geq\underline{\sigma}$

平台本来就选择 seller mode。禁止 dual mode 没有效果。

#### 情形 2：$0<\sigma<\underline{\sigma}$

平台原本选择 dual mode，但禁令后转向 seller mode。

结果：

- Platform profit $\Pi$ 下降。
- Consumer surplus 下降。
- Innovation 可能下降。
- Welfare 下降。

为什么福利下降？

1. 消费者失去通过平台发现 $S$ 的渠道。
2. $S$ 与 $M$ 的竞争消失，price squeeze 消失。
3. 交易数量减少。
4. 消费者无法同时享受 $S$ 的高质量产品和平台便利收益 $b$。

这也是文章认为最有现实意义的情形，因为大型平台往往有 $\sigma>0$。

#### 情形 3：$\sigma\leq0$

平台原本选择 dual mode，但禁令后转向 marketplace mode。

结果：

- Consumer surplus 仍然下降。
- Platform profit 下降。
- $S$ 的利润上升。
- Innovation 和 welfare 的变化不确定。

为什么不确定？

Marketplace mode 中，$S$ 面临较弱价格竞争，所以利润和创新激励可能更高。但消费者价格也更高，交易量更低。因此 welfare 取决于“更高创新”是否足以弥补“更少交易和更高价格”。

### 4.4 适合 slides 的政策图示

建议做一个三行表：

| 参数区域 | 禁令后平台模式 | 消费者剩余 | 福利 | 直觉 |
|---|---|---|---|---|
| $\sigma\geq\underline{\sigma}$ | Seller | 不变 | 不变 | 平台本来就不选 dual |
| $0<\sigma<\underline{\sigma}$ | Seller | 下降 | 下降 | 失去 discovery + price squeeze |
| $\sigma\leq0$ | Marketplace | 下降 | 不确定 | 创新增益 vs 价格/交易损失 |

### 4.5 本部分总结

基准模型下，禁止 dual mode 一旦有实际约束力，就总是降低消费者剩余。尤其当平台自营产品比 fringe sellers 更有效率时，禁令降低社会福利。这是文章最重要的政策反直觉。

## Presenter 5：Product Imitation, Self-Preferencing, and Policy Comparison

### 5.1 这一部分的目标

第五位汇报人负责文章后半部分：加入监管最担心的行为后，dual mode 是否仍有辩护空间？不同政策工具应该如何比较？

### 5.2 扩展模型的新设定

在 dual mode 中加入两个行为：

#### Product imitation

如果 $S$ 进入平台，$M$ 可以在定价前模仿 $S$ 的产品。最强设定是：

- imitation 是 perfect and costless。
- imitation 后 $M$ 的产品价值也变成 $\nu+\Delta$。
- $M$ 不能事先承诺不模仿。

#### Self-preferring / steering

平台可以决定是否向消费者展示 $S$。

- 如果展示，消费者知道 $S$。
- 如果不展示，消费者不知道 $S$，更可能买平台产品。

这相当于把平台的 recommendation algorithm 模型化成一个 binary steering decision。

扩展模型 timing 与基准模型类似，但 Stage 2 和 Stage 4 修改：

- Stage 2：$S$ 选择是否进入和创新水平；若 dual mode 且 $S$ 进入，$M$ 决定是否 imitate。
- Stage 4：价格设定后，$M$ 决定是否 show $S$；消费者再购买。

### 5.3 Proposition 5：Dual Mode with Imitation and Self-Preferencing

核心结论：

$S$ 总是选择最低创新：

$$
\Delta^{dual}=\Delta^l.
$$

如果 $\sigma\geq\Delta^l$：

- 平台不需要模仿。
- $M$ 设置高佣金 $\tau^{dual}=b+\Delta^l$。
- $M$ 不展示或不受 $S$ 竞争约束，卖自己的产品。
- $M$ 利润为

$$
\Pi^{dual}=(b+\sigma)G(\nu).
$$

如果 $\sigma<\Delta^l$：

- 平台可以通过高佣金或模仿完全提取 $S$ 的创新 surplus。
- 均衡结果等价于平台获得

$$
\Pi^{dual}=(b+\Delta^l)G(\nu).
$$

直觉：

加入 imitation 和 self-preferring 后，dual mode 的两个好处被破坏：

1. Self-preferring 消除了平台内有效竞争。
2. Imitation 消除了 $S$ 的创新激励。

更具体地说：

- $\Delta^{dual}=\Delta^l$ 的经济含义是，$S$ 预期高创新会被平台模仿或被平台通过推荐机制压制，因此不愿支付创新成本。
- 当 $\Pi^{dual}=(b+\sigma)G(\nu)$ 时，dual mode 的结果等同于 seller mode：平台靠自身产品优势和平台便利获利。
- 当 $\Pi^{dual}=(b+\Delta^l)G(\nu)$ 时，平台实际上把 $S$ 的基础创新价值完全转化为自己的利润，无论是通过高佣金还是通过模仿。
- 因此 Proposition 5 说明，真正伤害创新和竞争的是 imitation 与 steering 的组合，而不是 dual mode 这个身份本身。

### 5.4 Proposition 6：这时禁止 Dual Mode 是否有效？

禁止 dual mode 后：

- 如果 $\sigma\geq\Delta^l$，平台本来结果就像 seller mode，禁令无影响。
- 如果 $0<\sigma<\Delta^l$，平台转向 seller mode，消费者剩余不变，但 welfare 下降。
- 如果 $\sigma\leq0$，平台转向 marketplace mode，创新和福利上升。

这里的关键反直觉：

在有 self-preferring 和 imitation 时，禁止 dual mode 对消费者剩余不一定有帮助，因为 dual mode 中消费者原本也没有享受到有效竞争。但当 $0<\sigma<\Delta^l$ 时，禁令仍然降低 welfare，因为消费者不能结合 $S$ 的产品优势和平台便利。

经济学直觉是：结构性禁令只能改变平台“能否同时做两件事”，但不能直接恢复 $S$ 的创新激励，也不能保证消费者重新发现 $S$。如果平台转向 seller mode，市场仍然缺少创新卖家的有效竞争。因此，禁令可能没有修复真正的问题机制。

### 5.5 Behavioral Remedy 1：Ban Self-Preferencing Only

禁止 self-preferring 意味着：只要 $S$ 在平台上，$M$ 必须展示 $S$。

效果：

- Exploitative equilibrium 消失。
- Showrooming constraint 恢复。
- 平台内价格竞争恢复。
- 但 imitation 仍然存在，所以 $S$ 的创新仍为最低水平 $\Delta^l$。

Proposition 7：

- 如果 $\sigma$ 较高，平台可能转向 seller mode，结果类似禁 dual mode。
- 如果 $\sigma$ 较低，平台继续 dual mode，consumer surplus 和 welfare 上升。

直觉：

只禁 self-preferring 可以恢复竞争和降低价格，但不能恢复创新激励。

数学结果背后的经济学机制是：禁止 self-preferring 相当于强制平台展示 $S$，所以 $M$ 不能再通过隐藏 $S$ 来保护自营产品。但因为 imitation 仍然存在，$S$ 仍然预期创新会被复制，因此 innovation 不上升。这个政策主要改善的是价格竞争，而不是创新。

### 5.6 Behavioral Remedy 2：Ban Imitation Only

禁止 imitation 等价于让 $M$ 能够可信承诺不复制 $S$。

这使平台可以通过设定满足 innovation constraint 的佣金来激励 $S$ 创新：

$$
\tau\leq \bar{\tau}.
$$

如果创新足够有价值，平台选择

$$
\tau=\bar{\tau},\qquad \Delta=\bar{\Delta}.
$$

Proposition 8：

如果禁 imitation 改变平台行为，则：

- Innovation 上升。
- Consumer surplus 上升。
- Welfare 上升。
- 平台利润也可能上升，因为高创新扩大需求。

直觉：

平台有时也希望自己能承诺不模仿，因为这样才能诱导第三方卖家提供更有价值的创新产品，从而扩大平台可抽成的市场。

这里的关键经济学直觉是 commitment。没有监管时，平台事后想模仿；但正因为卖家预期平台会事后模仿，卖家事前不创新。禁止 imitation 相当于提供一种可信承诺，使平台能够通过保留卖家的创新 rents 来扩大市场规模。平台、消费者和福利可能同时受益。

### 5.7 Behavioral Remedy 3：Ban Both Imitation and Self-Preferencing

同时禁止 imitation 和 self-preferring 后，dual mode 回到基准模型的逻辑。

Proposition 9：

当平台继续采用 dual mode 时：

- Showrooming constraint 恢复。
- Innovation constraint 有效。
- $S$ 的创新激励恢复。
- Consumer surplus 和 welfare 上升。

文章强调二者有 synergistic effect：

- 禁 self-preferring 让平台不能通过隐藏 $S$ 来逃避竞争。
- 禁 imitation 让 $S$ 不担心创新被复制。
- 两者一起比单独使用更可能提高创新和福利。

经济学直觉是：self-preferring 和 imitation 分别破坏两个不同机制。前者破坏价格竞争，后者破坏创新激励。单独禁止其中一个只修复一半问题；同时禁止二者，才同时恢复 showrooming constraint、price squeeze 和 innovation constraint。

### 5.8 Corollary 2：Behavioral Remedies vs Structural Ban

这是政策结论的核心。

当 $\sigma>0$，也就是平台自营产品更有效率时，禁止 dual mode 后平台会转向 seller mode。相对于这种 structural ban，行为监管通常弱改进：

- Ban self-preferring：若平台继续 dual mode，则 CS 和 welfare 上升。
- Ban imitation：若诱导创新，则 CS、innovation 和 welfare 上升。
- Ban both：在平台继续 dual mode 的区域，CS、innovation、welfare 都上升。

当 $\sigma\leq0$ 时，结论更复杂，因为 structural ban 可能把平台推向 marketplace mode，并提高创新。但文章认为这不是最有经验相关性的情形。

### 5.9 本部分总结

加入 imitation 和 self-preferring 后，文章并不是否认监管问题。相反，它承认这些行为会伤害创新和竞争。但文章认为问题应该精准定位：

- Product imitation 损害创新激励。
- Self-preferring 损害平台内竞争。
- Dual mode 本身还可能包含有益的价格竞争和交易便利。

因此，最好的政策不是简单禁止 dual mode，而是限制具体扭曲行为。

## 6. 全场汇报的衔接建议

### 6.1 五人之间如何过渡

Presenter 1 到 Presenter 2：

“要判断禁令是否有效，不能只看现实案例，需要一个模型来比较平台在不同经营模式下的选择。”

Presenter 2 到 Presenter 3：

“有了这些 primitives 和 timing 后，我们用 backward induction 求解三种平台模式。”

Presenter 3 到 Presenter 4：

“既然 dual mode 在基准模型中可能带来 price squeeze 和消费者收益，那么直接禁止它会怎样？”

Presenter 4 到 Presenter 5：

“到目前为止还没有考虑监管者最担心的 imitation 和 self-preferring。加入这些行为后，结论会不会反转？”

### 6.2 适合 40 分钟汇报的时间安排

建议时间分配：

- Presenter 1：6 分钟。
- Presenter 2：9 分钟。
- Presenter 3：11 分钟。
- Presenter 4：6 分钟。
- Presenter 5：8 分钟。

虽然有 5 位成员，但理论重点集中在 Presenter 2 和 Presenter 3，因此这两部分应略长。

### 6.3 建议 slides 结构

建议总页数控制在 30-38 页左右：

1. Title。
2. Motivation。
3. Research question。
4. Main message。
5. Model overview。
6. Players and values。
7. Discovery and channels。
8. Timing。
9. Marketplace mode equilibrium。
10. Seller mode equilibrium。
11. Dual mode pricing subgame。
12. Price squeeze mechanism。
13. Innovation constraint。
14. Dual mode equilibrium。
15. Platform mode choice。
16. Ban dual mode: setup。
17. Ban dual mode: results。
18. Welfare intuition。
19. Imitation and self-preferring setup。
20. Dual mode with imitation and steering。
21. Why structural ban is limited。
22. Ban self-preferring。
23. Ban imitation。
24. Ban both。
25. Policy comparison。
26. Conclusion。

### 6.4 最后总结页

最后一页可以写：

Main takeaway:

平台 dual mode 有两面性。一方面，它可能带来 price squeeze、更多交易和更高消费者剩余；另一方面，product imitation 和 self-preferring 会削弱创新与竞争。因此，监管应优先限制具体行为，而不是直接禁止平台同时运营 marketplace 和销售自营产品。
