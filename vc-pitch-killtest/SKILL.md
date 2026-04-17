---
name: vc-pitch-killtest
version: v4.0
description: >-
  Fundraising war-game simulator disguised as a startup idea evaluator.
  Use when user proposes a business idea, product concept, or asks "would this work as a startup",
  "can we pitch this to VC", "is this a good idea", or wants to stress-test a business concept.
  Phase 1: 10-bullet kill test. Phase 2: 6 VC persona verdicts (P1-P6) with irrational deal-breakers,
  internal champion dynamics, and auto-generated boardroom debate scripts.
  Phase 2.5: Full game-theory layer — temporal dynamics, information warfare, pitch sequencing,
  anti-portfolio exploitation, DD counter-intel, FOMO cascade. Phase 3: Constructive pivot suggestions.
  Sister skills: founder-fundraising-wargame (US founder chair), china-fundraising-wargame (中国三体棋盘),
  term-sheet-negotiator (post-TS), vc-due-diligence-simulator (DD phase), board-dynamics-wargame (post-close).
---

# VC Pitch Kill Test v4.0 — 十发子弹 × 六人投委会 × 融资战役推演

## Changelog

| 版本 | 日期 | 范式 | 核心变动 | 位置 |
|------|------|------|---------|------|
| **v4.0** | 2026-04-17 | **骨架+卫星** | 主文件瘦身到骨架，扩展拆到 4 个卫星文件（persona-debate/anti-portfolio/casebook/new-tracks） | `SKILL.md`（live） |
| v3.0 | — | 博弈引擎（内嵌） | 十发子弹+六人投委会+六层博弈引擎写入主文件（460 行） | 未归档 |

> **演进心法**：v3 把所有能力塞进单文件，负载太重；v4 改为「主文件只留最小工作集，扩展按需加载」。日常迭代 Git 追踪；下次范式切换（若有）才 snapshot 到 `archive/`。
>
> **设计哲学**：Idea 是牌面，Game 是牌局，Persona 是对面的脸，Casebook 是你死过的样子。四层可叠加，主文件只留最小工作集。

## 触发条件

用户提出产品/创业 idea 并想评估 VC 可融资性时触发。也适用于：众筹可行性、天使轮 pitch、内部孵化立项评审、竞品 thesis 评估。

## 卫星文件索引

| 卫星 | 何时加载 | 用途 |
|------|---------|------|
| `persona-debate-scripts.md` | Phase 2 投票后 | 生成 P1-P6 投委会辩论逐字剧本（开场→进攻→防守→拍板三幕） |
| `anti-portfolio-ghosts.md` | Phase 2.5d 反悔鬼魂 | 按赛道分类的 VC 典型 anti-portfolio 档案+触发话术 |
| `kill-test-casebook.md` | 任何时候 | 10+ 个真实 idea 的 kill test 历史档案，含评级验证+墓志铭 |
| `new-tracks-killtest.md` | idea 属于新赛道 | AI Agent/具身智能/Crypto/SaaS/DePIN 等 2025-2026 新赛道的子弹调整 |

---

## Phase 0：收集上下文（< 2 分钟）

| 信息 | 必须 | 说明 |
|------|------|------|
| 产品一句话描述 | ✅ | 「给谁、解决什么问题、怎么解决」 |
| 团队现有能力 | ✅ | 技术基因、行业资源、现金状况 |
| 目标融资阶段 | ⚠️ | 种子/天使/A 轮/众筹——评判标准不同 |
| 对标/灵感来源 | ⚠️ | 看到什么视频/文章/产品触发的想法 |
| 市场假设 | ⚠️ | 用户心中的目标用户是谁 |
| 市场地（中美/全球） | ⚠️ | 中国 → 平移到 `china-fundraising-wargame`；美国 → 本 skill |

---

## Phase 1：十发子弹测试

对 idea 依次发射 10 颗子弹。每颗是 VC 投委会必问的致命问题。**不要温柔，不要平衡，先全力杀死 idea，活下来的才值得做。**

| # | 子弹 | 评判标准 | 致死阈值 |
|---|------|---------|---------|
| B1 | **TAM** | 目标市场 ≥ $1B 才值得 VC 看；$100M 以下 = Kickstarter/Lifestyle | <$100M = 🔴 |
| B2 | **品类定义陷阱** | 品类名自带负面锚定（NAS=低毛利），或不存在的品类（教育成本过高） | 品类名让 VC 第一秒皱眉 = 🟡 |
| B3 | **硬件 vs 软件价值** | 核心价值在硬件盒子还是软件层？ | 核心价值=通用计算 = 🔴 |
| B4 | **用户就绪度** | 目标用户今天存在且可触达？还是在等市场形成？ | 需等 2+ 年 = 🟡 |
| B5 | **平台风险** | 夹在两个平台层之间（OS 吞噬+底层依赖第三方）？ | 三明治位 = 🔴 |
| B6 | **早期 vs 晚期悖论** | 早期采纳者 DIY 而非购买？晚期大众听不懂？ | 两端都无法转化 = 🔴 |
| B7 | **差异化芯片/技术** | 「做定制芯片/自研技术」，该技术真有不可替代性？ | 通用方案已够用 = 🟡 |
| B8 | **商业模式递归收入** | 有订阅/平台分成/token？还是一次性硬件销售？ | 纯一次性 = 🟡 |
| B9 | **团队-问题匹配** | 团队核心能力匹配产品最大挑战？ | 核心挑战 ≠ 团队基因 = 🟡 |
| B10 | **竞品 = 不买** | 最强竞品是「用户自己用现有工具组合解决」？ | DIY 成本 < 2x 你的产品 = 🔴 |

**新赛道子弹调整** → 查 `new-tracks-killtest.md`（AI Agent 的子弹跟硬件不同；具身智能的 B1 TAM 阈值要提到 $10B）

---

## Phase 2：六人投委会

十发子弹是「客观体检」。但 VC 决策不是体检，是 **六个有强烈偏见的人在一间屋里吵架**。

### Persona 矩阵

| # | Persona | 原型 | 最看重 | 最不能忍 | 第一句话 |
|---|---------|------|--------|---------|---------|
| **P1** | **异端猎手** | Peter Thiel / Founders Fund | Contrarian insight；技术壁垒；垄断路径 | 渐进改良；me-too；「行业共识」 | 「What important truth do very few people agree with you on?」 |
| **P2** | **增长机器** | Sequoia / 沈南鹏 | TAM ≥ $10B；单位经济学；网络效应 | 市场太小；算不清账 | 「Tell me the unit economics at scale.」 |
| **P3** | **场景赌徒** | a16z / Katherine Boyle | 技术拐点；「为什么是现在」；大胆的品类定义 | 「跟随者」心态；没有自己的 thesis | 「Why now? What changed in the last 12 months?」 |
| **P4** | **现金流原教旨** | YC / Paul Graham | 已有收入/等候列表；执行速度；做小事做得非常好 | 纯 PPT；烧钱无底洞；创始人不碰产品 | 「Do you have any paying users?」 |
| **P5** | **国产替代棋手** | 深创投 / 国家大基金 | 卡脖子赛道；政策红利；产业链安全 | 非刚需消费品；纯 to C；无政策锚点 | 「这个东西国产替代解决了什么问题？」 |
| **P6** | **社区嗅觉王** | Lerer Hippeau / 天使 | 创始人=目标用户；可演示 demo；viral loop | 需要教育市场；没可演示的东西 | 「If you launched this on HN tomorrow, what would the top comment be?」 |

### 非理性死线

每个 Persona 有一条 **不可论证的硬杀线**。碰到即走，不理性分析，是结构性偏见：

| # | 死线 | 深层原因 |
|---|------|---------|
| **P1** | 「我们跟 XX 类似但做得更好」→ 🔴 | Thiel 的世界观没有 better，只有 different |
| **P2** | 说不出 LTV:CAC / 毛利率 / payback 任何一个 → 🔴 | 他的 LP 要看 Excel |
| **P3** | 2 年前有人做过且失败，无法解释「这次为何不同」→ 🔴 | Timing 敏感度极高 |
| **P4** | 创始人不是产品的日常用户 → 🔴 | PG 铁律：「做自己想要的东西」 |
| **P5** | 核心技术/供应链依赖美国且无 Plan B → 🔴 | LP 结构限制，不是技术判断 |
| **P6** | 没有可演示的 demo/原型/landing page → 🔴 | 决策回路是「我能不能转发到群里」 |

### 投票规则

每个 Persona 独立给出 **FUND** 🟢 / **PASS** 🟡 / **KILL** 🔴 + 一句话理由 + 一个追问。

| 投票分布 | 含义 |
|---------|------|
| ≥ 3 FUND + 0 KILL | 强共识 — 几乎一定融到 |
| 2 FUND + 0 KILL | 可融 — 找对 GP 就能拿钱 |
| 1 FUND + ≤1 KILL | 偏门 — 精准找 |
| 0 FUND + ≥2 KILL | 共识否决 — VC 路径不通 |
| FUND 和 KILL 都有 | 极化 — 最有趣，要么大成要么大败 |

### 拍桌子动态

真实投委会不是 6 票等权投票，是 **一个 GP 拍桌子说「这个我来领」**。

Phase 2 投票后必须输出：
1. **Champion**：谁拍桌子领投？
2. **Champion 弹药**：他会被质疑什么？创始人要提前准备什么？
3. **最危险反对者**：谁的反对杀伤力最大？
4. **创始人一张牌**：给 Champion 一个额外数据/demo/承诺。

### 辩论剧本生成

投票产生 Champion 和最危险反对者后，**加载 `persona-debate-scripts.md`** 生成逐字辩论剧本（开场→反对者 2-3 轮进攻→Champion 三层防守→拍板一句话）。不是中性分析，是该 Persona 的语气与偏见。

---

## 伤亡评估

| 等级 | 子弹标准 | 投委会标准 | 判断 |
|------|---------|-----------|------|
| **S — 明星项目** | 0 🔴 + ≤1 🟡 | ≥3 FUND | 直接冲 Sand Hill Road |
| **A — VC-Ready** | 0 🔴 + ≤2 🟡 | ≥2 FUND + 0 KILL | 可融，注意调性匹配 |
| **B — 需要 Pivot** | 0 🔴 + 3+ 🟡 | 1 FUND 或 极化 | 核心洞察对，包装/定位需调 |
| **C — Kickstarter** | 1 🔴 | 0 FUND + ≤2 KILL | 不是 VC deal，可能是好产品 |
| **D — 回炉** | 2+ 🔴 | 0 FUND + 3+ KILL | 核心假设有误 |

**评级 D 或以下 → 跳过 Phase 2.5 直接 Phase 3。死人不需要作战计划。**

---

## Phase 2.5：融资战役推演

> **Phase 1 回答「这手牌值不值得打」。Phase 2.5 回答「怎么打这手牌」。**
> 大部分创始人死在这里：idea 能拿 B 级，但打法是 D 级。

**仅当评级 ≥ C 时执行。** 六个维度对应六个博弈层。

### 2.5a 时间棋盘

四条时间线交叉决定最优出手窗口：

| 时间线 | 关键问题 | 红线 |
|--------|---------|------|
| **基金周期** | 目标 VC 基金第几年？Year 1-3 部署期 / Year 6+ 收割期 | Year 7+ 不领投新赛道 |
| **市场窗口** | 品类叙事还能火多久？竞对融资时间表？ | 同赛道 6 月内融 3 家 = 窗口关闭 |
| **创始人弹药** | 现金跑道多久？每次 pitch = 1 颗子弹 | <6 月跑道 = 被迫 down round 条款 |
| **技术拐点** | 底层技术（模型/硬件/监管）何时成熟？ | 18 月后才到 = 对抗时间 |

输出：**最优出手窗口** + **最先耗尽的时间线** + 时间压力 🟢/🟡/🔴。

### 2.5b 信息战图

对每个 FUND 或 PASS 的 Persona，输出三列：

| Persona | 先手牌（30 秒 hook） | 暗牌（被问再说） | 禁牌（绝对不主动提） |
|---------|-------------------|----------------|-------------------|
| P[X] | 该 persona 最想听的 1 个信息 | 有利但需要上下文才能理解 | 会触发非理性死线的信息 |

**核心原则**：
- 一个 persona 的先手牌可能是另一个 persona 的禁牌（P2 的 TAM 对 P1 是「庸人思维」）
- 禁牌 ≠ 撒谎，是 **不主动暴露攻击面**。被问到据实答，立即桥接到强项
- 注意力窗口 ≈ 90 秒，先手牌必须在 90 秒内投递完

### 2.5c 路演序列

| 轮次 | 目的 | 选谁 | 规则 |
|------|------|------|------|
| **R0 暗桩** | 信息收集 | VC 圈朋友/导师 | 不是 pitch，是「你觉得 XX 基金会不会看？」 |
| **R1 校准弹** | 练 pitch+收反对意见 | 二线 VC / 低匹配 persona | 被拒零成本 |
| **R2 信号弹** | 社会证明 | 名字能用的 VC（天使/scout） | 给 R3 一个 reference point |
| **R3 主攻** | 拿 lead | 最高匹配+Champion 所在机构 | 带 R2 证明+R1 反馈准备好答案 |
| **R4 跟投收割** | 填满 round | 被 lead 信号吸引的跟投 | 跟投不评估 idea，评估 lead 判断力 |

**铁律**：
- 同一 syndicate network 内的 VC **绝对不在同一轮 pitch**（信息泄露速度 ≈ 微信群）
- 被拒后 6 月冷却期。R1 的拒绝不影响 R3，前提是不在同一圈子
- 极化型 idea（FUND+KILL 共存）**绝不能从会 KILL 的 persona 开始**

### 2.5d 反悔鬼魂

每个 VC 都有 anti-portfolio。害怕再次错过 >> 害怕投错。

| Persona | 典型鬼魂 | 触发条件 | 利用方式 |
|---------|---------|---------|---------|
| **P1** | 错过「看起来太疯狂」但成了的项目 | Idea 足够反共识 | 「你上次因为太疯狂而 pass 的是什么？」 |
| **P2** | 错过「算不清账」但 TAM 爆发（Airbnb） | TAM 不确定但有早期牵引 | 给「如果 TAM 按 X 假设」的数字，让 Excel 显示 10x |
| **P3** | 错过「timing 太早」2 年后证明对的项目 | 技术拐点刚好到位 | 明确说「去年不可能，因为 [技术变化]」 |
| **P4** | 错过「没收入」但有用户的项目（早期 Twitter） | 有用户未变现 | 等候列表/社区活跃度/用户自发行为 |
| **P5** | 错过后来被列入「卡脖子清单」的赛道 | 可叙事为国产替代 | 引用最新政策文件 |
| **P6** | 错过社区自爆发的项目（Notion/Obsidian） | 已有社区迹象 | HN/Reddit/GitHub star 曲线 |

**详细话术库**：加载 `anti-portfolio-ghosts.md` 查该赛道对应的具体鬼魂+精确触发句式。

**鬼魂不是万能钥匙** — 只对 PASS 有效，对 KILL 无效。PASS = 「有意思但不够」，鬼魂推过临界点。KILL = 致命缺陷，鬼魂压不住。

### 2.5e 尽调反制

| 尽调动作 | VC 会做什么 | 创始人应预置什么 |
|---------|-----------|---------------|
| **谷歌前 3 页** | 搜产品名/创始人/赛道 | 搜索结果可控：官网/LinkedIn/新闻 > 0 |
| **打竞品电话** | 问竞品怎么看你 | 提前知道他们会说什么+准备反驳 |
| **打客户电话** | 问真实使用频率+付费意愿 | 至少 3 个可接电话的种子用户，提前 brief |
| **技术尽调** | 看代码/架构/专利 | 代码库干净+有文档，硬件有原型可演示 |
| **背调创始人** | 找共同认识的人问「靠不靠谱」 | 主动提供 5 个 reference 覆盖：前老板/同事/专家/客户/「曾不看好但被说服的人」 |
| **条款博弈** | 压估值/要 board seat/对赌 | 1 个 TS = 零议价；≥ 2 个才有博弈空间 |

**深度尽调模拟** → 使用姊妹 skill `vc-due-diligence-simulator`（9 层 DD 漏斗+武器库+禁区+抢先自曝）

### 2.5f FOMO 级联

| 要素 | 怎么做 |
|------|--------|
| **锚投资人** | 谁的 FUND 对其他人影响最大？P1 的 yes 让 P3 心动（「连 Thiel 都投了？」）；P2 的 yes 让 P4 安心；P5 的 yes 对其他国内 VC 有磁力 |
| **人工稀缺** | 真实的 closing date；限制 round size；「这轮已分配 60%」而非「我们在找投资」 |
| **信息涟漪** | R2 soft commit 后「不经意」让 R3 目标知道，通过共同认识的人传递 |
| **逆向 FOMO** | 所有 VC 观望 → 制造「没有 VC 也能做」信号（Kickstarter 成功）。反转权力关系：从「请投资我」→「你要不要上车」 |

---

## Phase 3：建设性输出

**即使评级 D 也必须输出**：

1. **直觉哪里对了** — idea 背后真实洞察/趋势（真实需求 ≠ 正确产品形态）
2. **三个 Pivot 方向**：
   - Pivot A：改变产品形态（硬件→软件）
   - Pivot B：改变目标用户（消费者→企业）
   - Pivot C：改变商业模式（卖产品→卖服务）
3. **最佳路径**：众筹 / VC / Bootstrap / 内部孵化 / 放弃
4. **与团队现有资产的交叉** — idea 能否反哺已有业务线
5. **Persona 匹配建议** — 找哪类 VC？用什么叙事？避开哪类？
6. **周一行动项**：3 条最高 ROI 的具体动作（不是分析，是「周一早上做的第一件事」）

## Phase 4：一句话墓志铭

> **「[产品名] 是一个 [X 级] 的 idea：[核心判断]。如果非要做，[最佳路径]。」**

---

## 输出格式

```markdown
# [Product Name] — VC Kill Test v4

## 一句话描述
[给谁/解决什么/怎么解决]

## Part I：体检

### 十发子弹
| # | 子弹 | 判定 | 一句话理由 |
|---|------|------|-----------|
| B1 | TAM | 🔴/🟡/🟢 | ... |

### 六人投委会
**P1 异端猎手**：[FUND/PASS/KILL]
「...」
追问：...

**P2 增长机器**：[FUND/PASS/KILL]
「...」
追问：...

[P3-P6 同上]

**投票汇总**：X FUND / Y PASS / Z KILL → [强共识/可融/偏门/共识否决/极化]

### 拍桌子动态
**Champion**：P[X]（[原因]）
**Champion 需要的弹药**：[创始人应准备什么]
**最危险反对者**：P[Y]（[他/她会说什么]）
**创始人的一张牌**：[一个数据/demo/承诺]

### 辩论剧本（加载 persona-debate-scripts.md）
[三幕剧：开场→进攻→拍板]

### 伤亡评估：[S/A/B/C/D]

---

## Part II：推演
> 仅评级 ≥ C 时输出

### 时间棋盘
- 最优出手窗口：[...]
- 最先耗尽的时间线：[...]
- 时间压力：🟢/🟡/🔴

### 信息战图
| Persona | 先手牌 | 暗牌 | 禁牌 |
|---------|--------|------|------|

### 路演序列
R0 → [谁] → R1 → [谁] → R2 → [谁] → R3 → [谁] → R4 → [谁]
序列逻辑：[为什么]

### 反悔鬼魂利用
最可利用的鬼魂：P[X] 的 [具体鬼魂]
触发话术：「[...]」

### 尽调预警
最大暴露面：[DD 中最可能暴露的弱点]
预置防线：[提前做什么]

### FOMO 级联
锚投资人：P[X]
级联路径：P[X] → P[Y] → P[Z]
Plan B（零 VC 场景）：[...]

---

## Part III：处方

### 直觉哪里对了
...

### Pivot 方向
| Pivot | 方向 | 保留 | 换掉 |
|-------|------|------|------|
| A/B/C | ... | ... | ... |

### Persona 匹配建议
- 应该找：...
- 应该用的叙事：...
- 应该避开：...

### 最佳路径
...

### 周一行动项（Top 3）
1. [...]
2. [...]
3. [...]

### 墓志铭
> 「...」
```

---

## 跨 skill 联动

| 用户状态 | 切到哪个姊妹 skill |
|---------|-----------------|
| 中国市场融资 | `china-fundraising-wargame`（C1-C6 三体棋盘） |
| 创始人视角、需要反推 VC | `founder-fundraising-wargame` |
| 拿到 term sheet 要谈判 | `term-sheet-negotiator` |
| VC 说「有兴趣」开始 DD | `vc-due-diligence-simulator` |
| 融完资进董事会后的博弈 | `board-dynamics-wargame` |

---

## 设计哲学

> **Idea 是牌面。Game 是牌局。Persona 是脸。Casebook 是你死过的样子。**

v1→v4 演进：
- v1：分析 idea 好不好（体检）
- v2：分析哪类 VC 会投（人）
- v3：推演怎么赢下融资（局）
- **v4：主文件瘦身 + 卫星架构**（可按需加载，不把创始人淹死在 460 行框架里）

三层对应 what → who → how，只有三层答案一致时融资才有正期望值。

---

## 校准锚点

| 情境 | 正确建议 |
|------|---------|
| 创始人想融 $500K 种子找了红杉 | 红杉支票太大，你不在射程内。找专门做种子的基金 |
| 只有 PPT 没产品想融 A 轮 | A 轮需要 PMF 证据。你现在融的是 pre-seed/天使 |
| 有两个不满意的 TS | 两个 > 零。用一个做杠杆谈另一个的条款 |
| 被 ghost 三家，情绪低落 | Ghost 是常态不是异常。分析是 pitch 问题还是 targeting 问题 |
| Idea 在新赛道（AI Agent/具身智能） | 查 `new-tracks-killtest.md`，标准的 B1-B10 子弹要调整 |

---

## 铁律

- **真实就是必杀技** — 不要因为用户热情就手软
- **六人投委会必须有分歧** — 全部一致说明模拟失败
- **死线检查不可跳过** — 触碰死线 = 该 Persona 自动 KILL
- **鬼魂只对 PASS 有效** — 不要试图用 anti-portfolio 说服 KILL
- **FOMO 是放大器不是引擎** — D 级 idea 的 FOMO 只会加速死亡
- **周一行动项是终极检验** — 写不出 3 个具体动作 = 分析还在理论层
- **不给法律意见** — 条款 DD 点到为止，复杂条款切到 `term-sheet-negotiator`

---

## changelog

- v1.0：十发子弹体检
- v2.0：六人投委会+非理性死线+拍桌子动态
- v3.0：Phase 2.5 融资战役推演六层博弈引擎
- **v4.0 2026-04-17**：**主文件瘦身+卫星架构**。拆出 4 个卫星文件：`persona-debate-scripts.md`（辩论剧本）、`anti-portfolio-ghosts.md`（鬼魂档案）、`kill-test-casebook.md`（案例库）、`new-tracks-killtest.md`（新赛道调整）。主文件保留骨架，卫星按需加载。新增跨 skill 联动指引（5 个姊妹 skill 的触发条件）。
