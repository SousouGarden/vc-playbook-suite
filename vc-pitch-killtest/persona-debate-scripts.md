# Persona Debate Scripts — 美国 VC 投委会逐字辩论模拟器

> v4.0 新增。与主文件 Phase 2「拍桌子动态」绑定使用。
> 中国版对应 `china-fundraising-wargame/persona-debate-scripts.md`。

**核心目的**：把 P1-P6 从「评估标签」升级为「能生成投委会辩论逐字稿」的博弈引擎。创始人进投委会前，必须在脑子里先跑一遍这场辩论——知道谁会拍桌子挺你、谁会质疑什么、Champion 在哪一刻被压制、你需要给他什么弹药翻盘。

**与主文件拍桌子动态的区别**：
- 主文件给的是「Champion 是谁+需要什么弹药」的结论
- 本文件给的是**辩论过程的逐字剧本**——Champion 的开场白、反对者的三轮进攻、Champion 的三层防线、最终拍板的那句话

---

## 使用方式

主文件 Phase 2 得出投委会投票（≥1 FUND 且非 0 KILL）后，对 **Champion** 和 **最危险反对者** 两个 Persona 生成逐字辩论剧本。

**输出格式：三幕剧** ——
- **Act I**：Champion 开场陈述（为什么领投 + 三条理由）
- **Act II**：反对者 2-3 轮进攻（每轮一个角度 + Champion 防守）
- **Act III**：Champion 拍板句式（用该 Persona 的世界观收束）

台词必须体现 Persona 的语气、用词、关注点（**不是中性分析**）。

---

## P1 异端猎手 — 辩论剧本模板

### 当 P1 是 Champion

**Act I · 开场白（P1 拍桌子版）**：

> "Partners, I'm leading this one. Here's why in three truths.
>
> **First**, this company is betting on something the consensus is wrong about. The consensus says [共识], but the founders believe [反共识 insight]. If they're right, the market doesn't just grow — it flips. That's the kind of bet we're in business for.
>
> **Second**, there is no better. There is only different. Everyone else in this space is iterating on the same assumption stack. These founders broke the stack. Look at [具体结构差异]. That's not a product feature, that's a philosophical commitment.
>
> **Third**, the moat isn't technology — it's the willingness to be wrong for five years before being right. Nobody in our portfolio has that. We need it."

**P1 最常被 P2 攻击的弹药库**：

| P2 的质疑 | P1 的防守 |
|----------|----------|
| "The unit economics don't work at any scale you've modeled." | "Unit economics at scale are a lagging indicator of product-market obsession, not a leading indicator of company quality. Sequoia missed Airbnb on a unit economics model. I don't want to be that VC." |
| "TAM is too small to justify our check size." | "TAM is a model of the present. Contrarian bets redefine the TAM. Nobody modeled the TAM for 'renting a room in a stranger's apartment' in 2008. I'm not buying into a TAM, I'm buying into a thesis-level insight." |
| "There are three well-funded competitors already." | "Wrong. There are three well-funded imitators. None of them have the founders' insight. Competition at the capital layer is irrelevant — what matters is competition at the insight layer, and there they're alone." |

**P1 最常被 P4 攻击的弹药库**：

| P4 的质疑 | P1 的防守 |
|----------|----------|
| "No paying users. This is vapor." | "Paying users in Year 1 is a proxy for product-market fit in small markets. In the markets Peter Thiel actually cares about, Year 1 revenue is a distraction. Stripe had no paying users for 18 months. PG turned them down. Are we PG right now?" |
| "Founder doesn't use their own product every day." | "The founder isn't the user. The user is someone they understand at a level the user themselves can't articulate. That's a different pattern, and a rarer one." |

**P1 的拍板句式**：

> "I hear the concerns, and I weight them at zero. Here's the deal: **if this works, it's a 100x. If it doesn't, we lose 1x. The portfolio math demands we take this bet. The only question is whether we want to explain to LPs five years from now why we passed on the one deal that would have justified the entire fund.** I'm prepared to have that conversation. Are you?"

### 当 P1 是最危险反对者

**P1 的否决逻辑**（当 idea 是 me-too 或渐进改良）：

> "I can't support this. Three reasons.
>
> **First**, this is a better version of an existing thing. Better is a losing strategy. The winners of our portfolio all chose different over better.
>
> **Second**, the founders can't articulate a single contrarian belief. I asked them 'what important truth do very few people agree with you on,' and they gave me a market-sizing answer. That's disqualifying.
>
> **Third**, the moat is execution. Execution is not a moat — it's a tax. Everyone eventually executes. The question is whether there's anything underneath the execution that actually differentiates, and in this case there isn't."

**P1 反对时的拍板句式**：

> "Look, I'll fund the next version of this idea — when they come back with a contrarian view of the world instead of a better version of an existing one. But this? **This is the kind of deal that returns 2x, feels good, and quietly kills the fund.**"

---

## P2 增长机器 — 辩论剧本模板

### 当 P2 是 Champion

**Act I · 开场白（P2 拍桌子版）**：

> "I'm taking this one. Three numbers.
>
> **One**: LTV-to-CAC ratio of [X:1] at current cohort. Not projected. Actual. This is not normal for a company at this stage.
>
> **Two**: TAM is $[X]B and the company is the category-defining name in a market where category definition matters more than share. Recall that Salesforce owned the category before owning the share.
>
> **Three**: We've priced in the execution risk. Even in the 40th percentile outcome, this fund gets its money back. That's the real test — not the upside, the downside."

**P2 最常被 P1 攻击的弹药库**：

| P1 的质疑 | P2 的防守 |
|----------|----------|
| "This is a better version of [existing incumbent]." | "Yes. And 'better' wins when the market is fragmented enough and switching costs low enough. This market has both. I'm not buying a contrarian insight, I'm buying an execution vehicle in a large underpenetrated market. Those exist too." |
| "The founders are iterating, not reinventing." | "Iteration is underrated. Most generational outcomes — Stripe, Datadog, Crowdstrike — were iteration plays, not reinvention plays. They just iterated better than the competition." |

**P2 最常被 P3 攻击的弹药库**：

| P3 的质疑 | P2 的防守 |
|----------|----------|
| "Why now? I don't see a tailwind." | "The tailwind is boring but real: [具体 macro/regulatory/behavioral shift]. This isn't a 'AI changes everything' story, it's a 'CFO buying behavior shifted after [event]' story. Both types of tailwinds make companies." |
| "This feels like a bet on the category, not the company." | "That's exactly what it is. Category leaders in large markets capture 60%+ of category value. Our risk is category-not-company, and I'd rather bet on category in a market this large." |

**P2 的拍板句式**：

> "I've run the model three ways. In the base case we return 4x. In the bear case we return 0.8x. In the bull case we return 12x. **Weighted expected value is 5.2x, which clears our hurdle. Fund math says yes. I'm not asking you to feel excited — I'm asking you to respect the math.**"

### 当 P2 是最危险反对者

**P2 的否决逻辑**：

> "I'm a no. The numbers don't work and I can't fake conviction around that.
>
> **The CAC is [X]. The LTV assumption requires retention that is 3x industry benchmark. No company has ever delivered that retention without a product moat this team hasn't built.**
>
> **TAM is inflated. They include [不应该算进 TAM 的市场] in their number. Adjusted TAM is $[真实数字], which isn't enough for fund math.**
>
> I don't have a problem with the founders. I have a problem with the spreadsheet. Spreadsheets don't lie as easily as pitches do."

**P2 反对时的拍板句式**：

> "Look, if I'm wrong, we'll pay a 10x regret tax. If I'm right, we'll save the fund 20% of its capital. **I'll take those odds every time. Pass.**"

---

## P3 场景赌徒 — 辩论剧本模板

### 当 P3 是 Champion

**Act I · 开场白（P3 拍桌子版）**：

> "This is a 'why now' deal and we're three months ahead of consensus. Let me sell it.
>
> **What changed in the last 12 months**: [具体技术/监管/behavioral shift]. This wasn't possible 18 months ago. In 18 more months, every tier-one will be chasing it and the entry price will be 3x.
>
> **Who else is in this**: Nobody. Yet. Two adjacent teams are probably working on it but haven't shipped. We have a 90-day window before consensus forms.
>
> **The founders**: They're not just building a product, they're defining a category. [Specific founder insight]. That's the thing you can't time — either you trust they see the shape of the future or you don't. I do."

**P3 最常被 P4 攻击的弹药库**：

| P4 的质疑 | P3 的防守 |
|----------|----------|
| "No revenue, no customers, no paying beta." | "If they had revenue we'd be paying 5x the price. The window to invest is exactly the period when the revenue doesn't exist yet. Revenue is a trailing indicator of every thesis I've ever been right about." |
| "This is a PPT deck, not a company." | "Most generational companies were PPT decks when we funded them. The question isn't 'does the company exist today' — it's 'does the category the company is defining exist in 36 months.' I'm betting yes." |

**P3 最常被 P2 攻击的弹药库**：

| P2 的质疑 | P3 的防守 |
|----------|----------|
| "Your TAM assumes a category that doesn't exist yet." | "Correct. That's the only kind of TAM worth paying attention to. Category-defining companies aren't priced against their current TAM, they're priced against the TAM they create. You're using the wrong yardstick." |

**P3 的拍板句式**：

> "Here's the thing about 'why now' deals: you only see them clearly in retrospect. In real time, they all look slightly crazy and slightly premature. That's not a bug, that's the signature. **If this deal felt 'obvious,' the price would already be 10x. We're paying for the privilege of seeing it 90 days before everyone else. I'll take that price.**"

### 当 P3 是最危险反对者

**P3 的否决逻辑**（当 timing 不对）：

> "The 'why now' doesn't exist. Three problems.
>
> **First**, this exact idea was tried in [之前失败的年份] and failed. The founders can't articulate a single reason why the environment has changed. That's a disqualification.
>
> **Second**, the technology cliff they're betting on is [X months/years] away, not 'now.' They're 12 months too early. Early is wrong.
>
> **Third**, there are three adjacent teams executing against the same thesis with better distribution. The narrative window is open, but these aren't the founders who will own the narrative."

---

## P4 现金流原教旨 — 辩论剧本模板

### 当 P4 是 Champion

**Act I · 开场白（P4 拍桌子版）**：

> "I'm in. Three things.
>
> **They're shipping**: Shipped [具体产品/feature] in the last 8 weeks. Not wireframes. Not roadmaps. Code in production.
>
> **Somebody is paying**: [X] paying users / $[Y] MRR. At this stage, I don't care if it's $10K MRR — the fact that humans with bank accounts are voluntarily sending money matters more than any TAM slide.
>
> **The founders use the thing**: They're their own first user. They hit their own bugs. They care about their own UX. Every successful founder I've ever backed had this property."

**P4 最常被 P3 攻击的弹药库**：

| P3 的质疑 | P4 的防守 |
|----------|----------|
| "$10K MRR isn't a signal, it's a rounding error. Why this, why now?" | "I don't have a 'why now' story. I have a 'they'll still be shipping in 24 months when everyone else stops' story. That's enough. The market always rewards founders who outlast the tourist capital." |
| "This is a small business, not a venture." | "Every big company was a small business first. The question isn't 'is it big now,' it's 'do these founders compound.' Compound makes small into large. Our job is to find the compound." |

**P4 最常被 P1 攻击的弹药库**：

| P1 的质疑 | P4 的防守 |
|----------|----------|
| "This is incremental. No contrarian bet." | "I'm not in the business of being contrarian. I'm in the business of being right. Contrarian is a strategy for VCs who don't trust their own taste in founders. I trust mine." |

**P4 的拍板句式**：

> "Here's my rule: **I fund founders I'd want to work for if I weren't running money.** These two, I'd work for. That's my entire thesis. I'm not going to dress it up in a framework."

### 当 P4 是最危险反对者

**P4 的否决逻辑**：

> "No. Three things and I'll be brief.
>
> **No users.** Zero humans voluntarily using the product.
>
> **No shipping velocity.** They showed me a roadmap, not a changelog. Changelogs are signal, roadmaps are noise.
>
> **Founder doesn't use the product.** They're building for a user they don't understand at a visceral level. You can't fake that."

**P4 反对时的拍板句式**：

> "Come back when someone is paying. Not when the model says someone will pay. When actual money has moved."

---

## P5 国产替代棋手 — 辩论剧本模板

> 注：P5 在美国语境中较少出现（美版更像是 a16z American Dynamism 或 SpaceX-style 「美国战略自主」派系）。下述模板同时兼容两种语境。

### 当 P5 是 Champion

**Act I · 开场白（P5 拍桌子版）**：

> "This is a strategic infrastructure deal. Three reasons I'm leading.
>
> **First**, the space they're building in is a named strategic priority — [specific government/industrial policy reference]. The capital environment for this category is about to turn on, and we're in before the turn.
>
> **Second**, the alternative today is [foreign incumbent], which creates a structural dependency that the market is quietly unwilling to accept going forward. These founders are the credible domestic alternative.
>
> **Third**, the downside is capped by the strategic value. Even if the business plan doesn't perform, the strategic asset is bought out by someone who needs the capability. We have a floor most deals don't."

**P5 的拍板句式**：

> "**Venture math usually says 'upside matters, downside is irrelevant because it's a zero.' This deal inverts that. The downside isn't zero — there's a strategic buyer at a floor. The upside is the domestic category definition. That's an asymmetric profile I don't see often. I'm in.**"

### 当 P5 是最危险反对者

**P5 的否决逻辑**（依赖美国技术栈且无 Plan B）：

> "I can't support this. The entire tech stack they depend on is licensed from [US vendor] with a single point of failure. One geopolitical shift and they're a zero. I'm not going to explain to my LPs that we invested in a company whose existence depends on the goodwill of a foreign government."

---

## P6 社区嗅觉王 — 辩论剧本模板

### 当 P6 是 Champion

**Act I · 开场白（P6 拍桌子版）**：

> "This is a community-native bet. Three signals.
>
> **One**: The landing page already has [X] signups from a soft launch with zero paid marketing. That's pure organic signal.
>
> **Two**: The founders are the top 0.01% of their own community. They wrote the stuff everyone in the niche has read. This isn't a founder attempting to build for a community — they *are* the community.
>
> **Three**: I tried the demo. I wanted to post it immediately. That's my entire diligence framework and it hasn't failed me yet."

**P6 最常被 P2 攻击的弹药库**：

| P2 的质疑 | P6 的防守 |
|----------|----------|
| "HN love doesn't pay bills." | "HN love is the leading indicator. Bills are the trailing indicator. If you only invest on trailing indicators, you buy at the top. I buy at the signal, which is when the community declares the founder." |
| "Community businesses don't scale." | "Some don't. Figma did. Notion did. Obsidian is. The pattern is: communities that form around a tool scale when the tool becomes a category verb. This one's becoming a verb." |

**P6 的拍板句式**：

> "**If I can't share this deal with five smart friends in my feed and have them say 'wait, is this real?' — I don't fund it. I sent it to five people yesterday. All five said 'how do I invest.' That's my answer.**"

### 当 P6 是最危险反对者

**P6 的否决逻辑**（纯 PPT，无可演示东西）：

> "No demo, no deal. I'm not a thesis investor, I'm a reflex investor. If I can't feel it, I can't fund it. The founders come back with a prototype that I can play with in 10 minutes, we have a conversation. Until then, there's nothing for me to react to."

---

## 交叉辩论矩阵（谁攻击谁最致命）

| Champion → 反对者 | 攻击向量 | Champion 最脆弱点 |
|-------------------|---------|----------------|
| **P1 → P2** | 数字理性攻击哲学直觉 | 「你的反共识洞察能在 DCF 里兑现吗？」 |
| **P1 → P4** | 地面执行攻击空中叙事 | 「你的 contrarian 客户在哪里？」 |
| **P2 → P3** | 单位经济学攻击 timing 叙事 | 「你的 why now 在模型里是个什么数？」 |
| **P2 → P1** | 历史数据攻击直觉判断 | 「95% 的 contrarian bets 是 0。你的 conviction 从哪里来？」 |
| **P3 → P2** | 非线性攻击线性外推 | 「你的 TAM 假设 5 年后的世界跟今天一样。我的假设是它不一样。」 |
| **P3 → P4** | 未来攻击现在 | 「你要的 paying users 会来的，但不是现在。现在的代价是便宜的估值。」 |
| **P4 → P1** | 常识攻击疯狂 | 「contrarian 不是借口。给我看用户。」 |
| **P4 → P3** | 地面数据攻击叙事 | 「'why now' 写在 deck 里就是 'we don't know'。」 |
| **P5 → P1** | 战略确定性攻击哲学不确定性 | 「我们的 LP 不吃 contrarian。他们吃战略价值。」 |
| **P5 → P3** | 政策时钟攻击市场时钟 | 「政策窗口的 timing 不是 market timing。你说的 why now 在政策眼里还早。」 |
| **P6 → P1** | 感性即时攻击冷抽象 | 「philosophy 不发帖。社区发帖。社区已经说话了。」 |
| **P6 → P4** | 分发攻击 bottom-up | 「你要的 paying users 不是付费，是 vibes。这个 vibe 对了。」 |

---

## 使用铁律

1. **Champion 的开场必须三句话讲完**，超过三句话 = 没有 conviction
2. **反对者的攻击必须具体到数字或事件**，「我不相信」不是攻击，是抱怨
3. **Champion 的防守必须在该 Persona 的世界观内**（P1 的防守不能用 P2 的语言）
4. **拍板句式必须用该 Persona 的招牌隐喻**（P1 讲哲学、P2 讲 math、P3 讲 timing、P4 讲 shipping、P5 讲战略、P6 讲 feed）
5. **不能有跨 Persona 的妥协**——真实投委会很少是「折中」的，是「有人让步或有人出局」
6. **输出要附「创始人应准备的弹药」清单**，让剧本变成可执行的 pitch 准备

---

## changelog

- v1.0 2026-04-17：首版美版。P1-P6 各自 Champion/反对者场景辩论剧本。交叉辩论矩阵。对齐 `china-fundraising-wargame/persona-debate-scripts.md` 的三幕剧格式。
