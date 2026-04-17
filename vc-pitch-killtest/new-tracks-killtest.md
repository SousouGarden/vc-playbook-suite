# New Tracks Kill Test — 2025-2026 新赛道子弹调整

> v4.0 新增。与主文件 Phase 1 十发子弹绑定使用。

**为什么需要这个卫星**：主文件的 B1-B10 子弹是通用框架，假设 idea 在相对成熟的 VC 赛道（SaaS / 消费硬件 / fintech 等）。但 2025-2026 年有几个新赛道的博弈规则结构性不同：

- 用主文件子弹评估会得出误导结论（例如：AI Agent 用 B1 TAM 去评估会 miss 平台延展性）
- VC 的评估标准也已变化（例如：具身智能可以 pre-revenue 融 ¥10 亿+，传统硬件 pre-revenue 不可能）
- 新 Persona 可能需要引入（例如：American Dynamism 派系 vs 原 P1 异端猎手）

本文件按赛道列出 **B1-B10 子弹的调整**、**新增/隐藏的子弹**、**Persona 权重调整**。

---

## Track A：AI Agent / LLM 应用层

### 赛道特征
- 产品层有明显 commoditization 风险（每家都在做「Cursor for X」）
- 底层模型是第三方（OpenAI/Anthropic/Google），平台风险极高
- 分发壁垒成为主要护城河（distribution > technology）
- Moat 主要在：用户数据反馈循环、垂直深度、integrations

### B1-B10 子弹调整

| # | 调整 | 原因 |
|---|------|------|
| B1 TAM | ⬆️ 提高阈值：从 $1B 提到 $5B | 通用 agent 赛道玩家太多，TAM 需要容得下 10 家同类公司 |
| B2 品类 | 「AI-native X」不再是差异化，变成品类入场券 | 2025 后每家产品公司都要 AI-native |
| B3 硬件/软件 | 不适用 | 纯软件 |
| B5 **平台风险** ⚠️ | **新增权重**：模型供应商的 will to compete | OpenAI 的 GPT Store、Anthropic 的 MCP、Google 的 Gemini—任何一个上游都可能直接做你做的事 |
| B7 **技术 story** | 🟡 阈值下调：「我们有 custom model」默认为 flag | 除非证明 data flywheel 存在，自研模型通常是 burn rate 黑洞 |
| B8 递归收入 | ⬆️ 要求更高：SaaS MRR + usage-based | Token 成本 passthrough 必须被 handle |
| B10 竞品=DIY | 🔴 阈值严格：ChatGPT + API 组合能替代 = 致命 | Prosumer 用户的 DIY 能力极强 |

### 新增子弹

| B_new | 问题 | 致死阈值 |
|-------|------|---------|
| **B11 Data Moat** | 产品使用产生的数据能否独占+反哺模型？ | 没有数据反馈循环 = 🔴 |
| **B12 Distribution Wedge** | 你有没有一条非付费的获客路径？（社区/API/开源/第三方 integration） | 纯依赖付费获客 = 🟡 |
| **B13 Model Agnosticism** | 产品能不能在 2 周内切换到不同模型？ | 与单一模型深度耦合 = 🟡 |

### Persona 权重调整

| Persona | 主文件权重 | AI Agent 权重 | 调整原因 |
|---------|----------|-------------|---------|
| **P1 异端猎手** | 中 | **低** | AI app 很少真正 contrarian，大部分是 me-too with wedge |
| **P2 增长机器** | 高 | **极高** | PLG 数据 + 单位经济学是主要 screening |
| **P3 场景赌徒** | 高 | 中 | Timing story 被说烂了，投资人对「why now」麻木 |
| **P4 现金流** | 中 | **高** | 早期 MRR + retention 是唯一硬信号 |
| **P6 社区** | 中 | **高** | HN/X 社区验证是低成本 diligence 工具 |

### 特殊警示
- **2026 Q2 开始**：多家一线 VC 对 AI app 赛道估值已经开始下修。2024 年的 thesis-driven 打法在 2026 年行不通
- **新的鬼魂**：Cursor / Perplexity / Lovable 的早期轮是 2025-2026 VC 的 anti-portfolio 主打。创始人要利用「你错过了 Cursor 的 $20M round」的结构

---

## Track B：具身智能 / 人形机器人

### 赛道特征
- Pre-revenue 可融 ¥5-15 亿（中国）/ $50-500M（美国）
- 估值与基本面脱钩，纯 FOMO 驱动
- 技术路径未收敛（模块化 vs 端到端、大模型大脑 vs 专用模型）
- 商业化路径未清晰（B2B 工业 / B2B 服务 / B2C 家庭全部在探索）

### B1-B10 子弹调整

| # | 调整 | 原因 |
|---|------|------|
| B1 TAM | ⬆️ 阈值提至 $50B+ | 本赛道资本消耗极大，TAM 不够大无法支撑烧钱速度 |
| B3 硬件/软件 | 硬件 vs 软件 **都重要**，但 software determinism 更稀缺 | 硬件 BOM 可买，软件大脑是真 moat |
| B4 用户就绪度 | 🟡 默认状态 | 几乎所有 humanoid 项目都在 education 期 |
| B6 早期/晚期 | 暂时不适用 | 赛道整体还在 demo 阶段，没有「早期晚期用户」分层 |
| B9 团队匹配 | 🔴 严格要求三栖 | 硬件 + 软件 + 仿真/数据 三重能力缺一不可 |

### 新增子弹

| B_new | 问题 | 致死阈值 |
|-------|------|---------|
| **B14 Demo 真实性** | Demo 能否在 VC 办公室现场复现？ | 实验室外跑不通 = 🔴 |
| **B15 Data Moat** | 有没有独占的物理世界训练数据？ | 纯 simulation 数据 = 🟡 |
| **B16 Commercial Landing** | 有没有一个清晰的「Year 2 商业化」场景？ | 只讲愿景不讲场景 = 🟡 |
| **B17 CVC 锁定风险** | 有没有接受车企 CVC 的排他条款？ | 接受排他 = 🟡（商业化路径被锁） |

### Persona 权重调整

| Persona | 主文件权重 | Humanoid 权重 | 调整原因 |
|---------|----------|-------------|---------|
| P1 异端猎手 | 中 | 高 | Humanoid 本身就是 contrarian bet |
| P2 增长机器 | 高 | **低** | 无 Excel 可做，P2 通常是被说服方非领投方 |
| P3 场景赌徒 | 高 | **极高** | Technology inflection + timing 是 thesis 的核心 |
| P5 战略资本 | 中 | **高** | 车企+政策+产业链协同 |
| P6 社区 | 低 | 中 | Twitter/X 上 humanoid demo 的 viral 潜力 |

### 特殊警示
- **FOMO 过热阶段**（2025-2026）：估值 bubble 明显，pre-revenue 融 $500M 不罕见
- 创始人陷阱：**不要接受「战略绑定+排他」的车企 CVC**，商业化路径会被锁
- 下行风险：一旦 2 个头部公司的 demo 被证伪或无法量产，整个赛道估值腰斩

---

## Track C：AI + 生物/医药（TechBio）

### 赛道特征
- 研发周期超长（5-15 年）
- 资本消耗极大（$100M-1B 才能到临床 III 期）
- 退出路径主要是被 Big Pharma 收购（不是 IPO）
- VC 内部有专门的 TechBio / Healthcare Fund（不是通用 VC）

### B1-B10 子弹调整

| # | 调整 | 原因 |
|---|------|------|
| B1 TAM | 看具体疾病 TAM，但要求 **disease-specific** 叙事 | 「AI for drug discovery」太宽泛 |
| B2 品类 | 「AI-driven drug discovery」本身是通用叙事，需要具体靶点/疾病 | 2020-2025 已有大量失败案例 |
| B8 递归收入 | 不适用 | TechBio 走 licensing + milestones + royalty |
| B10 竞品=不买 | 对标 Big Pharma 自研流水线 | 大药厂内部团队是结构性竞品 |

### 新增子弹

| B_new | 问题 | 致死阈值 |
|-------|------|---------|
| **B18 Regulatory Path** | 靶点 / 适应症的 FDA 监管路径是否清晰？ | 没有可对标的审批路径 = 🔴 |
| **B19 Clinical Validation** | 有没有 preclinical / in vivo 数据？ | 纯 AI prediction 无 wet lab validation = 🔴 |
| **B20 Pharma Partnership** | 有没有 Big Pharma 的 research collaboration？ | 纯 outside 开发 = 🟡 |

### Persona 调整
- 通用 Persona 全部低权重
- 需要引入 **P7 科学理事会**（TechBio 投资的特殊 Persona，要求 Chief Scientific Officer 层级的学术验证）

---

## Track D：DePIN / Crypto Infrastructure

### 赛道特征
- 混合了硬件 + 软件 + token incentive
- 分发依赖 token economics
- 法律结构复杂（token 是 security 还是 utility）
- VC 退出路径包括 token unlock（不是 IPO）

### B1-B10 子弹调整

| # | 调整 | 原因 |
|---|------|------|
| B1 TAM | ⬆️ 需要包含 crypto + 传统 TAM | DePIN 叙事通常对标 $10-100B 传统市场 |
| B3 硬件/软件 | 硬件是「入场成本」，软件+token 是价值 | 硬件越便宜越好 |
| B8 递归收入 | **Token-based** 递归 | 不是 SaaS MRR，是 token velocity + retention |

### 新增子弹

| B_new | 问题 | 致死阈值 |
|-------|------|---------|
| **B21 Token Design** | Token 的供需机制能否承担 10x 估值？ | Ponzinomics = 🔴 |
| **B22 Physical Moat** | 网络 physically 上分布有多广？能不能被 Copy+Paste？ | 硬件可 commodity 购买 = 🟡 |
| **B23 Regulatory Risk** | Token 的法律结构在哪个司法管辖区？ | US + 无法律架构 = 🔴 |

### Persona 调整
- 通用 P1-P6 全部低权重
- 引入 **P8 Crypto-Native VC**（Paradigm / a16z crypto / Multicoin / Polychain）

---

## Track E：Vertical SaaS（2026 新一代）

### 赛道特征
- 垂直行业的 workflow automation + AI
- TAM 看起来小（single vertical），但可以 stack verticals
- LTV:CAC 的 payback period 是核心指标
- 退出通常是 strategic acquirer（非 IPO）

### B1-B10 子弹调整

| # | 调整 | 原因 |
|---|------|------|
| B1 TAM | ⬇️ 可降到 $500M-$1B 单 vertical | Vertical SaaS 的 TAM 标准不同 |
| B9 团队匹配 | 🔴 严格要求 domain founder | 没有 vertical 资深 founder = 打不穿 |
| B10 竞品=不买 | 对标 Excel / 现有软件堆叠 | Vertical 里 incumbent 多但 workflow 多已过时 |

### 新增子弹

| B_new | 问题 | 致死阈值 |
|-------|------|---------|
| **B24 Workflow Depth** | 深入几层 workflow？表面工具 or end-to-end system？ | 只能替代表层 = 🟡 |
| **B25 ACV 潜力** | 能做到 $30K+ ACV 吗？ | 只能做 $5K ACV = 🟡 (SMB 赛道 VC 不喜欢) |

---

## Track F：Climate Tech / Hard Tech（能源/新材料/碳中和）

### 赛道特征
- 资本密集，需要政府补贴/碳税/监管驱动
- 技术风险 + 市场风险 + 监管风险三重
- 退出路径包括战略资本收购、政府资本接盘

### B1-B10 子弹调整

| # | 调整 | 原因 |
|---|------|------|
| B1 TAM | ⬆️ 要求 $100B+（climate 的 $ 单位级别） | 能源/工业品市场本身就是万亿级 |
| B3 硬件/软件 | 硬件 dominant | 纯软件 climate 公司 = 咨询公司伪装 |
| B8 递归收入 | 不适用 | 多数是 project-based + long-term PPA |
| B9 团队匹配 | 🔴 严格要求 technical founder（能源/化工/材料博士） | 商业背景 climate founder 极高失败率 |

### 新增子弹

| B_new | 问题 | 致死阈值 |
|-------|------|---------|
| **B26 Policy Tailwind** | 有没有明确的政府补贴/监管驱动？ | 纯市场驱动 = 🔴 |
| **B27 Capex Intensity** | 首条 commercial scale 生产线 capex 多少？ | $500M+ 且无 off-take agreement = 🔴 |
| **B28 Off-take Agreement** | 有没有潜在客户的预签约？ | 纯 speculative = 🟡 |

---

## 赛道跨界 idea 的处理

如果 idea 跨界（如：AI + biotech、DePIN + climate、humanoid + AI agent），处理原则：

1. **按主导赛道打 kill test**
2. **附加次要赛道的增量子弹**
3. **Persona 集合取并集**（不是交集）
4. **警示**：跨界 idea 的 VC 通常只有 thesis-driven fund 看（a16z / Khosla / Lux），avoid 通用基金

---

## 使用建议

1. **判断 idea 所在 Track**：
   - AI app / LLM wrapper → Track A
   - 机器人/具身智能 → Track B
   - AI + 药 → Track C
   - Crypto + 物理网络 → Track D
   - 垂类 SaaS → Track E
   - 能源/材料/气候 → Track F
   - 其他 → 主文件默认子弹

2. **用调整后的子弹重跑 Phase 1**：某些原本 🔴 的子弹在新赛道下可能不适用；某些 🟢 的子弹在新赛道下变 🔴

3. **用调整后的 Persona 权重重跑 Phase 2**：通用权重会误判

4. **Phase 2.5 博弈层的调整**：
   - Track A/B 的 FOMO 级联特别强（用好）
   - Track C 的路演序列必须先找 TechBio 专精 fund
   - Track D 的路演必须从 crypto-native VC 开始
   - Track F 的主攻对象是 American Dynamism / 国资战略资本

---

## changelog

- v1.0 2026-04-17：首版。6 个 track（AI Agent / Humanoid / TechBio / DePIN / Vertical SaaS / Climate）。每个 track 给 B1-B10 子弹调整、新增专属子弹、Persona 权重表、跨界 idea 处理、特殊警示。
