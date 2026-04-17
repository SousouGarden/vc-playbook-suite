---
name: VC Due Diligence Simulator
description: 从 VC 分析师视角模拟 3-week DD 过程——生成他们会挖的坑、会打的 reference call、会审的数据、会问的 24 个刁钻问题。创始人用来预演 DD，把所有弹药准备好。配合 founder-fundraising-wargame + term-sheet-negotiator 使用。
version: v1.0
created: 2026-04-17
---

# VC Due Diligence Simulator — 从 VC 视角模拟 DD 过程

> **定位**：
> - 不是「创始人应该准备什么材料」（那是 DD checklist）
> - 而是「VC 分析师在 3 周内到底会挖哪些问题、call 哪些 reference、审哪些数据、从哪个角度 break 这个 deal」
> - 创始人用这个 simulator 做 **"Red Team"**：先让自己被虐，再补足弹药去 pitch

**姊妹 skills**：
- `founder-fundraising-wargame`：融资整体战略
- `term-sheet-negotiator`：TS 条款博弈（post-DD）
- `vc-pitch-killtest`：pre-pitch 自杀测试

---

## 核心认知：DD 不是 formality，是 kill test

**创始人的 misconception**：「TS 签了就基本是 done」
**现实**：**20-40% of signed TS fail during DD**（根据 PitchBook 2023-2024 数据）

DD failure 的三大 root cause：
1. **创始人讲的 story 和数据对不上**（TAM 吹大、retention 美化、churn 隐藏）
2. **Reference call 暴露 founder 或员工 red flag**
3. **Technical / legal 发现之前不 visible 的 skeleton**

DD 是 VC 在「confirm 自己 thesis」和「find an excuse to back out」之间摆动。**每个 DD 信号都有权重**——signal strong enough 就 close、signal weak 就 walk。

---

## 3-Week DD Timeline 解构

### Week 1：Structured Questions + Data Room

**VC 目标**：建立数据 baseline，对比 pitch 时的声明

**具体行动**：
- 发 24-48 个 structured questions（见下文）
- 请求 data room access（所有 legal docs、financial records、employee list、customer metrics）
- 分析师独立核算 unit economics（不信你的 LTV/CAC 数字，重算）
- Run 公开检查（litigation history、domain registration、trademark search）

**创始人准备**：
- Data room 必须 already 100% ready（如果你 Week 1 才开始 scramble 组织，VC signal -10%）
- Structured questions 要在 48 小时内返回（delay > 72 小时 = signal weak）
- 所有数据三角验证（GA4 matches Stripe matches Mixpanel）

### Week 2：Reference Calls

**VC 目标**：triangulate founder + team + product claims，识别 red flag

**具体行动**：
- Founder reference calls（3-5 个）：past employer、co-founder、mentor
- Customer reference calls（3-5 个）：paying customers、churned customers
- Employee calls（如果有 exits）：前员工
- Competitor intelligence（lightweight）：找 competitor 的 investor 或员工 chat
- **Back-channel calls**（你不知道的那种）：VC 的 network 里找 6-7 个 random contacts who might know you
- Domain experts（技术 / market / regulatory）

**创始人准备**：
- 提前 prime references（告诉他们 VC 可能来 call，what deal）
- Prepare list of "inviters" references（happy customers）和 "tough" references（hard but fair customers）
- 对 churn customers，提供 context（why they churned, what's different now）
- **Key**：VC 的 back-channel calls 是 wild card——你无法控制。这就是为什么你**过去的行为 compounds**，现在到 founder 阶段才想修复 reputation 来不及

### Week 3：Deep Dives + Closing Checklist

**VC 目标**：针对 Week 1-2 发现的 issues 做 deep dive，最终形成 investment memo

**具体行动**：
- Technical deep dive（CTO 和 VC 带来的 technical advisor / operating partner 深聊）
- Financial audit-style review（accountant 或 operator 帮 VC 看数据）
- Legal review：cap table、IP assignment、customer contracts、employee agreements
- Final founder meeting：2-3 小时，基于 Week 1-2 findings 深 probe
- IC meeting：VC 内部投委会 approval

**创始人准备**：
- 任何 Week 1-2 提出的 issue 在 Week 3 必须有 response plan
- Final meeting 要带上 **cofounder + 1-2 key team members**（让 VC 看 team depth）
- 不要 over-commit 在 closing timeline（保留灵活空间）

---

## VC 会问的 24 个刁钻问题（分 8 类）

### Class 1：Market / TAM Kill Questions

**Q1**：「Walk me through your top-down TAM calculation. Then show me the bottom-up. Why do they differ?」
- **Trap**：创始人的 top-down 通常用 industry report 数字（膨胀）；bottom-up 更 reliable
- **Answer**：承认 gap，explain why bottom-up is more reliable，show the delta analysis

**Q2**：「If your thesis is right, what's the 10-year TAM? What's the serviceable TAM? What's the realistic obtainable TAM for you?」
- **Trap**：大部分创始人 only know total TAM
- **Answer**：有明确的 TAM → SAM → SOM 框架 + 数据支持

**Q3**：「Who is NOT your customer? And why?」
- **Trap**：创始人说 "everyone is our customer"（表示 PMF 弱）
- **Answer**：清晰的 exclusion criteria + 为什么这些 segment 不是 fit

---

### Class 2：Customer / Product Kill Questions

**Q4**：「Please share 3 customer interviews — both positive and negative. Raw transcripts or recordings」
- **Trap**：创始人只 share 正面 feedback
- **Answer**：提前 prepare 3 balanced interviews (positive + cautionary + churn)

**Q5**：「Your churned customers — have you talked to them post-churn? What did they tell you?」
- **Trap**：创始人没做过 churn post-mortem
- **Answer**：systematic churn interview program + learnings

**Q6**：「Show me your top 10 customers' actual usage data, not self-reported NPS」
- **Trap**：NPS 可能被 biased（只看 engaged users）
- **Answer**：Product analytics data show real usage depth + frequency

---

### Class 3：Unit Economics Kill Questions

**Q7**：「Your CAC payback — walk me through the calculation. What discount rate? Does it include ramp time? Free trial cost?」
- **Trap**：简化的 CAC payback 通常低估真实成本
- **Answer**：fully-loaded CAC（包含 sales 招聘、training、tools）+ proper discount rate

**Q8**：「LTV — what retention assumption are you using? What's the actual churn cohort data?」
- **Trap**：LTV 常用 aggressive retention assumption
- **Answer**：Cohort-based LTV calculation + sensitivity analysis

**Q9**：「Gross margin breakdown — what goes into COGS? Hosting, payment processing, support, customer success, what else?」
- **Trap**：创始人算 gross margin 时忽略 customer success (technical 属于 COGS or OpEx)
- **Answer**：Transparent breakdown + justify each category

---

### Class 4：Competition / Moat Kill Questions

**Q10**：「If [Incumbent] decided to build this tomorrow with their distribution advantage, what's your defense?」
- **Trap**：创始人 handwave「they're too slow」
- **Answer**：Specific structural advantages (data network effect, specialized talent, timing, regulatory moat)

**Q11**：「Your competitor [X] raised [Y] 6 months ago. They have [Z] employees. Why do you win?」
- **Trap**：创始人 say "we're better"（太主观）
- **Answer**：Specific differentiation in 2-3 dimensions + evidence

**Q12**：「What's the best piece of evidence that your competitors are failing or will fail?」
- **Trap**：创始人没做 competitor intelligence
- **Answer**：Specific signals (review trends, churn customers' feedback, competitive wins, talent movements)

---

### Class 5：Team / Founder Kill Questions

**Q13**：「Tell me about a decision you made 12 months ago you now regret. What did you learn?」
- **Trap**：创始人 perfectionist trap——say "I don't have regrets"
- **Answer**：Specific, significant regret + concrete learning + how it changed behavior

**Q14**：「Your last founder you worked with — walk me through why that ended. Who called it? What's your relationship with them now?」
- **Trap**：模糊回答 = 可能有 toxic pattern
- **Answer**：clear story，own responsibility，relationship status

**Q15**：「Your co-founder — where do you two disagree? Tell me a real conflict, how you resolved it」
- **Trap**：创始人 say "we never disagree"（假的，或 dysfunctional）
- **Answer**：Real conflict + resolution process + what you learned about working together

---

### Class 6：Strategy / Execution Kill Questions

**Q16**：「What are the 3 things that would have to go right for you to hit your 5-year plan? Rank them by risk」
- **Trap**：创始人 only list things they control
- **Answer**：Include external dependencies (market timing, regulatory, partner behaviors)

**Q17**：「If I gave you $50M today instead of the $10M you're asking — what would you do with the extra $40M?」
- **Trap**：创始人 struggle to answer (意味着他们 asking amount wrong)
- **Answer**：Specific playbook for bigger check + why not asking for it now

**Q18**：「If I gave you $2M today instead of the $10M you're asking — what would change?」
- **Trap**：创始人 say "we wouldn't hit milestones"（implies 10M is just-right，no flexibility）
- **Answer**：Show how plan adapts to smaller check + what milestones shift

---

### Class 7：Financials / Fraud Kill Questions

**Q19**：「Your revenue recognition policy — walk me through. Do you book multi-year deals upfront or ratably?」
- **Trap**：创始人 loose with revenue recognition 可能 inflated ARR
- **Answer**：Clear policy aligned with GAAP (or equivalent) + applied consistently

**Q20**：「What percentage of your ARR is from customers with concentration risk? Top 3 customers = % of ARR」
- **Trap**：高 concentration = fragile
- **Answer**：Transparent + 如果有，show diversification plan

**Q21**：「Your burn rate — monthly? Walk me through the gross vs net burn. What's your runway without revenue growth?」
- **Trap**：创始人 optimistic about revenue offset
- **Answer**：Conservative: net burn with current revenue, no growth assumption, clear runway months

---

### Class 8：Existential Kill Questions

**Q22**：「In the worst-case scenario where this doesn't work — how does it fail? What's the most likely failure mode?」
- **Trap**：创始人 refuse 谈 failure (signals overconfidence)
- **Answer**：Specific failure modes + monitored signals + pivot triggers

**Q23**：「If you had to shut down tomorrow, what do you think your investors would say about you 5 years later?」
- **Trap**：Pass the test of "would they back me again"
- **Answer**：Honest self-assessment + relationship-building practice

**Q24**：「Why are you doing this? What's the personal reason you'd keep going when every rational person would quit?」
- **Trap**：创始人 give PR answer (signals lack of real motivation)
- **Answer**：Personal narrative that is emotionally real, not performative

---

## Reference Call 脚本（VC 会问 reference 什么）

创始人需要 **prime** reference，让他们有 meaningful answers。

### VC 给前员工打电话

**VC 的典型问题**：
1. 「Tell me about working with [founder]. What was great? What was hard?」
2. 「If you had to point out the founder's weakness / blind spot, what would it be?」
3. 「Why did you leave? Honestly.」
4. 「Would you work for this founder again? Why / why not?」
5. 「What's the craziest thing you saw the founder do during difficult times?」

**你如何 prime 前员工**（不是 coach them, 是 give context）：
- 告知 raising，important to founder career
- Ask "can I list you as reference"
- Not "please say nice things" — but "be honest, I can take it"

### VC 给 customer 打电话

**VC 的典型问题**：
1. 「How did you find [company]?」
2. 「What was the purchase decision process? Who was involved?」
3. 「What are the 2-3 things that make this product indispensable to you?」
4. 「When have you been frustrated? How did they respond?」
5. 「If [company] went away tomorrow, what would you do? Go back to [old solution] or find alternative?」
6. 「What competitors did you evaluate?」

**创始人准备**：
- Select references strategically — mix of enthusiastic + pragmatic + critical (critical but fair)
- Pre-call customers to say "VC may reach out, it's OK to share your honest experience"
- Prepare a backup list (if first list doesn't respond)

### VC 给 industry expert 打电话

**VC 的典型问题**：
1. 「Given this thesis, who are the top 3-5 companies we should look at?」
2. 「[This founder] — what's your take? Have you heard of them?」
3. 「What's the most contrarian thing someone could do in this space?」
4. 「Who's going to win this market in 5 years?」
5. 「What are the technical / market / regulatory risks we should worry about?」

**创始人影响**：
- Industry experts should know you (positive signal if they've heard of you)
- If they're key influencers, get an intro to them before fundraising
- Proactively engage experts in thought leadership (podcasts, conferences, research) — becomes reference by default

---

## Data Room 结构 —— VC 期望看什么

**Tier 1：必须完美 (VC first look)**
- Cap table（过去 + 当前 + 融后）
- Pitch deck 最新版
- Financial statements (past + forecast)
- Unit economics breakdown
- Customer / revenue breakdown

**Tier 2：TS 签后 visible**
- Employee agreements + IP assignments
- Customer contracts（redacted top 10）
- Vendor contracts
- Cofounder agreement / equity agreements
- Board materials from past meetings

**Tier 3：Pre-close deep dive**
- Detailed product roadmap
- Security / privacy audits
- Insurance policies
- Past investor communications
- Tax filings (for older companies)

---

## Red Flag Detection — VC 会 flag 的 10 个信号

### Red Flag 1：Revenue concentration
- Top 1 customer > 30% ARR
- Top 3 customer > 50% ARR
- **How to mitigate**：Show diversification pipeline + long-term contracts

### Red Flag 2：Churn pattern
- Churn rate > 25% annually (SaaS)
- Churn concentrated in one segment (shows PMF problem)
- Churn accelerating, not decelerating
- **How to mitigate**：Explain churn composition + recovery plan + new cohort improvement

### Red Flag 3：Founder team dynamics
- Cofounder already left
- Equity imbalance (one founder >> other)
- Unresolved founder disputes
- **How to mitigate**：Clean, fair equity structure + healthy dynamics + documented agreements

### Red Flag 4：IP / Legal issues
- IP disputes or unclear ownership
- Pending litigation
- Regulatory investigations
- **How to mitigate**：Clean IP assignments + proactive legal audit + transparent disclosure

### Red Flag 5：Financial irregularities
- Cash / revenue mismatch
- Related party transactions
- Inconsistent accounting policies
- **How to mitigate**：Clean accounting + optional CFO/controller review + transparent disclosure

### Red Flag 6：Market timing concerns
- Industry in cyclical downturn
- Regulatory risks increasing
- Disruption from AI/new tech
- **How to mitigate**：Frame as opportunity + show specific positioning for changes

### Red Flag 7：Technical debt
- Product built on legacy stack
- Performance / reliability issues
- Security concerns
- **How to mitigate**：Specific roadmap + hire plan + acknowledge trade-offs made

### Red Flag 8：Team gaps
- Missing key roles (CFO / VP Sales / VP Eng)
- Over-reliance on founders
- High turnover in senior roles
- **How to mitigate**：Specific hiring plan with timeline + references for planned roles

### Red Flag 9：Go-to-Market uncertainty
- Unclear primary channel
- Unsustainable CAC in primary channel
- Dependency on one marketing tactic
- **How to mitigate**：Multi-channel strategy + experiments + pipeline validation

### Red Flag 10：Founder behavioral signals
- Evasive answers
- Different story for different audiences
- Overly aggressive tone
- Unable to acknowledge weakness
- **How to mitigate**：Practice transparency + own mistakes + build trust slowly

---

## DD Execution — 4 Phase

### Phase A：Before DD Starts (TS signing day to Week 1)
**创始人行动**：
- Immediately prepare data room structure
- Pre-call potential references
- Schedule all required founder time for DD
- Clean up any loose ends (legal docs, cap table, etc.)

### Phase B：Week 1 — Structured Questions
- Return questions within 48 hours
- Triple-check all numbers
- Flag any issues proactively
- Request weekly sync with VC to maintain momentum

### Phase C：Week 2 — Reference / Calls
- Be transparent about references
- Don't over-prime (VC can tell)
- Offer tough references alongside enthusiastic ones
- Be available for follow-up

### Phase D：Week 3 — Closing Sprint
- Legal review in parallel
- Founder availability for deep dives
- Be prepared for any late-breaking questions
- Set clear expectations on closing timeline

---

## Post-DD Red Team Debrief

After DD, whether it closes or not, do a red team:

1. **What did VC focus on that I didn't prepare well for?**
2. **What signal was weakest in my DD?**
3. **What would I have changed in my pitch based on DD questions?**
4. **What references / materials should I upgrade for next raise?**

**File output**：`dd-debrief-[vc-name]-[date].md`

---

## 执行指令（给 LLM 代理）

**使用此 skill 的 prompt 模板**：

```
我是 [公司 X]，准备进入 VC 的 DD 阶段。帮我：

1. 基于我的业务类型 [B2B SaaS / AI / ...]，预测 VC 最可能 probe 的 8 个刁钻问题（从 24 题库中选 + 定制）
2. 给我 3 组 reference call 脚本（前员工 / customer / industry expert），我需要 prime 什么
3. 根据我的情况，识别最可能的 3 个 red flag，给我 mitigation 策略
4. 给我一个 3-week DD timeline，具体每天应该做什么
5. 如果我 DD 可能 fail，最可能的 failure mode 是什么，如何 pre-mortem

关键信息：
- 业务：[describe]
- 关键 metrics：[share]
- 已签 TS：[VC name, terms]
- 特殊情况：[any issues that may surface in DD]
```

---

## 与其他 skills 的协作

- **前置**：`vc-pitch-killtest`（已经 kill test 过 idea）、`founder-fundraising-wargame`（已经 understand 博弈）
- **并行**：`term-sheet-negotiator`（DD 期间同时在 negotiate TS）
- **后置**：`board-dynamics-wargame`（DD 通过 close 之后 board 管理）

---

## 校准锚点 (V1.0)

本 skill 的设计假设：
- **2026 年 VC 行为**：更严格 DD（post-FTX/Theranos），Tier-1 VC DD period 3-4 周，Tier-2/3 更短
- **DD Fail Rate**：TS 签后 20-40% fail during DD
- **Red Flags 严格度**：2023+ LP 压力下 VC 对 red flags 更 unforgiving

---

## changelog

- v1.0 2026-04-17：首版。提出「DD = kill test，不是 formality」核心认知、3-week timeline 解构、24 个刁钻问题（分 8 类）、3 组 reference call 脚本、10 个 red flag 识别 + 缓解、4 阶段 DD 执行流程、执行指令。与姊妹 skill 差异化定位。卫星文件 `dd-casebook.md` 待后续完成。
