---
name: Term Sheet Negotiator
description: 美式 term sheet 条款级博弈引擎。不是解释条款，是 **反打 VC 套路**——识别 VC 的 opening move、压力点、concessions 意愿，生成具体的反向 term sheet、让步顺序、trade-off stack。与 founder-fundraising-wargame 配对使用。
version: v1.0
created: 2026-04-17
---

# Term Sheet Negotiator — 条款级博弈引擎

> **姊妹 skill**：
> - `founder-fundraising-wargame/term-sheet-anatomy.md`：条款 **识别** 和 **红旗判断**
> - 本 skill：条款 **反打** 和 **谈判策略**
>
> **定位区别**：
> - term-sheet-anatomy = 字典（每条是什么）
> - term-sheet-negotiator = 兵法（怎么反打 VC 的套路）

---

## 核心方法论：三个博弈层

### Layer 1：Opening Move 识别
VC 给你 TS 时，**他们已经打了一个 opening move**。任何 TS 都不是 take-it-or-leave-it，是 negotiation anchor。你要识别：

1. **他们的 must-have**（非谈不可的核心 3-5 条）
2. **他们的 nice-to-have**（可以让步的 5-10 条）
3. **他们的 throwaway**（故意高开但准备让掉的 3-5 条）

### Layer 2：压力点计算
每条 TS 背后，VC 有一个 **LP committee 预期** 和 **portfolio pattern**。你要识别哪些条款如果让步，他们 **内部无法交差**，哪些 **内部已经让过很多次**。

### Layer 3：Trade-off Stack
谈判不是每条单独谈，是 **整体交换**。你要构建「让这 3 条换那 2 条」的 trade-off stack，让 VC 觉得自己赢了整体同时你拿到关键条款。

---

## 卫星文件索引

- `clause-casebook.md`：30+ 条款的详细反打套路（VC opening 话术 + 创始人反打话术 + 让步阶梯）
- （未来扩展）`negotiation-scenarios.md`：10+ 完整谈判场景从 TS 收到到签字
- （未来扩展）`red-team-patterns.md`：VC 常见的 red-team 套路（时间压力、打探底牌、fake competition）

**本主文件**：提供方法论框架 + 完整的谈判流程 + 关键决策模型。具体条款反打话术在 `clause-casebook.md`。

---

## Phase 1：Term Sheet 诊断（收到后 24 小时）

### Step 1.1：分类

把 TS 30+ 条款分 5 类：

| 类别 | 比例 | 处理 |
|------|------|------|
| **绿色条款**（完全 OK） | 50-60% | 接受，不谈 |
| **黄色条款**（偏差但可接受） | 20-30% | 储备，不主动攻，但准备 trade 掉 |
| **橙色条款**（明显不利） | 10-15% | 主攻，争取改到行业标准 |
| **红色条款**（严重红旗） | 3-5% | 死磕，接受即毒药 |
| **缺失条款**（应有未列） | 2-5% | 主动加入（如 founder protection） |

### Step 1.2：计算"真实估值"

VC 给你的 Pre-money 不是真实估值。真实估值 = Pre-money ÷ (1 + option pool adjustment) × (1 − 清算偏好 effective cost) × founder vesting 已 vested 比例 × ...

**简化公式**：

```
真实估值 = Headline Pre-money × Terms Quality Multiplier

Terms Quality Multiplier:
- 1x Non-Participating:         1.00
- 1x Participating:             0.85
- 1x Capped Participating:      0.92
- 2x Non-Participating:         0.80
- Full Ratchet Anti-Dilution:   × 0.85
- Pre-money option pool:        × 0.85-0.90
- Protective provisions 过宽:    × 0.95
- 50% Drag-Along threshold:     × 0.92
- Aggressive vesting reset:     × 0.90
```

**示例**：VC A 给 $30M pre + clean terms vs VC B 给 $40M pre + participating + pre-money option pool

- VC A 真实：$30M × 1.0 = $30M
- VC B 真实：$40M × 0.85 (participating) × 0.87 (pre-money pool) = $29.6M

**VC B 看起来高 33%，实际持平**。创始人必须会做这个数学。

### Step 1.3：识别 VC 的 pattern

搜索这个 VC 过去 12 月的 公开 TS（Crunchbase / AngelList / 创始人群组）：

- 他们一般给什么 Liquidation Preference？
- 他们 board seat 政策（seed 要不要 seat）？
- 他们 no-shop 常见长度？

**结果**：你现在知道你拿到的 TS 是 **比他们平均更好 / 持平 / 更差**。

### Step 1.4：识别 opening move 的 "tells"

VC 在 TS 里留了 tells 告诉你他们的 priority：

| Tell | 意味着 |
|------|--------|
| 写得特别长的条款 | 他们内部 push 过多次，是 priority |
| 用 「standard」形容某条 | 他们预期你不会谈 |
| 特定 clause 带 explanation | 他们知道这条 unusual，预期你会谈 |
| TS 最后加 legal fees clause | Throwaway，一定可以谈掉 |
| 特别早提到 board seat | 他们 really 要 |

---

## Phase 2：反向 Term Sheet 构建（收到后 48-72 小时）

### Step 2.1：决定你的 3 项 must-win

你不可能全部谈赢。选 3 条最关键：

**默认 3 项 must-win**：
1. **Post-money option pool**（vs pre-money）
2. **1x Non-Participating Liquidation Preference**（拒绝 Participating）
3. **Founder-friendly board structure**（至少 odd number with independent）

**根据你的具体情况调整**：
- 如果是 hot deal + 多 offer：加 **估值 match 到 #2**
- 如果是 B2B SaaS 且你想要快速 scale：加 **取消 aggressive milestones**
- 如果你有 co-founder 争议历史：加 **vesting acceleration clauses**

### Step 2.2：准备你的 trade-off stack

你需要「我让这个你让那个」的具体 trade 组合：

**Trade Stack A：「pro-rata for preference」**
- 让步：给 VC 更多 pro-rata rights（对 follow-on 有利）
- 换取：Liquidation preference 从 Participating 换到 Non-Participating

**Trade Stack B：「legal fees for option pool」**
- 让步：提高 legal fees cap $25K → $75K
- 换取：Option pool 从 pre-money 换到 post-money

**Trade Stack C：「drag-along for board」**
- 让步：Drag-along 从 75% 降到 66%
- 换取：Board 增加 1 个 founder-friendly independent seat

**Trade Stack D：「no-shop extension for valuation match」**
- 让步：No-shop 从 30 → 45 days
- 换取：Pre-money valuation 从 $40M → $45M

### Step 2.3：构建反向 TS（Markup）

**输出格式**：Track-changes 的 Word / 或干净的 revised TS

对每一条：
- 绿色条款：不改
- 黄色条款：不改，准备 trade
- 橙色条款：改到 market standard，并加 comment 解释为什么
- 红色条款：改到 founder-friendly，并标注「red line for founder」

**策略**：你的反向 TS 应该「收敛」—— 不是每条都 maximal demand，而是每条都 sensible + 关键条款 absolutely firm。这样 VC 看到会觉得「这个创始人懂 market，不是无理」。

---

## Phase 3：谈判执行（反向 TS 发送后 1-2 周）

### Step 3.1：Initial response

发送反向 TS 时，附一封 email：

```
Hi [VC Partner],

Thanks so much for the TS. Really excited about partnering with [Fund].

I've reviewed the TS carefully with my lawyer and some advisors. Attached
is our proposed markup. A few high-level comments:

1. Overall we're aligned on [main themes]. The core economics work for
   everyone.

2. Three areas we'd like to discuss:
   (a) [must-win #1] — [1 sentence rationale]
   (b) [must-win #2] — [1 sentence rationale]
   (c) [must-win #3] — [1 sentence rationale]

3. A few smaller items flagged in the markup that I'd love to talk through
   but not dealbreakers.

Happy to jump on a call this week — when works for you?

Best,
[Founder]
```

**关键**：
- 不 over-negotiate。标明 3 大件 + 小件。
- 语气 partnership，不 adversarial。
- 不 mention 其他 offer（如果有，别透底，只暗示）。

### Step 3.2：First call dynamics

VC 会 push back。准备好应答：

| VC 的 push-back | 你的应答 |
|---------------|---------|
| "We've done 50 deals with these exact terms"  | "I've seen your portfolio. [Specific example] had different terms. Every deal is negotiated to fit." |
| "Our LPs require this protection" | "I understand LP pressure. Here's a structure that achieves that protection via [alternative]. Does that work?" |
| "If we change this, we need to change the valuation" | "Let's not link these. Let's talk terms on their merits. If the valuation is the ultimate question, let's go there directly." |
| "This is how Series A works in 2026" | "Let me share 3 recent comparable deals with different terms. [Share data]." |
| "Other investors wouldn't give you this" | "If that's true, it'll come up in our other conversations. I'll let you know if it does." |

### Step 3.3：Ping-pong management

大部分 TS 经过 2-4 轮 iteration 完成：

**Round 1**：你的反向 TS → VC 的 counter
**Round 2**：你的 counter-counter，focus 3 大件
**Round 3**：VC 让步某条，你 hold 住 must-win
**Round 4**：收尾，small details

**节奏控制**：
- 每轮间隔 2-4 天（不要立即回，别让对方觉得你 anxious）
- 每轮推进 1-2 个条款（不是全部一次）
- 保持 momentum 但不 rushed

### Step 3.4：死磕点的处理

如果对方 hard no on 你的 must-win：

**策略 A：升级**
- 从 partner 升到 general partner 或 founding partner
- 说「我们 discuss 了很多但差 1-2 条，能一起谈一次吗」
- 升级的好处：founding partner 的决策权更大

**策略 B：Bring in external validation**
- 律师说「市场数据支持我方」
- 其他 VC 的 TS（即使你不 close，可以 share 给现 VC 作为 benchmark）
- 顾问（ex-VC 或 ex-founder）加入 call 支持你

**策略 C：表达愿意放弃**
- 「If we can't get to X, I think this isn't the right fit」
- 这是核弹，只在 must-win 且你有 alternative 时用

**策略 D：找 trade**
- 「I can give you Y if you give me X」
- 回到 Trade Stack

---

## Phase 4：关闭（最后 3-5 天）

### Step 4.1：最后一英里的常见陷阱

**陷阱 1：Legal drafting creep**
- 律师 drafting 正式 docs 时，偷偷加 TS 没有的 clause
- 防御：你必须自己读每一版 drafting，不要完全依赖律师

**陷阱 2：Side letter surprise**
- VC 要求额外 side letter 加 MFN 或其他
- 防御：任何 side letter 必须 TS-level visibility

**陷阱 3：Closing conditions 扩张**
- VC 加「pending reference checks」「pending final DD」等
- 防御：TS 签署后 DD 应该 minimal，任何新条件都是 red flag

**陷阱 4：Wire delay**
- TS 签完但 wire 延迟 2-4 周
- 这期间 VC 可以 walk away
- 防御：TS 里 lock 住 wire 时间 + 如果 delayed 的 remedy

### Step 4.2：Closing celebration 之前

- [ ] 所有 TS markup 都反映到 final docs？
- [ ] Side letters 都 review 过？
- [ ] Cap table after closing 算过，没意外？
- [ ] Board composition 启动确定？
- [ ] 下次 board meeting scheduled？
- [ ] Founder-investor alignment on 12-month plan 有 doc 记录？

### Step 4.3：Post-closing 的"90 天蜜月期"

Closing 后 90 天是 investor 对你 signal 最好的时期：
- 主动 update，不要等问
- 解决 board dynamics 和 info rights 节奏
- 建立「good company to back」的第一印象

**Post-closing 陷阱**：closing 后 3-6 月 miss 某个 milestone → investor signal 急速反转 → 下轮 raise 困难

---

## 关键决策模型

### Model 1：是否接受 TS

**决策树**：
```
收到 TS
├─ 估值 < 行业 bottom quartile?
│  ├─ Yes: walk away (unless desperate)
│  └─ No: continue
├─ 3+ 红旗条款 (Full Ratchet, 2x Participating, etc.)?
│  ├─ Yes: hard negotiate or walk
│  └─ No: continue
├─ Board composition 合理?
│  ├─ No (e.g., VC majority at seed): hard negotiate
│  └─ Yes: continue
├─ 创始人直觉是否 good partner?
│  ├─ No: walk (signal future fights)
│  └─ Yes: negotiate to close
```

### Model 2：多 offer 时的选择

不只看 valuation，还看：

| 维度 | 权重 | 评分 |
|------|------|------|
| 估值（Real valuation after terms adjust） | 25% | |
| VC tier / signal | 25% | |
| Partner fit / 可交流度 | 20% | |
| Portfolio synergy | 10% | |
| Board 能力（能 helpful 吗） | 10% | |
| Pro-rata for next round | 5% | |
| Terms cleanness | 5% | |

**Pitfall**：只看 valuation 的创始人常常后悔。VC tier + partner fit 的长期价值通常 > 10-20% valuation premium。

### Model 3：什么时候 walk

**Walk signals**：
- VC 拒绝提供 comparable portfolio 的 TS references
- VC partner 突然「need to check with MD」之前没说过
- 谈判过程 VC 在 4 周内变了 position 2 次以上
- VC 要求「exclusive data access」超出 reasonable DD
- VC 提到「cornerstone」或「board chair」权力 > partner level

---

## 执行指令（给 LLM 代理）

**使用此 skill 的 prompt 模板**：

```
我收到一份 TS，帮我：
1. 分类 30 条款到 绿/黄/橙/红/缺失 5 类
2. 计算真实估值（用 Terms Quality Multiplier）
3. 识别 VC 的 3 项 opening move + 3 项 throwaway
4. 提出我的 3 项 must-win 和 3 个 trade stack
5. 给我一份反向 TS（markup format）
6. 草拟第一次回复 email
7. 预测 VC 最可能的 push-back + 我的应答

TS 内容：[paste TS here]
行业背景：[AI/SaaS/Biotech/etc.]
我的 BATNA：[多少 offer / 竞争激烈度]
```

---

## 与其他 skills 的协作

- **前置**：`vc-pitch-killtest` 帮你确认 pitch 结构、`founder-fundraising-wargame` 帮你融资整体战略
- **并行**：`term-sheet-anatomy` 是本 skill 的 reference guide（条款字典）
- **后置**：`board-dynamics-wargame` (v1.0) 帮你 post-closing board 管理、`vc-due-diligence-simulator` (v1.0) 帮你应对 closing DD

---

## 校准锚点（V1.0）

本 skill 的设计假设：
- **2026 年市场**：Series A 估值 $20-60M pre，term 偏 founder-friendly 相比 2021-2022
- **一线 VC 标准**：1x Non-Participating, Broad-based WA, 66%+ Drag-Along
- **创始人杠杆**：如果有 2+ TS → 强杠杆；1 TS → 中杠杆；0 TS (inside only) → 弱杠杆

如果市场条件变化（如 2027+ bubble 或 2027- downturn），需要调整锚点。

---

## changelog

- v1.0 2026-04-17：首版。提出「三层博弈（Opening Move 识别 / 压力点计算 / Trade-off Stack）」方法论、4 阶段完整流程（诊断 / 构建 / 执行 / 关闭）、3 个关键决策模型、执行指令。与 `founder-fundraising-wargame/term-sheet-anatomy.md` 差异化（字典 vs 兵法）。卫星文件 `clause-casebook.md` 待后续完成。
