# Kill Test Casebook — Idea 死亡档案馆

> v4.0 新增。10+ 个真实/类真实 idea 的 kill test 历史档案，带评级验证+墓志铭。

**为什么需要这个卫星**：Kill test 的价值不在于推理链条本身，而在于 **对模式识别的沉淀**。一个创始人看 5 个案例比读 50 条原则更能内化判断力。本文件收录已评估的 idea、它们的评级、事后验证（如果有）、以及可以复用的模式。

**案例来源**：
- 真实公司（已公开信息）
- 脱敏用户提交的 idea
- 经典教学案例（YC / a16z 博客 / 知名创始人访谈中的典型错误）

**引用原则**：真实公司案例基于公开信息；脱敏案例加「模式画像」标签。

---

## 案例 1：Markdown & Obsidian Native AI NAS — 评级 C（Kickstarter）

### 一句话描述
一个为 Obsidian/markdown 重度用户设计的、永远在线、本地 AI 运行的家庭 NAS 设备。

### 十发子弹体检

| # | 子弹 | 判定 | 一句话理由 |
|---|------|------|-----------|
| B1 | TAM | 🔴 | Obsidian 全球付费用户 ~200 万，愿意为专用硬件付费的 < 5% → TAM < $100M |
| B2 | 品类定义 | 🟡 | 「AI NAS」自带低毛利硬件锚定 |
| B3 | 硬件/软件价值 | 🔴 | 核心价值在通用计算能力，硬件盒子只是外壳 |
| B4 | 用户就绪度 | 🟢 | 目标用户存在且可触达（Obsidian 社区） |
| B5 | 平台风险 | 🔴 | 夹在 Apple/Mac mini（上层）+ 开源模型（底层）之间 |
| B6 | 早期/晚期悖论 | 🟡 | 早期用户 DIY（Mac mini + Obsidian 自建），晚期大众不懂 |
| B7 | 技术 story | 🟢 | 无自研芯片叙事风险 |
| B8 | 递归收入 | 🟡 | 纯一次性硬件销售 |
| B9 | 团队匹配 | 🟢 | 团队有硬件+软件基因 |
| B10 | 竞品=不买 | 🔴 | Mac mini + Ollama + Obsidian 的 DIY 组合 < 2x 你的产品价格 |

**3 🔴 + 3 🟡 → 评级 C**

### 六人投委会投票

| Persona | 投票 | 一句话 |
|---------|------|-------|
| P1 异端猎手 | PASS | 「有 insight（personal AI infra 是真趋势）但实现方式太 crowded」 |
| P2 增长机器 | KILL | 「TAM 太小，单位经济学不成立」 |
| P3 场景赌徒 | PASS | 「Personal AI 的 why now 对，但你不是这一代的答案」 |
| P4 现金流 | KILL | 「没有 paying users 证据，纯 PPT」 |
| P5 国产替代 | PASS | 「赛道不在政策框架里」 |
| P6 社区 | PASS | 「没 demo，但 Obsidian 社区可以转发」 |

**0 FUND + 2 KILL + 4 PASS → 共识否决**

### 真实洞察
- **对了的**：Personal AI Infrastructure 是真趋势；Markdown 是 LLM 的母语；永远在线 Agent 需要专用设备
- **错了的**：把洞察包装成消费硬件产品

### Pivot 方向

| Pivot | 换掉 | 保留 |
|-------|------|------|
| A：Obsidian native AI plugin（软件 SaaS） | 硬件 | Obsidian 重度用户 + AI 助理 |
| B：企业级 Personal AI Infra（B2B） | 消费市场 | Personal AI + 本地化 |
| C：Mac mini 预装镜像 + 服务订阅 | 硬件生产 | 重度用户的开箱即用体验 |

### 墓志铭
> 「Obsidian Native AI NAS 是一个 **C 级** 的 idea：洞察对了，包装错了。如果非要做，转成 Mac mini 预装镜像 + 订阅服务，把硬件的投入换成分发的规模。」

---

## 案例 2：AI 法律助手（to C，面向个人用户）— 评级 C（Kickstarter / 小生意）

### 一句话描述
一个面向个人用户的 AI 法律咨询助手，帮他们起草合同、回复诉讼、处理租房纠纷。

### 子弹体检速览
- B1 TAM：🟡（个人法律咨询市场大但付费率低）
- B6 早期/晚期：🔴（早期 = 律师自己用做效率工具；晚期 = 普通人遇到法律问题太低频）
- B10 竞品=不买：🔴（ChatGPT + Google 组合已经能解决 80% 轻量问题）

### 投委会
- P2 KILL（「frequency 问题无解，LTV 算不出来」）
- P4 KILL（「to C 法律 SaaS 的 retention 从来就没成过」）
- 0 FUND + 2 KILL → 共识否决

### 模式教训
**「to C + 低频专业服务」是 VC 赛道的结构性黑洞。** 解决这个问题的公司通常最后变成：
1. B2B（服务律师、服务法律援助机构）
2. 媒体（内容 → 线索 → 人工律师成交）
3. 保险（把低频需求打包为订阅）

### 墓志铭
> 「to C 法律助手是 **C 级** idea：真需求存在，但频率错配。VC 赛道走不通。转 B2B 或内容+线索模式。」

---

## 案例 3：Cursor-but-for-designers — 评级 B（需要 Pivot）

### 一句话描述
一个 AI-native 的 Figma 竞品，让设计师用自然语言驱动设计迭代。

### 子弹体检
| # | 判定 | 理由 |
|---|------|------|
| B1 TAM | 🟢 | Figma $20B 估值、全球设计师市场巨大 |
| B2 品类 | 🟡 | 「Cursor for X」已经被多家占位 |
| B3 硬件/软件 | 🟢 | 纯软件 |
| B5 平台风险 | 🟡 | 底层依赖 GPT/Claude 等第三方模型 |
| B9 团队匹配 | 🟡 | 需要同时懂设计 + 懂 AI + 懂 browser performance |
| B10 竞品=不买 | 🟡 | Figma 自己做 AI 功能的速度 |

**0 🔴 + 4 🟡 → 评级 B**

### 投委会
- P3 FUND（「AI + design tools 是真 inflection，timing 对」）
- P6 FUND（「designer 社区有 viral 潜力」）
- P2 PASS（「distribution 打不过 Figma」）
- P1 PASS（「这不是 contrarian，是 bet on execution」）
- **2 FUND + 0 KILL → 可融，需找 P3/P6 类型**

### 策略建议
- **找 a16z / Lerer Hippeau** 类型，避开 Sequoia / Founders Fund
- 先做 wedge 产品（如「自动布局生成」或「设计系统管理」），不要一开始打 Figma replacement
- 社区先行：在 X / Dribbble / Figma 社区持续输出 → 建立 designer 创始人信任
- 融资轮次：先拿 $2-3M seed，做 12 月 wedge 验证，再考虑 Series A 打全产品

### 墓志铭
> 「Cursor-for-designers 是 **B 级** idea：需求真，timing 真，但 distribution 是死线。找对 VC（thesis-driven + 社区嗅觉）+ 先做 wedge 产品，有打法。」

---

## 案例 4：人形机器人家庭陪伴（to C）— 评级 D

### 一句话描述
一个 1 米高的人形机器人，主打家庭陪伴、儿童教育、老人看护。

### 子弹体检
- B1 TAM：🟡（看起来大但付费意愿极低）
- B3 硬件/软件：🔴（硬件 BOM 成本极高，软件能力依赖基础模型进展）
- B4 用户就绪度：🔴（「家庭机器人」市场需要 5+ 年教育）
- B5 平台风险：🔴（硬件 + 基础模型 + 内容 三层全是上游风险）
- B9 团队匹配：🔴（需要硬件 + 软件 + 内容生态三栖团队）

**4 🔴 → 评级 D**

### 投委会
- P2 KILL、P4 KILL、P5 KILL（注：中国产业资本可能不 KILL，但 to C 场景下 P5 也 KILL）
- **3 KILL → 共识否决**

### 真实洞察
- Personal robotics 是真赛道，但入口不是「家庭陪伴」，是 **单任务专用机器人**（扫地、物流、工业）

### 三条 Pivot
- A：单任务厨房机器人（B2B 餐饮连锁）
- B：老人看护的 companion AI（软件 app + 摄像头，不是硬件机器人）
- C：儿童教育玩具（降低价格+简化功能，不是「陪伴机器人」）

### 墓志铭
> 「人形陪伴机器人是 **D 级** idea：技术路径不可行，市场不 ready。赛道对，形态全错。Pivot 到单任务机器人或软件陪伴。」

---

## 案例 5：Crypto Wallet for Normies — 评级 B（需要 Pivot）

### 一句话描述
一个面向 crypto 小白的、极简体验的 wallet 产品，强调「比银行 app 还好用」。

### 子弹体检
- B1 TAM：🟢（crypto 用户基数大）
- B2 品类：🟡（「crypto wallet」这个词让非 crypto 用户望而却步）
- B4 用户就绪度：🔴（「让小白用 crypto」过去 5 年多次失败）
- B10 竞品=不买：🟡（Coinbase / Kraken / Binance 已经在做 wallet 功能）

**1 🔴 + 2 🟡 → 评级 B**

### 投委会
- P1 FUND（「如果真能让 normie 用起来，contrarian bet」）
- P6 FUND（「crypto 社区对好 UX 的 wallet 一直有期待」）
- P4 KILL（「5 年没人做成，你为什么不一样？」）
- **2 FUND + 1 KILL → 极化**

### 策略建议
- 极化型 idea → **绝对不能从会 KILL 的 persona 开始**（禁止 pitch 任何 PG/YC 类型做 R1）
- 从 crypto-native VC 开始（Paradigm / a16z crypto / Polychain）
- 拿到 1 个 crypto-native lead 后，才能扩展到非 crypto VC

### 墓志铭
> 「Crypto wallet for normies 是 **B 级 极化** idea：要么是下一个 Venmo，要么是第 20 个失败案例。序列极其重要，先找 crypto-native 锚投资人。」

---

## 案例 6：AI-Generated Podcast 工厂 — 评级 D

### 一句话描述
一个用 AI 生成播客内容的平台，每天自动产出 1000+ 集 niche 播客。

### 子弹体检
- B1 TAM：🟡（播客市场大但已被 Spotify/Apple 整合）
- B2 品类：🔴（「AI 生成内容」在 2025-2026 已经 commoditize）
- B4 用户就绪度：🟡（听众对 AI 生成内容的辨识度和抵触度上升）
- B10 竞品=不买：🔴（用户已经习惯人类主播，切换成本高）

**2 🔴 + 2 🟡 → 评级 D**

### 真实洞察
- 问题不在「AI 能不能生成播客」，问题在「人类为什么要听 AI 生成的播客」

### 墓志铭
> 「AI podcast 工厂是 **D 级** idea：技术可行，需求不存在。Pivot 到 AI 辅助人类主播（tool，not replacement）。」

---

## 案例 7：Healthcare Startup 以 AI 诊断为 wedge — 评级 C

### 一句话描述
一个 AI 医疗诊断助手，对标皮肤科/眼科/放射科的早期筛查。

### 子弹体检
- B1 TAM：🟢
- B2 品类：🟡（「AI medical diagnosis」已被 20+ 公司占位）
- B4 用户就绪度：🔴（FDA 审批 + 医院采购 + 医生信任三重墙）
- B9 团队匹配：🔴（缺医疗行业资源的团队做 healthcare AI → 极高失败率）

### 模式教训
Healthcare AI 的 pattern 几乎全是「技术通过 + 商业化死」：
- 数据获取难（隐私 + HIPAA）
- 监管路径长（FDA approval 3-5 年）
- 销售周期长（医院采购 2-3 年）
- 支付方博弈复杂（保险公司 + Medicare + 医院）

### 墓志铭
> 「Healthcare AI 诊断是 **C 级** idea：不是 VC 赛道，是 strategic acquirer 赛道。Pivot 到给医院提供效率工具（不碰诊断），或被 Epic/Cerner/Verily 收购为终局设计。」

---

## 案例 8：Shopify for X（垂直电商工具）— 评级随品类

### 模式画像
「Shopify for [restaurants / creators / niche industry]」是一个家族，评级高度依赖具体品类：

| 品类 | 评级 | 关键差异 |
|------|------|---------|
| Shopify for restaurants（POS + 线上点单 + 配送） | B+ | Toast/Square 已抢占，但 niche 仍有机会 |
| Shopify for creators（creator 专用电商） | C+ | Gumroad/Stan Store/Beacons 已 crowded |
| Shopify for B2B industrial | B | TAM 巨大，打法复杂 |
| Shopify for legal services | D | 监管限制+低频 |

### 墓志铭
> 「Shopify for X 是一个需要非常具体 vertical 的模板。抽象评级不存在——每个 X 需要单独做 kill test。」

---

## 案例 9：碳中和 SaaS（给企业做 ESG 报告）— 评级 B

### 子弹体检
- B1 TAM：🟢（监管驱动，企业 ESG 报告强制化）
- B3 硬件/软件：🟢
- B4 用户就绪度：🟢（监管窗口已开）
- B10 竞品=不买：🟡（Excel 手工 + 咨询公司组合是主要竞品）

**0 🔴 + 1 🟡 → 评级 B+**

### 投委会
- P2 FUND（「监管驱动的 SaaS 有 sticky 属性」）
- P5 FUND（「政策对齐」）
- P3 PASS（「不是 technology inflection」）
- **2 FUND + 0 KILL → 可融**

### 策略建议
- 聚焦一个监管明确的国家先做（EU CSRD 最强制）
- B2B SaaS 经典打法：ACV $30-100K，enterprise sales
- 避免打成咨询公司模式

### 墓志铭
> 「碳中和 SaaS 是 **B+ 级** idea：不性感但扎实。找 P2/P5 双喜欢的 GP，走 enterprise SaaS 经典打法。」

---

## 案例 10：硬件众筹类（DIY 小众硬件）— 评级 C

### 模式画像
各种「我做了一个很酷的小众硬件」——机械键盘、便携相机、AI 相框等。

### 评级规律
- 几乎必 C 级（不是 VC 赛道，是 Kickstarter / DTC 赛道）
- B1 🔴（TAM 太小）
- B5 🟡/🔴（分发渠道风险）
- B8 🟡（一次性销售）

### 墓志铭
> 「DIY 硬件基本都是 C 级——不要找 VC，直接上 Kickstarter 或做 DTC 品牌。硬件 VC 只投 B1 TAM ≥ $5B 且有平台属性的硬件。」

---

## 模式库：经常被 miss 的致死模式

| 模式 | 描述 | 典型案例 | 为什么 VC miss |
|------|------|---------|-------------|
| **分销三明治** | 夹在一个即将吞噬你的平台 + 一个必须依赖的底层提供方之间 | 2015-2018 各种 Twitter 客户端、各种 Facebook Platform 应用 | 创始人低估平台的 will to compete；VC 因为看到 traction 而 miss 结构风险 |
| **Toy 看起来** | 表面看起来不像 serious 公司，实际是下一代 category definer | 早期 Twitter、Snapchat、TikTok | VC 根据「看起来 serious」做 pattern match，错过真正 disruptive 的 toy pattern |
| **Founder-problem mismatch** | 创始人背景跟问题域不匹配，但他们相信自己能 crash course | 很多 healthcare/deep tech 非 domain 创始人 | VC 因「founder seems smart」而给机会，但执行时两年 gap 没法填 |
| **Market that doesn't exist yet** | 创始人在做的 category 还不存在，需要市场教育 | AR/VR 早期、元宇宙、AI agent 早期 | 太早 = 时间/钱烧完 category 还没来 |
| **B2C high-frequency false positive** | 看起来高频，实际 session 太短无法商业化 | 大量早期冥想 app、闹钟 app | 早期 DAU 高但 LTV 低到无法支撑 CAC |

---

## 给创始人的 Self-Test 流程

用本 Casebook 自测你的 idea：

1. **先找 3 个最像的案例** — 不是商业模式最像，是 **结构最像**
2. **看这 3 个案例的致死模式** — 你是否踩了同一个
3. **看这 3 个案例的 pivot 方向** — 哪条 pivot 对你适用
4. **看这 3 个案例的墓志铭** — 你的墓志铭长什么样？如果写出来你觉得羞耻 → 早下船

**残酷但诚实**：大部分 idea 都能在本 Casebook 里找到至少一个结构近亲。如果你找不到，要么你真的 novel（0.5% 概率），要么你还没看清自己的结构（99.5% 概率）。

---

## changelog

- v1.0 2026-04-17：首版。10 个已评估 idea 的档案（含真实公司/脱敏 idea/经典教学案例）。模式库收录 5 种经常被 miss 的致死模式。Self-Test 流程。
