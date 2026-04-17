# DD Casebook — DD 失败与成功的案例拆解

> v1.0 首版。与主文件绑定使用。

**本文件的 10 个案例**：5 个 DD 失败导致 deal 崩掉的，5 个 DD 穿越惊险情况成功 closing 的。每个案例按「Context / DD Trigger / Red Flag / Founder Response / Outcome / Lessons」展开。

**案例来源**：抽取自 2018-2024 年美国创投圈典型模式（敏感细节模糊化）。

---

## 失败案例 1：SaaS Startup — "ARR 幽灵"

### Context
- Series A，$40M pre，raise $10M
- Pitch 声明 ARR $4M，growing 15% QoQ
- VC 签 TS，进入 3-week DD

### DD Trigger
- Week 1 Data Room：customer list 显示 ARR $4M 实际 = $3.2M ACV + $800K booked but not yet invoiced
- Week 1 unit economics：VC 的 analyst 重算 LTV/CAC → LTV 比创始人声明低 40%（不同 retention 假设）
- Week 2 customer calls：3 个 "top customer" 实际上 month-to-month（不是 annual 合同）

### Red Flag
- **Revenue recognition inconsistency**：founder 把 sales commitment 计入 ARR，实际会计里不是
- **Retention assumption aggressive**：用了 peak cohort 的 retention 外推到全公司
- **Customer stickiness exaggerated**：month-to-month 被 pitch 成 "annual"

### Founder Response
- Week 1 end：VC 提问 revenue recognition，founder defensive → signal 变差
- Week 2：founder 尝试 "recharacterize" 数据 → 进一步 lose credibility
- Week 2 end：VC 内部 partners 讨论，开始 lean 对 walk

### Outcome
- Week 3：VC 口头 "need to revisit valuation + terms"
- 一周后：VC 提出 revised terms，pre-money 从 $40M → $25M + 2x Participating
- Founder 无法接受，TS 终止
- Founder 花 3 个月重新 raise，最终 $28M pre + clean terms from another VC

### Lessons
- **Revenue recognition honesty is existential**：inflate ARR 的 short-term benefit 远远不及 DD 曝光的 long-term cost
- **Don't use peak cohort metrics to extrapolate**：VC 的 analyst 会重算，用 blended cohorts
- **Month-to-month customers 不是 "ARR"**：至少要 clarify, 不要 present as annual
- **Defensive response in DD = death signal**：要么 acknowledge 问题并 move on，要么 walk away from the deal

---

## 失败案例 2：AI Startup — "Demo 与现实的 Gap"

### Context
- Seed+，$25M pre，raise $8M
- Product demo 惊艳，"AI agent that replaces entry-level analyst"
- VC 签 TS，TS signing 当天 founder demo 了 2 小时

### DD Trigger
- Week 1 Technical review：VC 带来 AI advisor（senior engineer at major AI lab）问架构
- Advisor 发现：demo 用了 GPT-4 + 3 个 prompt engineering layer，没有 proprietary model training
- Advisor 的 assessment：「这个团队是 prompt engineering team, not AI team. Any well-funded competitor can replicate in 3 months」
- Week 2：VC 找 2 个 "customer" do reference call → 发现 customer 只是 paid pilot，month-to-month，没签 commercial contract

### Red Flag
- **Technical moat 不存在**：wrap existing foundation model 不是 moat
- **"Customers" 是 pilot 不是 revenue**：no commitment beyond trial
- **Founder 不懂 technical depth**：被 AI advisor 问深了就 handwave

### Founder Response
- 试图说 "we have proprietary data + fine-tuning pipeline" → advisor 要看 code/architecture → no real system existed
- 试图说 "pilots will convert to revenue" → 没有 pipeline evidence
- Week 2 mid：VC 开始 ghost（不回邮件）
- Week 3：VC 发"after IC discussion, we're unable to proceed" email

### Outcome
- TS 撤销
- Founder 公开说 "market conditions changed" → 其他 VC 听到后 ghost
- 6 个月后融资失败，公司 wind down

### Lessons
- **AI moat 必须是 real**：wrap foundation model 不是 defensible
- **Pilot ≠ revenue**：不要混为一谈
- **Technical founders 必须能 defend 技术 depth**：找不到 technical cofounder 就不要 pitch AI
- **"Market conditions changed" 是 VC 圈的 scarlet letter**：听到就 know deal fell apart

---

## 失败案例 3：Consumer Startup — "创始人 Reference 灾难"

### Context
- Series A，$60M pre，raise $15M
- Founder 是 well-known serial entrepreneur，previous exit
- VC 签 TS，被 founder reputation 吸引

### DD Trigger
- Week 2 Reference calls：VC 找 founder 的 previous startup 的 2 个 cofounders call
- Cofounder 1：founder 是 "great at fundraising, bad at team management"
- Cofounder 2：founder 在 previous company 的 exit，actually forced to step down before acquisition
- VC 的 back-channel call：former employee 说 founder 有 aggressive firing pattern + "burned bridges"

### Red Flag
- **Previous exit narrative 不完全真实**：was forced out
- **Team management pattern**：history of high turnover, burnt bridges
- **Blind spot**：founder 不认识这是 pattern, defensive when asked

### Founder Response
- Week 2：VC 谨慎问 previous company 的 dynamics → founder 给 PR 答案
- Week 2 end：VC 再问 specific 前员工 reference → founder 给了 3 个，但 2 个 didn't respond (unusual)
- Week 3：VC 开始做 random back-channel calls to founder's network

### Outcome
- Week 3 mid：VC 通知 need more time for DD (bad signal)
- Week 4：VC decline，cite "team dynamics concerns"
- Founder 后续告 VC 其他 portfolio founder 帮 "validate"，但 damage done
- 6 个月后另一 VC 签 TS，同样 DD 问题，同样 fail
- 一年后 founder 最终 raise $8M at $25M pre (from smaller VC)，$35M down from original target

### Lessons
- **Reputation compounds**：past behavior 是 future pattern，VC 会挖
- **Back-channel calls 是 wild card**：你无法控制，所以不要给 VC 任何 reason to dig
- **Defensive answers 永远是 bad signal**：be honest about past imperfections
- **Cofounder departure 的 narrative 是 scrutinized**：若你 previous company 有 messy exit，不要 present 得 clean

---

## 失败案例 4：B2B SaaS — "Cap Table Nightmare"

### Context
- Series B，$150M pre，raise $30M
- Growth metrics solid，product-market fit clear
- VC 签 TS，准备 close

### DD Trigger
- Week 1 Legal review：cap table 显示 3 个 early angel investors 的 ROFR 未 formally waived in previous rounds
- Week 2：其中 1 个 angel 在 current round 要求 exercise ROFR + participate pro-rata
- Week 2 end：angel 要求的 amount 让 VC 的 Series B 份额从 $30M → $22M
- Week 3：第二个 angel 跟进，同样要求 pro-rata

### Red Flag
- **Historical cap table governance 有漏洞**：早期 angels 的 rights 没 properly managed
- **Rights stacking**：多轮 ROFR + pro-rata 累积
- **Communication failure**：founder 没提前和 angels 协调

### Founder Response
- Week 2：尝试 negotiate with angels individually → 失败 (angels 有 leverage)
- Week 2 end：提议 VC "let's proceed with smaller check" → VC 不愿意 (fund math doesn't work)
- Week 3：提议 "maybe re-price or re-structure" → VC considers walking

### Outcome
- Week 4：VC 提议 pre-money bump + longer DD + new term → founder 觉得过分
- Week 5：deal 结构变成 TS revised multiple times
- 最终 close，但 pre-money 从 $150M → $120M，6 week delay
- Founder 额外花 $500K legal fees in process

### Lessons
- **Cap table hygiene is critical**：每轮融资都要 properly 管理 ROFR/pro-rata waivers
- **Communicate with early stakeholders before TS**：不要等他们 surprise you
- **"Stacking rights" 会累积成 disaster**：每个 small right 独立看是 OK，stacked 起来是 showstopper
- **Legal hygiene 不是 bureaucratic，是 existential**：每轮都要 right

---

## 失败案例 5：FinTech Startup — "Regulatory 地雷"

### Context
- Series A，$50M pre，raise $12M
- Fintech 公司，regulated industry
- VC 签 TS，regulatory compliance 是 known risk 但 accepted

### DD Trigger
- Week 1 Legal review：VC 的 regulatory counsel 深度审查
- Week 2：发现 company 过去 12 月运营时，一个 key state 的 money transmitter license 还在 pending，已经处理 $50M transactions
- Week 2 mid：counsel 估算 potential liability $2-5M + possible cease & desist order
- Week 3：VC 内部 assess，说 "this is a material issue we can't price around"

### Red Flag
- **Unauthorized operations**：在 regulated activity without proper license
- **Liability exposure**：potential significant fines
- **Ongoing risk**：即使 close，regulatory overhang 影响 next round

### Founder Response
- Week 2：承认 issue，但 frame 为 "industry standard practice"
- Week 2 end：提供 legal memo 说 "not material"
- VC 的 counsel 不 buy it, 估算 exposure 仍然 $2-5M
- Week 3：founder 试图 "fix" by rushing license filings → 太晚

### Outcome
- TS 撤销
- VC 的 concern 传遍圈，其他 VC 都 pause
- Founder 花 6 个月 fix license + pay fines
- 一年后 raise Series A，but at $30M pre ($20M lower) + VC 加 extensive compliance covenants

### Lessons
- **Regulated industries require clean compliance before fundraising**：不要带 skeleton
- **"Industry standard 不等于 legal"**：fintech 圈常见 practice 可能 unlicensed，不代表可以
- **Don't try to fix last-minute**：DD 时发现只会 make it worse
- **Regulatory overhang 的 dilution cost > license 成本**：proactive compliance is cheap

---

## 成功案例 1：HealthTech — "透明度赢得 Trust"

### Context
- Series A，$35M pre，raise $10M
- Healthcare 产品，FDA 审批中
- VC 签 TS，FDA risk 是 known

### DD Challenge
- Week 1 Data Room：founder 提供了 **transparent FDA communications**，包括 negative feedback from recent submission
- Week 2 Expert calls：VC 找 2 个 FDA regulatory experts 评估
- Expert 1 说：审批 delays likely 6 months extra
- Expert 2 说：there's a 15% chance of outright denial

### Founder Response
- **Proactive disclosure**：在 Week 1 就 flag 这些 risks in context
- **Alternative path**：提供了 510(k) path analysis + 另外 2 个 regulatory pathways
- **Financial stress test**：show runway with worst-case FDA delay
- **Response to expert feedback**：approach each concern with specific mitigation plan

### Outcome
- Week 3：VC IC 讨论，decision = proceed but with milestone structure
- Final terms：original $35M pre preserved, but $10M check split into $5M at close + $5M upon positive FDA milestone
- Close happened Week 4，2 weeks later than original plan

### Lessons
- **Transparency builds trust**：不要 hide risks，present 他们 with mitigation
- **Multiple path planning**：show that you have plan B + C，not just plan A
- **Accepting milestone structure in exchange for valuation preservation**：smart trade
- **Expert opinion should reinforce, not undermine**：找到好的 regulatory narrative

---

## 成功案例 2：Deep Tech — "Technical DD Mastery"

### Context
- Series Seed，$15M pre，raise $5M
- Quantum computing startup
- VC 签 TS，但 technical DD 是 make-or-break

### DD Challenge
- Week 2 Technical review：VC 带来 3 个 quantum computing experts
- 每个 expert 都有自己的 framework 评估 technology
- Expert 1 focus on error correction approach
- Expert 2 focus on scaling challenges
- Expert 3 focus on competitive landscape

### Founder Response
- **Founder + CTO 都参加**：分工回答 technical vs strategic 问题
- **Prepared response to 30+ technical questions ahead of time**
- **Proactive demo**：not just slides, 让 expert 实际 interact with system
- **Honest uncertainty**：acknowledge "we don't know yet" for 3 specific technical questions, frame as research agenda

### Outcome
- Week 3：VC IC 有分歧 (2 of 3 partners)
- Champion partner brought experts' written assessment as evidence
- Close happened Week 4，按 original terms
- Expert reviews 实际上 later 被 VC 用来 sell deal to follow-on investors

### Lessons
- **Technical depth can be demonstrated in DD if preparation is right**
- **Admitting what you don't know is actually credibility-building**
- **Involve technical team, not just founder**：VC 要看 team depth
- **Proactive demo trumps slides**：experts want to see, not hear

---

## 成功案例 3：Marketplace — "Customer 洪水"

### Context
- Series A，$45M pre，raise $12M
- Consumer marketplace
- VC 签 TS，customer retention 是 key question

### DD Challenge
- Week 1 metrics request：VC 要 cohort data
- Week 2 customer calls：VC 想 call 20+ customers
- VC 的 分析师计算 reveal: customer LTV 其实依赖 repeat behavior，只有 60% customers are repeat

### Founder Response
- **Provide extra cohort data**：除了 VC 要的，additional cut (monthly cohort + segment by behavior)
- **Offer 50+ customer references**（超过 VC 要求的 20）
- **Preemptively flag**："40% of customers are one-time, here's why and here's the plan"
- **Unit economics transparency**：show CAC/LTV with and without repeat behavior assumption

### Outcome
- Week 2 end：VC analyst built independent model，匹配 founder 的数据
- Week 3：VC focus 在 "plan to convert one-timers"，founder 已有详细 plan
- Close happened on schedule，original terms

### Lessons
- **Over-deliver on DD material**：VC 感觉 "this founder has nothing to hide"
- **Preemptive framing of weaknesses**：show you understand the issue
- **Customer abundance**：让 VC 有 flexibility 在谁 call
- **Independent analyst validation**：让 VC 自己算 → 得到相同结果 → trust builds

---

## 成功案例 4：SaaS Pivot Story — "Honest Reset"

### Context
- Series A，$20M pre，raise $6M
- Company 原本 B2C SaaS，过去 12 月 pivot 到 B2B
- VC 签 TS，pivot story 是 core narrative

### DD Challenge
- Week 1：VC 发现 B2C 产品 12 个月前有 $1M ARR，now $400K
- Week 2 customer calls：前 B2C customers 讲 negative experience（pivot 让他们 feel abandoned）
- Week 2：新 B2B customers 只有 6 months data，very early

### Founder Response
- **Preemptive narrative**：TS signing 前就 framed pivot as "decisive strategic move"
- **Acknowledge B2C wind-down impact**："we chose to lose this revenue to focus on what will scale"
- **Provide detailed pivot rationale**：why B2B is bigger, why we're positioned, why now
- **Share learning from B2C mistakes**：don't hide them, use as evidence of sophistication

### Outcome
- Week 3：VC 的 IC 有 debate ("is this a failed B2C or successful B2B?")
- Champion partner 说 "the narrative is honest and the pivot logic is sound"
- Close happened week 4，terms slightly adjusted (raise $5M instead of $6M, reserve for extension)

### Lessons
- **Pivot story must be confident, not apologetic**
- **Acknowledge past mistakes as evidence of current wisdom**
- **Separate past economics from current**: don't blend old B2C metrics with new B2B
- **Accept some adjustment**：$5M vs $6M is reasonable for pivot risk

---

## 成功案例 5：Enterprise SaaS — "Reference Tsunami"

### Context
- Series B，$100M pre，raise $25M
- Enterprise SaaS with Fortune 500 customers
- VC 签 TS，enterprise sales motion 是 key thesis

### DD Challenge
- Week 2：VC 想 call 10 enterprise customers
- Founder 提供 15 customers, 说 "call anyone you want"
- 1 of the customers 实际上在 churn consideration (not yet decided)

### Founder Response
- **Proactive communication with "at-risk" customer**：told customer "VC might call, here's context"
- **Pre-call customer to understand their specific concerns**
- **Gave customer permission to be honest about concerns**
- **Simultaneously developed and shared concrete plan to address their concerns**

### Outcome
- Week 2 end：VC called at-risk customer
- Customer shared concerns but also said "they've been addressing, I'm still engaged"
- VC 实际上 impressed by founder's handling
- Week 3：close happened按 original terms

### Lessons
- **Never hide customer concerns，work with them**
- **Give customers permission to be honest**
- **Simultaneously develop mitigation plan，not after concerns raised**
- **Turn potential red flag into evidence of strong customer relationships**

---

## 通用 DD 模式总结

### Pattern 1：Transparency Multiplies Trust
- 每个成功案例都涉及 proactive disclosure
- 每个失败案例都涉及 defensive posture
- 关键：不是 "no issues"，是 "we know about issues, here's our plan"

### Pattern 2：Prepare Ahead of Time
- DD 开始才 scramble = death
- DD 开始前就有 data room + references ready = survival
- 创始人应该 continuously run "internal DD" on themselves

### Pattern 3：Reference Strategy Matters
- 不要只给 enthusiastic references
- Include tough but fair references
- Pre-brief references (give context, not script)

### Pattern 4：Technical Depth Requires Founder Capability
- Founder 必须能 independently defend technical claims
- If you can't, hire CTO before fundraising

### Pattern 5：Legal Hygiene Is Existential
- 每轮融资都 properly 管理 cap table
- 不要 accumulate "small issues" that stack into big problems

### Pattern 6：Regulatory 和 Compliance 不能 shortcut
- Regulated industries need clean compliance before fundraising
- Don't rely on "industry standard" if not explicitly legal

---

## 创始人 DD 预演 Template

每个创始人在 TS 签前应该 run this template：

**Section 1：数据一致性**
- [ ] ARR 和 revenue recognition policy 完全一致？
- [ ] Unit economics 经得起 "fully-loaded" 重算？
- [ ] Cohort retention data 是否 blended (non-cherry-picked)?

**Section 2：团队 reference**
- [ ] 3-5 前员工愿意 give honest reference?
- [ ] 3-5 customer 愿意 give enthusiastic reference?
- [ ] 2-3 industry expert 愿意 validate thesis?
- [ ] Back-channel 潜在 risk 清单（什么 random calls VC 会做？）

**Section 3：技术 defensibility**
- [ ] Founder + CTO 能 defend 技术 architecture?
- [ ] Technical moat 经得起 expert review?
- [ ] Competitor analysis 是 honest？

**Section 4：Legal 清洁**
- [ ] Cap table 所有 previous rights 已 waived?
- [ ] IP assignment 清晰？
- [ ] 没有 pending litigation?
- [ ] Regulatory compliance clean?

**Section 5：Financial 透明**
- [ ] Burn rate 正确报告？
- [ ] Revenue concentration risk 清楚？
- [ ] Churn pattern 理解 + 可 explain?

---

## changelog

- v1.0 2026-04-17：首版。提供 10 个 DD 案例（5 失败 + 5 成功），总结 6 个通用模式，提供创始人 DD 预演 template。配合主文件的 24 问题和 Reference Call 脚本使用。
