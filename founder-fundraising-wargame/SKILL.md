---
name: founder-fundraising-wargame
version: v2.0
description: >-
  US fundraising war-game from the founder's chair — mirror skill to vc-pitch-killtest.
  Phase 0: fund anatomy (how VCs make money). Phase 1: recon (know VC before pitch).
  Phase 2: 6-persona boardroom simulation (P1-P6 US archetypes).
  Phase 2.5: 6-layer battle engine — temporal board, information warfare, pitch sequencing,
  anti-portfolio ghosts, DD counter-intel, FOMO cascade.
  Phase 3: tactical execution + term sheet signals. Phase 4: post-close transitions.
  Use when user is planning fundraising, preparing to pitch VCs, confused about VC behavior,
  negotiating term sheets, asking "how do I raise money", "what do VCs want", "why did this VC pass".
  Sister skills: vc-pitch-killtest (VC chair), china-fundraising-wargame (中国三体棋盘),
  term-sheet-negotiator (post-TS), vc-due-diligence-simulator (DD phase), board-dynamics-wargame (post-close).
---

# Founder Fundraising War Game v2.0 — 美国棋盘博弈引擎

## Changelog

| 版本 | 日期 | 范式 | 核心变动 | 位置 |
|------|------|------|---------|------|
| **v2.0** | 2026-04-17 | **博弈引擎** | 从知识库升级到推演：Phase 0 基金解剖+Phase 1 侦察+Phase 2 六人投委会+Phase 2.5 六层博弈引擎+Phase 3/4 战术执行与退出 | `SKILL.md`（live） |
| v1.0 | — | 知识库（内嵌） | VC 怎么赚钱、LP 结构、投组逻辑、美式条款基础 | 未归档 |

> **演进心法**：v1 知道规则，v2 推演怎么赢。姊妹：`china-fundraising-wargame`（中国三体棋盘）、`vc-pitch-killtest`（VC 椅子）。日常迭代 Git 追踪；下次范式切换（若有）才 snapshot 到 `archive/`。
>
> **核心区别**：中国融资 = 三体博弈（创始人 vs VC vs 政府）。
> **美国融资 = 二人博弈**（创始人 vs VC），但 VC 内部的投委会辩论是隐藏的第三体——创始人看不见它，但它决定你的命运。

## 触发条件

- 用户即将或正在融资，需要策略指导
- 用户对 VC 决策逻辑困惑（「为什么他们 pass 了？」）
- 用户收到 term sheet 需要解读
- 用户问「怎么找投资人」「该不该融资」「怎么谈估值」
- 用户刚被拒绝，需要理解发生了什么

## 卫星文件索引

| 卫星 | 何时加载 | 用途 |
|------|---------|------|
| `vc-persona-debate-us.md` | Phase 2 投票后 | P1-P6 美版投委会辩论逐字剧本 |
| `term-sheet-anatomy.md` | Phase 3d 拿到 TS | 美式 TS 逐条拆解（liquidation pref/protective provisions/ROFR/drag-along/vesting） |
| `us-casebook.md` | 任何时候 | 美国公司融资死法档案（Zenefits/WeWork/Theranos/Clubhouse/Rabbit） |
| `bridge-round-playbook.md` | 需要 Bridge/SAFE/extension | 美版特产的 bridge round 博弈 |

---

## 核心前提

**大部分创始人融资失败，不是因为 idea 差，是因为他们在玩一个不懂规则的游戏。**

他们不知道：
- VC 的钱不是 VC 的钱（是 LP 的钱，LP 有自己的规则）
- VC 说「有兴趣」不是有兴趣（是在收集信息决定要不要 pass）
- 估值不是你说了算也不是 VC 说了算（是基金数学倒推出来的）
- 被拒绝 ≠ idea 差（可能只是不匹配 GP 的 thesis / 基金阶段 / 投组需求）
- **投委会里有一个 Champion 在为你拍桌子**——你的 pitch 应该是给 Champion 的弹药库，不是给所有人的均衡陈述

本工具教创始人 **读懂对手的牌 + 推演怎么赢**。

---

## Phase 0：基金解剖学

> 不懂这一层的创始人 = 棋盘上不知道规则的棋子。

### 0a. 基金数学

| 概念 | 公式 / 规则 | 对创始人意味着什么 |
|------|-----------|-----------------|
| **基金规模** | 一支基金 = $X0M | $200M 基金不会投 $500K 种子——管理成本 > 收益 |
| **2/20 模型** | 管理费 2%/年 + Carry 20% | GP 靠管理费活着，靠 carry 发财。**管理费 = 无论好坏都拿 → 大基金有惰性。Carry = 只有赚了才拿 → 小基金更饥饿** |
| **支票大小** | 基金规模 × 3-5% = 单笔上限 | $100M 基金甜蜜点 = $3-5M。你要 $500K 嫌太小；$20M 吃不下 |
| **所有权目标** | 10-20%（种子），15-25%（A 轮） | 估值 = 支票 ÷ 目标所有权。VC 投 $5M 要 20% → 你的 pre-money = $20M。**不是你值多少，是他的数学需要你值多少** |
| **回报倍数** | LP 期望 ≥ 3x net（顶级 5x+） | 30 笔投资的基金，需要 1-2 笔 ≥ 50x 才达标 |
| **幂律分布** | 80-90% 回报来自 10-20% 项目 | VC 宁可 10 个高风险 bet 让 1 个爆，也不投 10 个稳健。**「稳健」是 VC 不想听的语言** |
| **基金生命周期** | 10 年（3-4 年部署 + 6-7 年退出） | Year 1-3 积极找 deal（你的窗口）。Year 7+ 管理退出（不看新项目）。**问 VC 他们基金是哪一年的** |

### 0b. LP 类型与约束

VC 的 LP 结构决定了 VC 的风险偏好——这不是 GP 个人选择，是 **合同义务**。

| LP 类型 | 典型代表 | 风险偏好 | 对 VC 行为的影响 |
|---------|---------|---------|----------------|
| **大学捐赠** | Yale / Stanford Endowment | 超长期，可承受高波动 | 支持 VC 投高风险早期。**最好的 LP——给 VC 最大自由度** |
| **养老金** | CalPERS | 中期，需要稳定现金流 | VC 被迫平衡增长与退出。倾向投有收入公司 |
| **家族办公室** | 各种 | 高度个人化 | 可能有特定偏好/排除。创始人可能碰到「LP 不让投你这个方向」 |
| **主权基金** | Mubadala / GIC / 中投 | 规模巨大，回报稳定 | 通常只投到 growth+。地缘政治敏感 |
| **母基金（FoF）** | 各种 | 分散化，看 GP track record | 标准化 LP，约束少。但看历史 DPI |
| **CVC** | Google Ventures / 腾讯投资 | 战略协同 > 财务 | **隐藏议程**：获取技术/阻止竞对/锁定供应链。问：如果被竞对收购，CVC 会不会行使否决权？ |

### 0c. 投组构建逻辑

VC 不是在真空评估你，是在 **已有 20 个棋子的棋盘上** 决定要不要放第 21 个。

| 约束 | 含义 | 创始人怎么利用 |
|------|------|-------------|
| **赛道集中度** | 大部分基金不投同赛道两家直接竞品 | 目标 VC 已投你竞品 → **game over**。反过来：投了你的上下游 = 你是拼图缺口 |
| **阶段分布** | 基金有阶段偏好 | 你 pre-revenue 找 growth fund = 白费 |
| **地理配置** | 有些基金有地理分散要求 | 某基金中国 portfolio 太少 → 你的 deal 对他们有配置价值 |
| **follow-on 预留** | 通常 40-60% 资金预留做 follow-on | 已部署 70%+ = 新 deal 竞争剩余 30%，标准更高 |
| **DPI 压力** | LP 看 DPI（现金回报比例） | Year 5+ 但 DPI 低 → GP 有退出压力，不投需要 7 年退出的项目 |

---

## Phase 1：侦察

> 走进会议室之前，你应该比 VC 更了解 VC。

### 1a. VC 情报清单

对每个目标 VC，约会议前收集：

| 情报 | 在哪里找 | 为什么重要 |
|------|---------|-----------|
| 基金年份 / DPI | Pitchbook / Crunchbase / 直接问 | Year 1-3 积极部署 vs Year 6+ 不看新 |
| 最新基金规模 | 新闻 / SEC / 中基协 | 决定支票大小甜蜜点 |
| GP 个人 thesis | GP 的 X / 播客 / 博客 / 演讲 | **用 GP 自己的语言回 pitch 他**——最高效的 hook |
| 已投 portfolio | VC 官网 | 有你竞品 or 上下游？可介绍哪家 portfolio 公司？ |
| 最近 3 个 deal | 新闻 | 当前偏好方向 |
| anti-portfolio | 博客 / 访谈 / Bessemer 公开 | 后悔 pass 了什么？触发「鬼魂」话术 |
| LP 构成 | 备案信息 | 决定风险偏好底层约束 |
| 合伙人分工 | LinkedIn / 引荐人 | 找错 GP = 被转介到「不太管这个方向」的人 |

### 1b. 引荐博弈

冷邮件转化率 ≈ 1-3%。热引荐 ≈ 20-40%。**引荐本身是信号博弈**。

| 引荐人类型 | 信号强度 | 注意事项 |
|-----------|---------|---------|
| 该 VC 已投公司的创始人 | ⭐⭐⭐⭐⭐ | 最强。「我投的人推荐的人，眼光同一水平线」 |
| 该 VC 的前同事 / 朋友 | ⭐⭐⭐⭐ | 社交关系 = 面子成本 → 一定被认真看 |
| 其他 VC | ⭐⭐⭐ | 双刃剑：引荐 VC 层级更高 → 正信号；同级 → 「为什么他自己不 follow-on？」 |
| 行业 KOL | ⭐⭐ | 说明被行业认可，但 VC 做独立判断 |
| 冷请求 | ⭐ | 等于冷邮件加一层包装 |

**铁律**：引荐人必须能回答「你为什么推荐他？」——只转发不了解 = 信号为零甚至为负。

---

## Phase 2：美国六人投委会

> v1.0 没有 Phase 2。v2.0 补齐——投委会不是你看不见的黑盒，是你可以推演的舞台。
> 与 `vc-pitch-killtest` v4.0 共享 P1-P6 定义，但 **从创始人视角使用**——你要知道：
> - 你会在哪个 Persona 面前得 FUND / PASS / KILL
> - 谁会做你的 Champion
> - Champion 会被哪个反对者攻击
> - 你要给 Champion 什么弹药

### 六 Persona 与创始人应对

| # | Persona | 原型 | 你怎么 pitch 他 | 他最容易 KILL 你因为 |
|---|---------|------|--------------|------------------|
| **P1** | **异端猎手** | Peter Thiel / Founders Fund | 开场一个 contrarian insight，其他都不说 | 你的产品是 me-too 的包装 |
| **P2** | **增长机器** | Sequoia / Accel | 三个数字（LTV:CAC / 毛利率 / payback），然后让他自己问 TAM | 你说不出 unit economics 任何一个 |
| **P3** | **场景赌徒** | a16z / Benchmark | 「why now」一句话，然后 technology inflection 证据 | 你的 why now 是去年说过的话 |
| **P4** | **现金流原教旨** | YC / 天使 | 直接说有谁在付钱，其他都不用讲 | 你自己不是产品用户 |
| **P5** | **战略资本** | American Dynamism / 国防/能源 | 战略价值 + 政策对齐 | 你依赖外国技术且无 Plan B |
| **P6** | **社区嗅觉王** | Lerer Hippeau / 消费天使 | 你发 demo 链接而不是 pitch deck | 你没有可演示的东西 |

### 非理性死线（创始人视角——**碰到就绕开**）

| # | 死线 | 如果你碰了 → 怎么补救 |
|---|------|-------------------|
| **P1** | 「我们跟 XX 类似但做得更好」→ 🔴 | 不要 pitch P1。找 P2/P4 类型 |
| **P2** | 说不出 LTV:CAC / 毛利率 / payback → 🔴 | 在见 P2 之前，让财务顾问建模。宁可数字粗糙也要有 |
| **P3** | 2 年前有人做过且失败，无法解释「这次为何不同」→ 🔴 | 准备一个 specific 技术/行为 shift 的证据，不要抽象谈 |
| **P4** | 创始人不是产品的日常用户 → 🔴 | 找个 co-founder 是用户。或者绕开 P4，找 P1/P3 |
| **P5** | 核心技术/供应链依赖美国且无 Plan B → 🔴 | 在中美 tension 语境下，对 P5 不适用；改找 American Dynamism（美国战略自主） |
| **P6** | 没有可演示的 demo/原型/landing page → 🔴 | 先做 demo 再 pitch。P6 的会议就是 demo review |

### 投票规则

| 投票分布 | 含义 |
|---------|------|
| ≥ 3 FUND + 0 KILL | 强共识 — 少见，几乎一定融到 |
| 2 FUND + 0 KILL | 可融 — 找对 GP 就能拿钱 |
| 1 FUND + ≤1 KILL | 偏门 — 精准找 |
| 0 FUND + ≥2 KILL | 共识否决 — VC 路径不通 |
| 分裂 | 极化 — 最有趣 idea，要么大成要么大败 |

### 拍桌子动态（创始人版）

投票后创始人必须回答：
1. **我的 Champion 是谁？** 他最可能因为什么 FUND 我？
2. **Champion 会被谁攻击？** 攻击角度是什么？
3. **我要给 Champion 什么弹药？** 一个数据/demo/承诺，让他能压住反对者
4. **我会不会意外引爆反对者的非理性死线？** 如果会，重写 pitch 的顺序

### 加载辩论剧本

为 Champion 和最危险反对者生成逐字辩论剧本 → **加载 `vc-persona-debate-us.md`**

---

## Phase 2.5：美版融资战役推演

> **Phase 0-2 回答「这手牌值不值得打」。Phase 2.5 回答「在美国牌桌上怎么赢」。**
> 六层博弈引擎，与 `china-fundraising-wargame` v2.0 对称（但规则完全不同）。
>
> **仅当投委会有 ≥1 FUND 时执行。** 0 FUND = 牌面不够，先改牌。

### 2.5a 时间棋盘（美版）

四条时间线交叉决定最优出手窗口：

| 时间线 | 关键问题 | 红线 |
|--------|---------|------|
| **基金周期** | 目标 VC 基金第几年？Year 1-3（部署期激进）/ Year 6+（收割期保守） | Year 7+ 不领投新赛道，只跟投 |
| **市场窗口** | 品类叙事还能火多久？竞对融资时间表？ | 同赛道 6 月内融 3 家 = 窗口关闭 |
| **创始人弹药** | 现金跑道多久？每次 pitch = 1 颗子弹 | < 6 月跑道 = 被迫 down round 条款 |
| **技术拐点** | 底层技术（模型/硬件/监管）何时成熟？ | 18 月后才到 = 对抗时间 |

**美版特殊时间线**：**退出周期**。美国 VC 的 LP 对 DPI 的耐心比中国长，但 IPO 窗口和 M&A 窗口也有周期性。2023-2025 IPO 窗口关闭 → VC 对需要快速 exit 的项目更谨慎；2026 Q1 开始边际打开。

输出：**最优出手窗口** + **最先耗尽的时间线** + 时间压力 🟢/🟡/🔴。

### 2.5b 信息战图

美国的信息战特殊之处：**每个 Persona 的注意力窗口更短**（< 60 秒的 hook），但 **思维开放度更高**。

对每个 FUND 或 PASS 的 Persona，输出三列：

| Persona | 先手牌（30-60 秒 hook） | 暗牌（被问再说） | 禁牌（绝对不主动提） |
|---------|-------------------|----------------|-------------------|
| P1 | 一句 contrarian insight | 竞品分析（P1 不关心） | me-too 叙事 / 「市场饱和」语言 |
| P2 | 三个 unit economics 数字 | 技术细节 | 「这是下一个 Google」类叙事 |
| P3 | Why now 的具体 technology shift | TAM 数字（太大反而不可信） | 「这已经工作 18 个月了」（不够早） |
| P4 | 「X 人在付钱 $Y/月」 | 愿景（P4 对愿景免疫） | 「用户将会」类未来时态 |
| P5 | 战略价值 + 政策锚点 | 单位经济学（P5 不看 IRR） | 外国技术依赖 |
| P6 | Demo 链接 | 商业模式（P6 不关心） | 「我们还在构建 MVP」 |

**美版核心原则**：
- 一个 Persona 的先手牌可能是另一个的禁牌（P2 的 TAM 对 P1 是「庸人思维」）
- 禁牌 ≠ 撒谎，是 **不主动暴露攻击面**。被问到据实答，立即桥接强项
- **不同于中国**：美国不需要「两本 deck」——一本 deck 足够，但 pitch 的 **顺序** 要按 Persona 调整

### 2.5c 路演序列（美版）

美国的路演序列与中国有三个结构性差异：

| 维度 | 美国 | 中国 |
|------|------|------|
| **冷邮件转化率** | 1-3%（有一定概率） | < 1%（几乎为零） |
| **FA 作用** | B 轮后重要，A 轮前可选 | A 轮就需要，关系大于 PPT |
| **政府介入** | 几乎不存在 | 三体博弈核心 |

**五轮路演框架（美版）**：

| 轮次 | 目的 | 选谁 | 规则 |
|------|------|------|------|
| **R0 暗桩** | 信息收集 | VC 圈朋友/导师/scout | 「我不是在融资，就想聊聊方向」——获取情报+建立关系 |
| **R1 校准弹** | 练 pitch + 收反对意见 | 二线 VC / 低匹配 persona | 被拒零成本。目的是听反对意见并加固 pitch |
| **R2 信号弹** | 社会证明 | 名字能用的天使 / scout | 拿 soft commit 不需大额。给 R3 一个 reference point |
| **R3 主攻** | 拿 lead | 最高匹配 + Champion 所在机构 | 携带 R2 证明 + R1 反馈准备答案。**最好的子弹，不能浪费** |
| **R4 跟投收割** | 填满 round | 被 lead 信号吸引的跟投 | 跟投方决策模型 = 信任 lead，不独立判断 |

**美版铁律**：
- 同一 syndicate network 内的 VC **绝对不在同一轮 pitch**（Sand Hill Road 上信息传播速度 ≈ Twitter DM）
- 被拒后 6 月冷却期。R1 的拒绝不影响 R3，前提是不在同一圈子
- 极化型 idea（FUND+KILL 共存）**绝不能从会 KILL 的 persona 开始**
- **美版特殊**：Demo Day / Founder Summit 等场合是 R2 的绝佳触发器（社交证明效率极高）

### 2.5d 反悔鬼魂（美版）

每个美国 VC 都有 anti-portfolio。害怕再次错过 >> 害怕投错。

基本框架见 `vc-pitch-killtest/anti-portfolio-ghosts.md`（已覆盖 Bessemer 公开列表、Sequoia/a16z/FF/YC 的典型鬼魂、6 大 Persona 的鬼魂触发字典）。

**创始人视角的鬼魂使用**：
1. 只在 **R3 主攻或 Partner Meeting** 使用，不要在 R1/R2
2. 让 VC 自己说出鬼魂名字，而不是你主动说
3. 鬼魂不是万能钥匙——对 KILL 无效，只对 PASS 有效

### 2.5e 尽调反制（美版）

美国 VC 的 DD 比中国更系统化（专业 DD 公司、尽调流程标准化），但也更 **可预测**：

| DD 动作 | VC 会做什么 | 创始人应预置 |
|--------|-----------|------------|
| **Google 前 3 页** | 搜产品名/创始人/赛道 | 搜索结果可控：官网/LinkedIn/新闻 > 0 |
| **LinkedIn 侦察** | 团队背景 + 跳槽模式 | 让团队 LinkedIn 专业+一致 |
| **Glassdoor** | 公司文化 | 如果有 Glassdoor 页面，确保评分 ≥ 3.5 |
| **打竞品电话** | 问竞品怎么看你 | 提前知道他们会说什么+准备反驳 |
| **打客户电话** | 付费意愿 + 使用频率 | 至少 3 个可接电话的种子用户，提前 brief |
| **Reference check** | 找共同认识的人 | 主动提供 5 个 reference（前老板/同事/专家/客户/「曾不看好」的人） |
| **Background check** | 法律/信用/犯罪记录 | 提前自检（US：sex offender 名单、SEC 处罚、破产记录） |
| **技术 DD** | 代码/架构/IP | 代码库干净+有文档，IP 归属清晰 |

**深度尽调模拟** → 使用姊妹 skill `vc-due-diligence-simulator`

### 2.5f FOMO 级联（美版）

| 要素 | 美国打法 |
|------|---------|
| **锚投资人** | 美国 FOMO 级联的最强触发器是 **tier-1 VC 之间的 signaling**。a16z 领投 → Sequoia 会重新看。Founders Fund 领投 → a16z 会警觉 |
| **人工稀缺** | 真实 closing date；限制 round size；「这轮已分配 60%」 |
| **信息涟漪** | R2 soft commit 后「不经意」让 R3 目标知道，通过共同认识的人传递。X（Twitter）是美国信息涟漪的主要媒介 |
| **Tier 信号游戏** | 美国独有：不同 VC 的 signal 权重不同。拿到 tier-1 的 TS → 整个 sand hill road 会迅速看到；拿到 tier-3 lead → 对 tier-1 几乎没级联效应 |
| **逆向 FOMO** | 所有 VC 观望 → 制造「没有 VC 也能做」信号（Kickstarter 成功 / 收入增长 / 客户预付款）。反转权力关系：从「请投资我」→「你要不要上车」 |

---

### 2.5 汇总输出格式

```
## 美版融资战役推演

### 时间棋盘
- 最优出手窗口：[...]
- 最先耗尽的时间线：[...]
- 时间压力：🟢/🟡/🔴
- 退出窗口预警：[IPO/M&A 窗口对你的影响]

### 信息战图
| Persona | 先手牌 | 暗牌 | 禁牌 |
|---------|--------|------|------|
| P[X] | ... | ... | ... |

### 路演序列
R0 → [谁] → R1 → [谁] → R2 → [谁] → R3 → [谁] → R4 → [谁]
序列逻辑：[为什么这个顺序]

### 反悔鬼魂利用
最可利用的鬼魂：P[X] 的 [具体鬼魂]
触发话术：「[...]」（只在 R3+ 使用）

### 尽调预警
最大暴露面：[DD 中最可能暴露的弱点]
预置防线：[提前做什么]

### FOMO 级联
锚投资人：P[X] 类型 / tier-[N]
级联路径：P[X] → P[Y] → P[Z]
Plan B（零 VC 场景）：[...]
```

---

## Phase 3：战术执行

### 3a. BATNA 评估

你的 BATNA = 如果这轮融不到，你会怎样？BATNA 决定谈判底线。

| BATNA 等级 | 状态 | 对融资的影响 |
|-----------|------|------------|
| **S — 不需要你** | 已盈利 / 多个 TS / Kickstarter 成功 | 完全谈判权。挑 VC、谈条款 |
| **A — 能活** | 跑道 ≥ 12 月 + 收入增长 | 有时间挑选。不需接受第一个 offer |
| **B — 紧迫** | 跑道 6-12 月，无收入 | 3-4 月内需 close |
| **C — 绝望** | 跑道 < 6 月，无收入无备选 | VC 闻到绝望。**谈判权 = 0**。先延跑道再融资 |

**非对称信息利用**：你知道 BATNA，VC 不知道。但 VC 会从你行为推断：
- 催促 timeline → 暗示 C 级
- 比较 TS → 暗示 A/S 级
- 对估值无所谓 → S 级 或 C 级绝望（VC 会分辨）

### 3b. 信号审计

每个行为都在发送信号。**大部分创始人无意识地发送错误信号**。

| 行为 | 发出的信号 | 修正 |
|------|----------|------|
| 用 Gmail 而非自有域名 | 不认真 / 不投入 | 花 $12/年买域名。成本 ≈ 0 |
| Pitch deck > 15 页 | 不能提炼 | 10-12 页，每页一论点 |
| 第一次见面谈估值 | 不懂规矩 | 估值最后谈。先建 conviction |
| 对竞品攻击性强 | 不自信 / 无 moat | 承认竞品 + 解释 wedge |
| 说「我们没有竞品」 | 没做功课 / 市场不存在 | **永远有竞品**——「用户不改变行为」是终极竞品 |
| 追邮件 3 天没回 | 绝望 | 等 5-7 工作日。追邮件附新信息（新客户/新数据） |
| 同时告诉两个 VC「你是我的 first choice」 | 被发现 → 永久失信 | VC 圈极小，信息传播极快。**永远不要撒谎** |

### 3c. 会面博弈

1 小时 VC 会面信息密度分布极不均匀：

| 时间段 | 发生什么 | 创始人做什么 |
|--------|---------|----------|
| **0-2 min** | VC 形成第一印象（70% 权重） | **hook**：一句话讲清你是谁/做什么/跟他有关。不要从市场规模开始——从 insight 开始 |
| **2-10 min** | VC 做快速分类（属于哪个赛道 / 像哪个成功项目） | 帮 VC 完成分类。主动说「我们像 [已投公司 X] 但在 [Y 领域]」——锚定效应 |
| **10-30 min** | VC 开始提问（DD 第一步） | 每个问题 = 情报。记录。VC 问什么 = 担心什么 = 下次主动回答 |
| **30-50 min** | 还在聊 = 有兴趣。话题转向团队/执行/timeline | **反向 DD 窗口**：问基金阶段、decision process、timeline、谁做最终决定 |
| **50-60 min** | 收尾。「我们内部讨论」或「介绍合伙人」 | 「介绍合伙人」= 强正信号。「内部讨论」= 中性（可能礼貌 pass）。**当场约下一步具体时间**——模糊的「下周联系」= 大概率不联系 |

### 3d. 读懂 VC 的「不」

VC 几乎不直说「不」。拒绝需要翻译：

| VC 说的话 | 真实含义 | 怎么办 |
|---------|---------|------|
| 「市场太早了」 | 我看不懂 / 不在我的 thesis / 不敢赌 timing | 这不关于你，关于这个 VC。找 thesis-driven fund（P3 类型） |
| 「估值太高了」 | 可能真高，或 = 不够想投但便宜可以赌一把 | 多家都说高 → 真高。一家说 → 他不是你目标 |
| 「我们想看更多数据」 | 70% 拖延（等看下月增长）。30% 真做模型 | 问：「具体什么数据？达到 X 你 commit 吗？」 |
| 「我们已有类似 portfolio」 | 真冲突。**Game over** | 不要试图说服。问：「你觉得谁会对这方向更感兴趣？」 |
| 「现在 LP 环境不好」 | 可能真（冬天）。也可能借口 | 整体冬天 → 调整期望。只有这家 → 借口 |
| 「你应该再长一长」 | 最诚实的拒绝之一。看到潜力但下注太早 | **感谢+记录+3 月后带新数据回**。最易转化为 FUND 的 PASS |
| 「很感兴趣，下周跟进」→ 消失 | Ghost = Pass | 发 1 封 follow-up。2 周无回 → move on。不追超 2 次 |

### 3e. Term Sheet 博弈（总览）

拿到 term sheet 后另一个游戏开始。**深度拆解 → 加载 `term-sheet-anatomy.md`**。本处只覆盖总览信号：

| 条款 | 看起来像什么 | 陷阱在哪 | 怎么谈 |
|------|-----------|--------|--------|
| **估值（Pre-money）** | 「你值 $20M」 | 估值高 ≠ 好。高估值 = 下轮必须更高（否则 down round） | 合理就好。宁估值低 10% 条款干净，不要高 20% 但附带陷阱 |
| **清算优先权** | 「1x non-participating preferred」 | 1x 是标准。**> 1x = 红旗**。Participating = VC 先拿回本金再按比例分剩余 | 1x non-participating 是底线 |
| **董事会席位** | 「我们要一个 board seat」 | 种子轮不该给 board seat。让出一次 → 后续轮次叠加 → 失去控制 | 种子：2 founder + 1 independent。A 轮：2 founder + 1 VC + 1-2 independent |
| **反稀释** | 「Broad-based weighted average」 | 标准。**Full ratchet = 红旗** | Broad-based 是底线 |
| **Drag-along** | 「[X]% 股东同意出售，所有人跟」 | 阈值太低（50%）→ VC 可强制卖公司 | 阈值 ≥ 75%，创始人持股期内一票否决 |
| **Protective provisions** | 「我们要每月财报 + 可列席 board」 | 如果范围过宽 → 日常运营需 VC 批准 | 限制在融资/出售/关闭公司等重大事项 |

**最重要的博弈规则**：只有 1 个 TS = 零议价权。≥ 2 个 = 有博弈空间。**路演序列的终极目的就是在同一周内拿到 2+ TS**。

**深度条款谈判** → 使用姊妹 skill `term-sheet-negotiator`

---

## Phase 4：融后过渡

> v2.0 新增。大部分创始人融资结束就以为游戏结束——其实新游戏才开始：董事会、员工、下一轮、退出。

### 4a. Post-Close 的 90 天

| 时间段 | 必做 | 避免 |
|--------|------|------|
| **Week 1-2** | 通知所有人（员工/客户/投资人）；更新法律文件 | 太早公关（等 1 个月的 steady state） |
| **Week 3-6** | Board 第一次会议；set expectations；部署资金计划 | 过度承诺 milestone 时间表 |
| **Month 2-3** | 开始执行 + 第一次 board update | 推迟 bad news |

### 4b. 下一轮的准备从今天开始

融资 close 的第一天就要开始准备下一轮：

| 准备项 | 怎么做 |
|--------|------|
| **Board update rhythm** | 月度 update，不要等 quarterly。板子在 loop 里 = 下轮容易融 |
| **KPI 追踪** | 定义 3-5 个 North Star metric，每月给 board 看 |
| **创始人 mental model** | 下一轮融资 = 12-18 月后。今天的每个决策都在影响下轮 narrative |
| **Relationship banking** | 没拿你钱的 tier-1 VC → 月度非正式 update，让他们看到 traction |

### 4c. 董事会博弈（总览）

**深度董事会动态** → 加载姊妹 skill `board-dynamics-wargame`

融后最容易被忽视的博弈：
- CEO vs Board 的信息不对称设计
- 独董的选择与控制
- 罢免触发条件
- Investor rights 如何转化为 Board rights

---

## Phase 5：特殊情境剧本

### 5a. 被 Ghost 后怎么办

```
Day 0: 会面结束，VC 说「下周联系」
Day 7: 发 follow-up，附一个小更新（新客户/新功能）
Day 14: 没回 → 发最后一封：「我知道你很忙。如果时机不对完全理解，
        但如果是我可以改进的地方，我非常 welcome honest feedback。」
Day 21+: 没回 → Move on。3-6 月后带显著不同 traction 重新联系
```

核心：给 VC **一个体面的出口**。降低他说不的成本 → 反而可能获得有价值反馈。

### 5b. Bridge Round / 困境融资

美版特产的 bridge round 有专门博弈。**加载 `bridge-round-playbook.md`**。总览：

| 正常市场 | 冬天规则 |
|---------|---------|
| 选最好的 VC | 选 **愿意给钱** 的 VC |
| 优化估值 | 优化 **生存概率** |
| 多个 TS 再选 | 第一个 TS 就认真考虑 |
| 不接受 participating | 如果是唯一的钱 → 接受，争取 sunset clause |

### 5c. 中美转场

如果你的退出路径变了（A 股 → 美股 或 美股 → 港股），加载 `china-fundraising-wargame` 交叉评估。

### 5d. M&A 接洽

有时候融资的真实结局是并购。信号：
- CVC 在 DD 期间问「你们会考虑被收购吗？」—— 不是随便问
- 主业公司派 Corp Dev 人员约见，不是战投 → 收购信号
- 估值谈判卡在一个「奇怪的低价」——可能他们在做 acqui-hire 评估

---

## 执行指令

1. **判断用户所处阶段和币种轨道**：
   - 刚有想法，未开始融资 → 从 Phase 0 开始教育
   - 已在融资，遇到具体问题 → 跳到相关 Phase
   - 拿到 TS，需要解读 → Phase 3e + 切到 `term-sheet-negotiator`
   - 被拒，想理解 → Phase 3d + Phase 5a
   - 融后博弈 → Phase 4 + 切到 `board-dynamics-wargame`

2. **交叉引用**：
   - Idea 跑过 `vc-pitch-killtest` → 用其评级+P1-P6 投票作为本工具 Phase 2 输入
   - 中国市场 → 切到 `china-fundraising-wargame`

3. **输出风格**：
   - 不要教科书式罗列。**用创始人听得懂的语言**
   - 每条建议附「为什么」——不懂原理的战术会被错误应用
   - 行为在发错信号 → 直接指出，不要委婉
   - 给 **具体可执行的行动**，不是原则

4. **红线**：
   - 不给法律意见（TS 解读点到为止，复杂条款建议找律师）
   - 不鼓励欺骗（信息管理 ≠ 撒谎。禁牌 ≠ 否认）
   - 不假装融资总能成功——kill test 评级 D，诚实说「现在不该融资」

---

## 校准锚点

| 情境 | 正确建议 |
|------|---------|
| 创始人想融 $500K 种子找了红杉 | 红杉支票太大，不在射程。找专门做种子的基金 |
| 只有 PPT 没产品想融 A 轮 | A 轮需 PMF 证据。你现在融的是 pre-seed/天使 |
| 有两个不满意 TS | 两个 > 零。用一个做杠杆谈另一个的条款 |
| 被 ghost 三家，情绪低落 | Ghost 是常态。分析是 pitch 问题还是 targeting 问题 |
| BATNA C 级，无选择 | **不要融资，先延跑道**。Bridge / 个人借款 / 削减成本 |
| 融完 A 轮，下一轮遥远 | 今天就开始准备 B 轮。Board update 节奏 + Tier-1 VC relationship banking |

---

## 设计哲学（v2.0）

> **v1.0 = 知识库**（VC 怎么赚钱）
> **v2.0 = 博弈引擎**（怎么在美国牌桌上赢）

三层演进：**what**（规则是什么）→ **who**（谁在对面）→ **how**（怎么赢）。

与 `china-fundraising-wargame` v2.0 对称但规则不同：
- 中国 = 三体博弈（创始人 vs VC vs 政府）
- 美国 = 二人博弈但投委会内部辩论隐藏第三体
- 中国 = 返投+对赌+注册地
- 美国 = Term sheet 条款战
- 中国 = FA 是关系中间件
- 美国 = Warm intro 替代 FA

---

## changelog

- v1.0 2026-04-17：首版知识库
- **v2.0 2026-04-17**：**全面升级为博弈引擎**。新增 Phase 2（六人投委会）+ Phase 2.5（融资战役推演六层博弈）+ Phase 4（融后过渡）。拆出 4 个卫星文件（`vc-persona-debate-us.md` 辩论剧本 / `term-sheet-anatomy.md` TS 拆解 / `us-casebook.md` 案例库 / `bridge-round-playbook.md` bridge round 博弈）。与 `china-fundraising-wargame` v2.0 对称架构，与 `vc-pitch-killtest` v4.0 共享 P1-P6 定义。新增跨 skill 联动（5 个姊妹 skill）。
