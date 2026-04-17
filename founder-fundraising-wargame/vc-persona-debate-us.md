# VC Persona Debate — 创始人对 6 人投委会的应战台本

> v2.0 新增。与主文件 Phase 2 绑定使用。
> 姊妹文件：`vc-pitch-killtest/persona-debate-scripts.md`（VC 之间互相辩论的剧本，本文件是创始人对 persona 的应答剧本）

**为什么要两个版本**：
- **vc-pitch-killtest 的 persona-debate**：模拟投委会内部 P1-P6 拍桌子辩论，用于创始人「预演投委会会发生什么」
- **本文件**：模拟每个 persona 直接提问 + 创始人的应答，用于创始人「实战 meeting room 里怎么对话」

两者配对使用：先用前者知道「谁会挺我谁会反」，再用本文件知道「具体怎么对话」。

---

## Persona 快速回顾

| Persona | 代表 | 喜欢什么 | 讨厌什么 | 你的应对策略 |
|---------|------|---------|---------|-----------|
| **P1 异端猎手** | Peter Thiel / Founders Fund | contrarian + 垄断思维 | me-too / 线性改良 | 给「共识是错的」的 thesis |
| **P2 增长机器** | Sequoia / Benchmark | PMF + 数据 + 单位经济 | 讲故事 / 无 metrics | 给硬数字 + growth engine |
| **P3 平台玩家** | a16z / General Catalyst | 大赛道 + 平台故事 | 小市场 / 小格局 | 给 category-creating 愿景 |
| **P4 品味大师** | Benchmark / 老牌 seed | product beauty + 创始人直觉 | 过度工程 / 无品味 | 给 design 细节 + user love |
| **P5 企业收割机** | Greylock / Bessemer B2B | enterprise sales + TAM | B2C / 不规模化 | 给 enterprise pipeline + retention |
| **P6 工程原教旨** | USV / YC / 开发者向 | tech moat + 开发者体验 | 市场/销售导向 | 给 architecture + developer love |

**关键**：一个 meeting 中你可能面对多个 persona 的 GP。你要先识别每个人的 persona，再对每个 persona 定制 hook。

---

## P1 异端猎手 — 创始人应战台本

### 识别信号（meeting 前 5 分钟）
- 问「你们反对什么共识？」
- 谈 Girard / Thiel / philosophical first principles
- 对 benchmark 和竞争对手列表不感兴趣
- 问「如果对手 raise $100M 明天入场，你们怎么办？」（想听你说「他们做不到因为 X」）

### 开场 hook
```
"Here's what the market consensus is:[共识]。
Here's what's actually true:[反共识洞察]。
If we're right, the winner isn't who scales fastest—it's who built
on the right assumption from day one. Everyone else is fighting over [mainstream battleground]。
We're building in [unmonitored territory]. Here's why that matters..."
```

### P1 典型提问 + 应答台词库

**Q1: "What important truth do very few people agree with you on?"**（这是 Thiel 签名问题）

❌ 差答案：「我们的技术比竞争对手好」（这是 better not different）
❌ 差答案：「市场越来越大」（这是共识，不是反共识）

✅ 好答案：
```
"The consensus is that [X is the future]. That's wrong—or at least,
it's right for the wrong reasons. What's actually happening is [Y],
and [Y] makes most of the current [X] bets obsolete within 3 years.
Here's the evidence nobody's paying attention to: [specific data
or observation]. We're betting the sequence is Y → X', not
straight-line X."
```

**Q2: "Who are your competitors?"**

❌ 差答案：列 10 家公司 + SWOT 分析（说明你在 mainstream 市场）

✅ 好答案：
```
"At the surface level, we appear to compete with [3 companies].
But those companies solve [problem A]. We solve [problem B].
The only company that understands [problem B] the way we do
is [或者:没有人]. So strategically we're not in their market—
they're building the train and we're building the runway."
```

**Q3: "Why now? Why hasn't this been done yet?"**

❌ 差答案：「技术成熟了」（太泛）

✅ 好答案：
```
"Three things had to converge: [tech enabler X], [market shift Y],
[regulatory or cultural change Z]. They didn't converge until
[specific quarter/year]. Anyone who tried before [year] would have
failed because [Z was missing]. The secret is that Z happened
quietly and most people haven't noticed."
```

**Q4: "What if you're wrong?"**

❌ 差答案：「我们有 pivot option」（P1 听起来像没信念）

✅ 好答案：
```
"If we're wrong about [core insight], the whole thesis collapses—
I won't pretend otherwise. But here's the disconfirming evidence
we watch for: [3 specific signals]. If any of those appear, we
know we need to re-evaluate in 60 days. So far zero of those
signals have appeared—in fact, [opposite signals] have."
```

### P1 不喜欢的话
- 「We're the Uber of X」
- 「We have first-mover advantage」（P1 认为 second/third mover 经常赢）
- 「Our TAM is $100B」（TAM 对 P1 是 lagging indicator）
- 「We have great traction」（P1 要的是 insight，不是 traction）

### P1 最后决策时的关键瞬间
如果 P1 是你的 Champion，他会说：「Partners, this might 0-out or it might return the fund. The math demands we take it.」——他在押赌。
如果 P1 反对，他会说：「This is a 2-3x outcome that quietly kills the fund's headline returns.」——他觉得你是 me-too。

---

## P2 增长机器 — 创始人应战台本

### 识别信号
- 问「show me the retention cohorts」
- 问「what's your CAC and LTV」
- 对 design / philosophy 不感兴趣
- 看你的 dashboard 如果没有 = 离开

### 开场 hook
```
"Here's our unit economics in one slide: CAC $[X], LTV $[Y],
payback [Z] months. Here's the growth engine that drives it:
[channel with numbers]. Here's the retention: Month 1 [%],
Month 6 [%], Month 12 [%]. Here's what breaks the model positively:
[specific lever we haven't pulled yet]."
```

### P2 典型提问 + 应答台词库

**Q1: "Show me your cohorts."**

❌ 差答案：展示 aggregate growth，无 cohort 切分

✅ 好答案：
```
"Here's our Q[X] cohort by signup quarter. Retention M1 [%], M3 [%],
M6 [%]. You'll notice Q2 cohort is flatter than Q1—that's because
we changed [specific onboarding]. Q3 cohort recovered to [%] because
we fixed [issue]. Here's the test we're running now on Q4..."
```

**Q2: "What's your CAC breakdown by channel?"**

✅ 好答案：
```
"Three channels. Paid social: CAC $[X], payback [Y] months, at
$[volume]/month currently. Content/SEO: CAC $[X], payback longer
but declining. Referral: CAC effectively $[low], but capacity
capped at [%] of growth. The thesis is that we scale paid to [$X]
until CAC/LTV drops below [ratio], then we shift mix."
```

**Q3: "What's your growth model for the next 12 months?"**

✅ 好答案（给 P2 一个 spreadsheet，不是一个 pitch）：
```
"Three scenarios. Base case: [$X] ARR by Q4, assumes [assumptions].
Stretch case: [$Y] ARR, assumes [additional lever]. Downside:
[$Z] ARR if [risk] materializes. Here's the spreadsheet—let's
poke holes in the base case together."
```

**Q4: "How do you know this will scale?"**

✅ 好答案：
```
"Three pieces of evidence. First, our top decile cohorts behave like
[benchmark company] at similar stage. Second, the channel we're
scaling behaves more like [PLG example] than [ad arbitrage example],
which means CAC deflation potential. Third, we've done [specific
experiment] that validates the next tier of scale. Here's what I
can't answer yet: [honest uncertainty]. We need [specific amount]
to de-risk that."
```

### P2 不喜欢的话
- 「We're building for a 10-year vision」（P2 要 12-month model）
- 「Metrics don't tell the whole story」（P2 认为 metrics 就是故事）
- 「We haven't measured that yet」（Fatal，P2 立即降权）
- 「Our contrarian view is...」（P2 认为 contrarian 是免责借口）

### P2 的决策关键
如果 P2 是 Champion，他会说：「The unit economics work at [Z scale]. This is a capital efficiency story, not a moonshot.」
如果 P2 反对，他会说：「Numbers are soft. Come back when cohorts are sharper.」

---

## P3 平台玩家 — 创始人应战台本

### 识别信号
- 问「how big can this get?」
- 关心 category-defining 可能性
- 对 narrative / 媒体曝光敏感
- 谈 portfolio 公司 synergy

### 开场 hook
```
"This isn't a product, this is a category. Today the category doesn't
exist—everyone's competing in [adjacent category]. In 5 years, the
category will be [new name], and the dominant player will have:
[platform attribute 1], [2], [3]. We're building that player.
Here's our progress so far..."
```

### P3 典型提问 + 应答台词库

**Q1: "How big can this become?"**

❌ 差答案：「$50M ARR by Year 5」（P3 觉得你不 ambitious）

✅ 好答案：
```
"Think about it this way. Today there's [$X]B spent on [existing
category]. Our thesis is that [shift] will redirect [Y%] of that to
the new category we're creating. That's a [$Z]B TAM opening.
In 7-10 years, if we execute, we're the [platform in X position].
Here's the first adjacent market we'll enter: [market 2]. Here's
the second: [market 3]."
```

**Q2: "Why are you the team to build this?"**

✅ 好答案：
```
"Three reasons. First, category creation requires 7+ years of
obsession—I've been thinking about [problem] since [year/event].
Second, platform plays require parallel investment across product
/ community / ecosystem—we've already done [specific proof of
this multi-threaded execution]. Third, we have access to [unique
distribution / partnership / data] that nobody else in the space
has."
```

**Q3: "What's the viral / network effect mechanic?"**

✅ 好答案：
```
"Three layers of network effect. First, [direct network: more
users → more value per user]. Second, [data moat: more users →
better product]. Third, [ecosystem: more users → third parties
build on top, which attracts more users]. Here's the current
K-factor: [number]. Here's the path to K > 1: [specific product
lever]."
```

**Q4: "What's your defensibility?"**

✅ 好答案：
```
"Not technology—technology is table stakes. Defensibility comes from
three compounding assets: data, community, and ecosystem. In 3 years
we'll have [data asset nobody can replicate], [community with
[specific behavior]], and [ecosystem with [# of third-party
integrations]]. That's the moat. Attempting to replicate it in 2029
requires time travel."
```

### P3 不喜欢的话
- 「We're a SaaS tool」（太小）
- 「Our target is $10M ARR」（不 ambitious）
- 「We don't need to think about adjacent markets yet」（P3 觉得你在 miss 大机会）
- 「The platform will come later」（P3 认为你不懂 platform dynamics）

### P3 的决策关键
如果 P3 是 Champion，他会说：「This is a category-creating bet. The downside is bounded, the upside redefines the market.」
如果 P3 反对，他会说：「This is a feature, not a platform. I don't see how this scales to our check size.」

---

## P4 品味大师 — 创始人应战台本

### 识别信号
- 赞你的产品设计
- 问「为什么这个按钮不是圆形？」这种细节
- 对 founder-market fit 非常关注
- 问你自己怎么使用产品

### 开场 hook
```
"Let me just show you the product. [Demo 30 seconds to 2 minutes,
obsess over 3 specific design decisions].
I can talk about TAM and unit economics after, but I want you to
feel the product first—because that's where our moat is."
```

### P4 典型提问 + 应答台词库

**Q1: "Walk me through why you made this design decision."**（指向 UI 某个细节）

✅ 好答案：
```
"Here's the thinking. [Explains user psychology + micro-design
trade-off]. We tried [3 other versions]. Each failed because
[specific user feedback]. This version works because [subtle
insight about user behavior]. It took [X weeks/months] to get
to this."
```

**Q2: "Do you use your own product every day?"**

✅ 好答案（不只是 Yes）：
```
"Every day, and here's what I noticed yesterday: [specific micro-
insight from own usage]. That's going to become [feature X] in
Q[Y]. I can't build products I don't live in."
```

**Q3: "What do your users love about the product?"**

❌ 差答案：「NPS 60」（数字对 P4 不够）

✅ 好答案：
```
"Read this [specific user message or tweet]. Here's another
one. [Read it aloud with emotion]. What users say about us is
they come back not because we're 'better,' but because no one
else gets them. I save these. I have [N] of them. Want to read
three more?"
```

**Q4: "What's your aesthetic philosophy?"**

✅ 好答案：
```
"Three beliefs. First, [aesthetic belief about minimalism/
complexity/reference]. Second, [belief about user agency vs
guidance]. Third, [belief about how software should feel—
tool vs partner vs whatever]. These aren't taste preferences,
they're operating constraints on every decision we make."
```

### P4 不喜欢的话
- 「The design is not our differentiation」（P4 relying on design taste）
- 「We optimize for growth, not beauty」（P4 认为 beauty is growth）
- 「Here's our feature roadmap」（P4 要 philosophical 而不是 checklist）
- 「We'll hire a design team later」（P4 认为 design 必须从 day 1 inside founder）

### P4 的决策关键
如果 P4 是 Champion，他会说：「This founder builds products I'd use. That's the whole thesis.」
如果 P4 反对，他会说：「The taste isn't there. I don't believe this team ships the right product.」

---

## P5 企业收割机 — 创始人应战台本

### 识别信号
- 问「ACV, logo count, net revenue retention」
- 关心 sales motion（inside sales / field sales）
- 问 customer reference
- 谈 enterprise 采购 cycle

### 开场 hook
```
"Here's where we are: [$X] ARR, [Y] enterprise logos, [Z]% NRR,
ACV [$amount]. Here's the sales motion: [inbound/outbound/PLG
hybrid]. Here's the 3 customer references I'd point you to:
[Name], [Name], [Name]. Here's how we get to $100M ARR..."
```

### P5 典型提问 + 应答台词库

**Q1: "What's your Net Revenue Retention?"**

✅ 好答案：
```
"Trailing 12 months NRR is [%]. Broken down: gross retention [%],
expansion [%], churn [%]. The expansion is driven by [specific
motion: seat expansion / product line cross-sell / usage tier].
Our top 20% customers are at [NRR %]—that's the cohort we
optimize for."
```

**Q2: "Walk me through your largest customer."**

✅ 好答案：
```
"[Customer name, if reference-permitted, else description].
Started [date] at ACV [$X]. Expanded to [$Y] in Month 12 because
[specific expansion event]. They've hit [usage milestone]. Main
decision-maker is [title], champion is [title]. Renewal up
[date]—confidence level: [low/medium/high]."
```

**Q3: "What's your CAC payback in enterprise?"**

✅ 好答案：
```
"Current payback [X] months, but that blends [mid-market] and
[enterprise]. Pure enterprise payback is [Y] months because
ACV is [$Z] but sales cycle is [W months] and discount from
list is [%]. We're tightening that by [specific motion]—
expect payback to compress to [target]."
```

**Q4: "How are you going to get to $100M ARR?"**

✅ 好答案：
```
"Three horizons. H1: scale current ICP [current state] to [$X]
ARR. This is capital-in-hand if we hire [# reps] at [$Y quota].
H2: expand into [adjacent ICP] at Year [#]—we've validated with
[# pilots]. H3: platform play—sell [second product line] into
existing install base at [$Z uplift per customer]."
```

### P5 不喜欢的话
- 「We're product-led, sales-led doesn't matter」（P5 认为你不懂 enterprise）
- 「We haven't thought about NRR yet」（Fatal）
- 「Our first 10 customers were friends」（不可重复的模式）
- 「Enterprise comes later」（P5 认为 enterprise 是主菜）

### P5 的决策关键
如果 P5 是 Champion，他会说：「The GTM motion is capital-efficient at scale. I see $100M ARR in 5 years.」
如果 P5 反对，他会说：「The sales motion doesn't scale past $10M. Team needs VP Sales before I can support this.」

---

## P6 工程原教旨 — 创始人应战台本

### 识别信号
- 问 architecture / 技术 stack
- 关心 developer experience / API design
- 对 GTM 和 marketing 不感兴趣
- 问 open source / community strategy

### 开场 hook
```
"Here's the technical insight: [specific architectural bet that
most don't see or believe]. Here's why it matters: [performance
/ cost / capability implication]. Here's what we built:
[concrete implementation + link to repo/demo]. Here's why
developers will adopt us: [specific DX delight]."
```

### P6 典型提问 + 应答台词库

**Q1: "Walk me through your architecture."**

✅ 好答案（带白板图）：
```
"[Draw diagram]. Three layers. Layer 1: [infra bet]. Layer 2:
[protocol / abstraction]. Layer 3: [developer API]. Key decision
was [specific trade-off]: we chose [approach A] over [approach B]
because [performance/cost/flexibility reason]. The cost was
[specific downside we accepted]. Here's the test data."
```

**Q2: "Why should developers use you instead of [incumbent]?"**

✅ 好答案：
```
"Three reasons. First, our API does in [X lines] what theirs does
in [Y lines]. Here's the concrete comparison [code snippets].
Second, our latency is [A ms] vs their [B ms]—here's the
benchmark. Third, [something delightful that isn't in the
marketing—like 'we have a better error message' or 'we expose
the thing they hide']."
```

**Q3: "What's your open source strategy?"**

✅ 好答案：
```
"[OSS component] is under [license], with [# GitHub stars]. The
commercial offering is [specific feature set] on top. Community
strategy is [community-building motion]. Monetization vector is
[where OSS ends and commercial begins]. Concrete examples of
companies who have successfully done this split: [1-2 references]."
```

**Q4: "What's your developer adoption path?"**

✅ 好答案：
```
"Funnel looks like: [Hacker News / Twitter / blog] → [docs /
tutorial] → [first successful API call in <5 min] → [first
project deployed in <1 hour] → [paid tier at [specific usage
threshold]]. Current stage: [%] drop-off at [specific step].
We're fixing that by [DX investment]."
```

### P6 不喜欢的话
- 「Developers don't matter, end-users do」（P6 觉得你不懂 bottom-up sales）
- 「We're closed-source」（视具体 case，但 P6 对 closed-source 默认怀疑）
- 「Our stack is proprietary」（P6 认为 proprietary 不是 moat，实际壁垒是 developer love）
- 「We'll open source later」（P6 立即怀疑你的决心）

### P6 的决策关键
如果 P6 是 Champion，他会说：「Technical founders building for technical users. This compounds. I want in.」
如果 P6 反对，他会说：「The architecture doesn't have depth. This could be cloned in 6 months by anyone on AWS.」

---

## 多 Persona meeting 的实战策略

### 场景 1：P1 + P2 同坐（Thiel 式 + Sequoia 式）
**冲突**：P1 要 contrarian，P2 要 metrics
**你的策略**：开场给 contrarian thesis（吸 P1），中段给 hard numbers（吸 P2），结尾给 Peter Thiel-style truth（P2 不反对数据+故事组合）
**错误做法**：纯数据（P1 走神）或纯故事（P2 扣分）

### 场景 2：P3 + P5 同坐（平台玩家 + 企业收割）
**冲突**：P3 要 platform 宏大叙事，P5 要 enterprise pipeline
**你的策略**：先给 enterprise pipeline（地板）再给 platform vision（天花板）；证明你是 category creator 且 GTM 能 ship
**错误做法**：先宏大叙事再说没 revenue（P5 扣分）

### 场景 3：P4 + P5 同坐（品味 + 企业）
**冲突**：P4 要 design obsession，P5 要 sales efficiency
**你的策略**：演示产品细节（吸 P4）→ 但解释这个 design 细节如何 drive enterprise adoption（说服 P5）
**错误做法**：把 design 和 GTM 说成两个不同 motion

### 场景 4：P6 + P3 同坐（工程原教旨 + 平台）
**冲突**：P6 要 technical depth，P3 要 market breadth
**你的策略**：技术架构决定 category creation 的可能（技术是 moat 的源头，不是 detail）
**错误做法**：纯技术（P3 走神）或纯 vision（P6 扣分）

---

## 如何识别 meeting 里的 persona

**会议开始前 5 分钟注意**：
- 他们 LinkedIn 简介 / Twitter 上的语言
- 他们过往投资组合里的公司类型（看他们投资过的 website / 创始人 tweet 风格）
- 他们问的第一个问题通常暴露 persona

**会议开始第 1-2 个问题**：
- 如果第一个问题是「why now」→ P1/P3
- 如果第一个问题是 metrics → P2/P5
- 如果第一个问题是关于产品细节 → P4
- 如果第一个问题是关于技术 → P6

**问「对你来说投资成功是什么样子？」**：
- 「A fund-returning outlier」= P1
- 「Clear path to $1B+ revenue」= P2
- 「Category-defining company」= P3
- 「A product people can't live without」= P4
- 「Dominant B2B SaaS」= P5
- 「Developer-first leader」= P6

---

## changelog

- v1.0 2026-04-17：首版。覆盖 6 个美国 VC persona 的创始人应答台本、典型提问应对、不喜欢的话、多 persona 同坐策略、识别方法。与姊妹文件 `vc-pitch-killtest/persona-debate-scripts.md` 差异化（VC 内部辩论 vs 创始人外部应答）。
