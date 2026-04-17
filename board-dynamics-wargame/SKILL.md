---
name: Board Dynamics Wargame
description: CEO 被罢免的 Boardroom 博弈推演引擎。不是讲「怎么开好 board meeting」，而是「VC + 独董如何联合 fire 你」「CEO coup 如何预防」「产品战略分歧如何不变成 personnel 分歧」。含 10 个经典 CEO 罢免 / board 政变案例 + 5 种 faction 动态 + 12 种 boardroom move。
version: v1.0
created: 2026-04-17
---

# Board Dynamics Wargame — CEO 去留的博弈推演

> **核心命题**：Series A 之后，创始人是否能保住 CEO 位置，取决于 board 政治，不取决于业绩。Travis Kalanick 的 Uber 在他被 fire 时 valuation 是 $70B，Sam Altman 在 2023/11 被 fire 时 OpenAI 是全球最重要 AI 公司。**业绩不是护身符**。

**定位**：
- `founder-fundraising-wargame` = 融资阶段博弈（pre-close）
- `term-sheet-negotiator` = 条款博弈（TS 阶段）
- `vc-due-diligence-simulator` = DD 博弈（TS 到 close）
- **`board-dynamics-wargame`** = 融后董事会博弈（post-close，ongoing）

**卫星文件**：
- `board-coup-casebook.md`：10 个 CEO 罢免案例深度拆解 + 5 个 CEO 守位成功案例

---

## Part 1：董事会的 faction 结构

### 5 类 board member

| 类型 | 行为模式 | 在 coup 中的角色 |
|------|---------|--------------|
| **Founder（you）** | 产品/愿景驱动，emotional stake | 核心被 target |
| **VC Preferred**（Lead VC） | Fund return 驱动 | 最可能主导 coup 或 veto 你 |
| **VC Preferred**（Follow-on VC） | 跟随 lead VC | Swing vote，可 swing either way |
| **Founder-chosen Independent** | 你选的 advisor，通常忠诚 | Your 核心支持者 |
| **VC-chosen or Negotiated Independent** | VC network，通常偏 VC | VC 的核心支持者 |

### Typical board 演进

**Seed 阶段**：1-2 founder only (ideal) 或 1 founder + 1 VC observer
**Series A**：2 founder + 1 VC + 1 independent (5 seats total)
**Series B**：2 founder + 2 VC + 1 independent (5 seats total)
**Series C+**：2-3 founder + 3-4 VC + 2-3 independent (7-9 seats total)

### 关键数学

**创始人被 fire 的数学条件**：
- 5-person board：VC + 1 independent vs founder + 1 ally = 2:2 tie → independent 决定胜负
- 7-person board：2 VC + 2 independent = 4 vs 3 founder-aligned

**结论**：**只要 board 不是 founder majority，你 always 在 risk 区**。

---

## Part 2：12 种 Boardroom Move

### Move 1：Quiet Polling
VC 在 board meeting **之前** 单独 call 每个 independent + other VC，试探意见。如果发现 majority 支持 fire CEO，才在 meeting 提议。

**你的 counter**：你自己 quiet poll。任何 board meeting 之前，知道每个 member 的 position。

### Move 2：CEO Succession Sub-committee
VC 提议成立 "CEO succession planning committee"（看起来是 governance best practice）。这是 coup preparation，目的是 formalize 谁接替 CEO 的讨论。

**你的 counter**：proactively 提议 succession planning（从位置主导），或者要求 founder participation in committee。

### Move 3：Independent 任命
VC 推动 board 加 "independent director"，提供 "industry expertise"。实际是 VC 网络的 loyalist。

**你的 counter**：**Approval right on independent directors** 是 TS 时必须争取的。没有这个的话，永远在 risk。

### Move 4：Information Asymmetry Attack
VC 要求额外的 monthly CEO metrics + direct access to team（超出 standard info rights）。这是 building own intel channel，绕过 CEO。

**你的 counter**：所有 team communication 必须 through CEO 或 CEO-approved channel。Info right 不是 "inspect whenever"。

### Move 5：Back-channel to Key Employee
VC 直接 call 你的 CTO / CFO / VP Sales，了解 "real situation"。这是 building employee loyalty outside CEO。

**你的 counter**：在 closing TS 时就 set expectation 「all board/employee interactions go through me」。如果 VC 违反，这是严重信号。

### Move 6：Portfolio Founder Referrals
VC 让其他 portfolio company founder "meet" 你，实际是评估是否是 CEO material。这是 secret assessment。

**你的 counter**：任何 founder intro 要求 context（why are we meeting?）。Proactively propose your own peer groups.

### Move 7：Performance Framing
VC 在 board meeting 重新 frame 过去 12 月的执行——把 "original plan" 改为更严厉的 KPI，然后 claim CEO "missed goals"。

**你的 counter**：每个 board meeting start with a recap of **agreed** goals (get them in minutes). 不要让 goalpost 被后移。

### Move 8："Consultant" Engagement
VC 提议请 "management consultant" 评估 org effectiveness。Consultant 通常 report to VC 不是 founder，结论 predetermined。

**你的 counter**：Consultant 的 engagement letter 必须 require founder approval + report 必须 simultaneously go to founder and VC.

### Move 9：Financial Pressure Tactic
VC 在 budget 审批时 squeeze you——cut budget，force hard decisions，然后 blame "missed metrics" on CEO。

**你的 counter**：Budget approvals 必须 tied to agreed plan，不是 arbitrary 重新定义。每个 budget cut 的 rationale 必须 documented.

### Move 10：Pre-meeting Coalition Building
VC 在每个 board meeting 前 24-48 小时，和 other board members 有 "pre-meeting call"——实际是 alignment session。Founder 通常被 excluded。

**你的 counter**：Propose "All board members have pre-meeting 1-on-1 with CEO" as standard. Or at minimum, request inclusion in VC pre-meeting.

### Move 11：Confidential 1-on-1 with Independent
VC 和 independent director 有 "friendly dinner"，frame 为 board building。实际是 recruit independent 去 coup 阵营。

**你的 counter**：Proactively have your own dinners with independents. Build your relationship capital before VC does.

### Move 12：The Surprise Motion
Coup 的最后一步：在 board meeting 突然 propose "resolution to remove CEO and appoint interim CEO [name]"，before founder 能 prepare。

**你的 counter**：**Pre-meeting**，demand 所有 resolutions 24 小时 before meeting 发给所有 member. 如果 surprise motion 出现，你有 standing objection "improperly noticed"（依赖 company bylaws）.

---

## Part 3：Coup 的 Triggering Events（12 类）

### Category A：Performance-based triggers

**Trigger 1**：Missed 3+ major milestones 连续
**Trigger 2**：Revenue forecast miss > 30%
**Trigger 3**：Cash runway < 6 months unexpected
**Trigger 4**：Major customer churn concentration

### Category B：People-based triggers

**Trigger 5**：Cofounder departure（especially co-CEO）
**Trigger 6**：C-level turnover > 2 in 12 months
**Trigger 7**：Board complaint from 3+ employees (through VC channel)
**Trigger 8**：Pattern of "bad hire" decisions

### Category C：Governance/trust triggers

**Trigger 9**：Missed board disclosure (material info VC didn't know about)
**Trigger 10**：Related party transaction without approval
**Trigger 11**：Legal / regulatory issue not disclosed
**Trigger 12**：Founder personal issue affecting work (divorce, illness, substance)

---

## Part 4：Coup-Proofing 7-Layer Defense

### Layer 1：TS Level Defense
- Board composition：至少 odd number + founder 或 founder-chosen independent 多数
- Protective provisions 不覆盖 CEO hire/fire（keep this at board level，don't add preferred veto）
- **Dual-class stock**：如果可以，争取 super-voting on CEO election（controversial but effective）

### Layer 2：Relationship Defense
- 每个 board member 每月 1-on-1（30 minutes，formal）
- Every independent 每季度 informal dinner
- Quarterly "where are we heading" alignment discussion
- 知道每个 member 的 personal incentive (what makes their fund look good)

### Layer 3：Information Defense
- Weekly or bi-weekly CEO update email 给全 board
- Proactive flagging of 问题 (VC 发现 problem before you told them = huge trust loss)
- **Monthly KPI dashboard** standardized（保证你定义 the metrics, 不是他们后来重新 frame）

### Layer 4：Coalition Defense
- Relationship capital with **2 of 3 non-founder board members**
- Cultivate independent directors' loyalty through meaningful engagement
- If possible, have a non-VC institutional investor (like strategic corporate投资 or large angel) on board

### Layer 5：Governance Defense
- Enforce proper notice for board meetings + resolutions (24 小时 advance copy)
- Standing "CEO's agenda" 在每个 meeting（不让 VC 主导 agenda）
- Detailed board minutes (prevent revision history of "agreed goals")

### Layer 6：Performance Defense
- Over-communicate on execution (weekly metrics + monthly summary)
- Set conservative goals + systematically over-deliver
- **If you're going to miss**: pre-announce 4-6 weeks before, with mitigation plan

### Layer 7：Succession Defense
- Preemptively propose "CEO development framework"（get in front of it）
- Identify + groom 2 internal CEO candidates (gives board comfort that succession doesn't have to be external)
- **Counter-intuitive move**: make yourself "more replaceable" in operations → harder to fire you for being "indispensable"

---

## Part 5：Coup 发生的 Playbook

如果 coup 已经在进行（你 detect signals），步骤：

### Step 1：Detect (Month 0)
识别信号：
- VC 开始 "pre-meeting" calls
- Independent 变 distant
- VC 提议 new board member / committee
- Info request 变密集
- Key employee 被 directly reached out

### Step 2：Assess (Day 1-7)
- Quiet call 每个 board member: assess their position
- Talk to trusted advisors（lawyer + founder mentors）
- Determine if coup is truly happening or you're paranoid

### Step 3：Leverage (Day 7-14)
如果 coup is real，你的 leverage 是什么：
- **Financial**：是否有 cash runway? If crisis needs you to raise, you have leverage
- **Operational**：是否有 key customer relationships dependent on you? Key employees who would follow you out?
- **Strategic**：是否有 critical M&A or partnership in flight?
- **Legal**：founder 的 IP assignments 条款、employment rights

### Step 4：Negotiate (Day 14-30)
选择路径：

**Path A：Fight to stay**
- Line up support from your side (independent you have relationship with)
- Prepare "reconciliation" plan to address board concerns
- Request "cooling off" period

**Path B：Negotiate exit package**
- Accept you're out，negotiate：
  - Severance (6-12 months)
  - Accelerated vesting (100% preferred)
  - Consulting agreement (stay connected, potentially transition smoothly)
  - Non-compete relaxation
  - Stock / IPO / acquisition participation rights

**Path C：Nuclear option**
- Resign + take team + sue for contractual violations
- 只在 you have strong legal position + cash to fight + willing to go public

### Step 5：Execute (Day 30+)
- If fighting：board meeting prep, line up your votes
- If exiting：ensure contracts signed before announcement

---

## Part 6：Post-Coup Options

### Outcome 1：CEO stays
- 需要 rebuilding trust with VC
- Accept some concessions (more oversight, new hires)
- Document agreements in writing

### Outcome 2：CEO stays with reduced role
- "Executive Chairman" or "Chief Product Officer"
- 通常是 transitional (6-12 months)
- Signal is you're being "managed out gracefully"

### Outcome 3：CEO transitions out
- Negotiate exit package (see above)
- Retain board seat if possible (for founder perspective)
- Retain meaningful equity

### Outcome 4：Nuclear exit
- Legal battle with VC
- Public narrative war
- Often results in years of litigation

---

## Part 7：经典案例快速回顾（详见 board-coup-casebook.md）

| 案例 | 公司 | 年份 | CEO | Outcome |
|------|------|------|-----|---------|
| Sam Altman | OpenAI | 2023 | Fire → Reinstate (4 days) | Full recovery |
| Travis Kalanick | Uber | 2017 | Fire | Permanent exit |
| Steve Jobs | Apple | 1985 | Fire | Exile + Return |
| Steve Jobs | Apple | 1997 | Coup succeeded | Reinstated |
| Jack Dorsey | Twitter | 2008 | Fire | Returned 2015 |
| Parker Conrad | Zenefits | 2016 | Forced resign | Founded Rippling later |
| Adam Neumann | WeWork | 2019 | Forced resign | $1.7B severance |
| Bob Swan | Intel | 2021 | Replaced | Out |
| Kenneth Lin | Credit Karma | 2020 (acquisition) | Stayed | Full exit |
| Andy Rubin | Android | 2014 | Forced out | Founded Essential |

**Pattern**：
- Founder who are **visionaries but not operators** 最脆弱
- Founder who have **super-voting stock** 最 resilient
- **Timing** matters: growth phase 比 maturity phase 更容易 fire CEO

---

## Part 8：Red Flag / Yellow Flag Catalog

### Red Flags (Existential)
- VC 要求 CEO succession planning committee (and you're not leading)
- 3+ board members 有 "quiet 1-on-1s" excluding you
- Key employee 被 VC direct approach
- Board agenda 被 VC 主导
- Protective provisions 新增 CEO-related items

### Yellow Flags (Warning)
- VC 开始用 formal language in board meetings (less casual)
- Info requests 超出 standard
- Independent director becomes distant
- Founders being asked "succession plans" more frequently

### Green Flags (Healthy)
- Board debates issues openly
- Founder relationship with each board member has trust
- VC supports founder in tough decisions
- Independent directors bring expertise not politics

---

## 执行指令（给 LLM 代理）

**使用此 skill 的 prompt 模板**：

### Scenario A：Board 设计 (Pre-TS)
```
我在谈 Series A TS，VC 提议 board composition [describe]. 帮我：
1. 分析这个 composition 对 coup risk 的影响
2. 提出我应该 counter 的 TS 条款
3. 给我 independent director 选择的 criteria
```

### Scenario B：Ongoing Board 管理
```
我是 CEO，我的 board composition 是 [describe]. 最近感觉 [specific signal]. 帮我：
1. 识别这是 Red/Yellow/Green flag
2. 如果 coup is happening，assess my leverage
3. Propose 具体应对策略
```

### Scenario C：Coup 发生时
```
我 detected coup signals: [list them]. 帮我：
1. 评估 coup 是否 real (or paranoia)
2. 如果 real，我的 4 个 options (fight / negotiate / nuclear / exit) 的 pros/cons
3. Specific playbook for 下 30 days
```

---

## 与其他 skills 的协作

- **前置**：`term-sheet-negotiator`（board composition 在 TS 时 set）
- **前置**：`founder-fundraising-wargame`（理解融资 + board 整体）
- **并行**：`vc-due-diligence-simulator`（post-close 也需要 ongoing diligence on board）

---

## 校准锚点 (V1.0)

- **2023-2024 environment**：LP pressure on VC to show returns → more aggressive CEO replacement
- **Post-OpenAI drama**：Some VCs more cautious about coups (bad PR)
- **AI-native companies**：Founder concentration higher → dual-class and super-voting more common

---

## changelog

- v1.0 2026-04-17：首版。提出「5 类 board member + 12 种 boardroom move + 12 类 coup triggers + 7 层 coup-proofing defense + coup 发生时 playbook + 4 种 post-coup outcomes」。基于 OpenAI/Uber/Apple 经典案例。卫星文件 `board-coup-casebook.md` 待完成。
