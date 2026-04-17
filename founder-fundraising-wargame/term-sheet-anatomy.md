# Term Sheet Anatomy — 美式 TS 逐条拆解

> v2.0 新增。与主文件 Phase 3e 绑定使用。
> 条款深度谈判 → 使用姊妹 skill `term-sheet-negotiator`（带条款博弈 + 反打话术）。

**本文件目的**：对美式 term sheet 的每一条做「看起来是什么 / 实际意味着什么 / 陷阱在哪 / 正常值 / 红旗值」的四列展开。创始人拿到 TS 后逐条比对。

**免责声明**：以下是博弈论分析，不是法律意见。任何 TS 都应找律师审。

---

## TS 的结构（以 NVCA model 为基准）

美式 TS 通常 4-8 页，分为 4 大块：

1. **Economics** — 钱相关：估值、支票、股权、期权池、清算优先权、反稀释
2. **Control** — 权力相关：董事会、protective provisions、information rights、drag-along
3. **Founder-specific** — 创始人相关：vesting、founder restrictions、transfer restrictions
4. **Mechanics & Miscellaneous** — 流程：closing conditions、no-shop、legal fees

Binding vs non-binding：大部分条款不 binding（意向书性质），但 no-shop、confidentiality、expenses reimbursement 通常 binding。

---

## Part 1：Economics（钱）

### 1.1 Valuation（估值）

```
Pre-Money Valuation: $[X]M
Amount Raised: $[Y]M
Post-Money Valuation: $[X+Y]M
VC Ownership: [Y / (X+Y)]%
```

| 维度 | 看起来是什么 | 实际意味着什么 | 陷阱在哪 |
|------|-----------|--------------|---------|
| **Valuation 数字** | 「我值 $20M」 | 这是下一轮的 floor，不是成就 | 高估值 = 下轮必须更高（否则 down round） |
| **Pre vs Post money** | 两个数字 | 期权池算在 pre 还是 post 完全改变稀释 | 「$20M pre + 10% option pool pre」 = 你实际稀释 30%，不是 20% |
| **VC Ownership** | 「他要 20%」 | 基金数学倒推的结果 | 支票大小是固定的，估值决定所有权 |

**正常值（2026 市场）**：
- Pre-Seed: Pre-money $3-8M，raise $500K-2M
- Seed: Pre-money $6-15M，raise $2-5M
- Series A: Pre-money $20-60M，raise $8-20M
- Series B: Pre-money $80-300M，raise $20-80M
- （AI/hot sectors 乘以 2-5x）

**红旗值**：
- 估值明显高于行业中位数 → 下轮压力巨大
- 估值低于行业底线 + option pool 前置 → 你被低估 + 被稀释

### 1.2 Option Pool（期权池）

```
Post-Closing Option Pool: [X]% of fully-diluted post-money capitalization
Created out of pre-money (or post-money)
```

| 维度 | 真相 |
|------|------|
| **默认**：10-20% post-money | 最关键博弈：**前置 pre-money vs 后置 post-money** |
| **前置 pre-money** | 池子由创始人承担稀释 → 创始人实际股权少 |
| **后置 post-money** | 池子由所有人（含 VC）承担 → 创始人受益 |

**博弈点**：
- VC 默认写「pre-money」——你必须谈到 post-money
- 如果必须前置，谈 **smaller pool first, refresh later**（初始 5-10%，下轮再加）

**陷阱话术**：「我们需要 20% option pool pre-money for hiring」→ 你可以问 **「具体的 hiring plan 呢？如果招人 plan 只需 10%，我们先开 10%，下轮按需要再加」**

### 1.3 Liquidation Preference（清算优先权）

```
[X]x Liquidation Preference
Participating / Non-Participating / Capped Participating
Seniority: [Senior to common / Pari passu with other series]
```

这是 TS 里最容易被 overlook 但后果最严重的条款。

| 类型 | 意思 | 对创始人的影响 |
|------|------|-------------|
| **1x Non-Participating** | VC 要么拿回 1x 投资，要么按比例分 | **标准**。小退出 VC 拿本金，大退出 VC 按比例分 |
| **1x Participating** | VC 先拿回 1x 投资，**再** 按比例分剩余 | 🚩 **红旗**。小退出创始人几乎拿不到钱 |
| **1x Capped Participating** | Participating，但最多拿 2-3x | 中间状态。Cap 越低越好 |
| **2x/3x Non-Participating** | VC 拿回 2x/3x 或按比例，取较大 | 🚩🚩 **严重红旗**。只应在 distressed financing 出现 |
| **2x/3x Participating** | 最糟糕组合 | 🚩🚩🚩 **直接拒绝** |

**计算例子**（公司以 $50M 卖出，VC 投 $10M 持 20%）：

| 清算条款 | VC 拿到 | 创始人 + ESOP 拿到 |
|---------|--------|-----------------|
| 1x Non-Participating | max($10M, 20% × $50M = $10M) = $10M | $40M |
| 1x Participating | $10M + 20% × $40M = $18M | $32M |
| 2x Non-Participating | max($20M, $10M) = $20M | $30M |
| 2x Participating | $20M + 20% × $30M = $26M | $24M |

**博弈规则**：
- **1x Non-Participating** 是 2025-2026 美国一线 VC 的行业标准
- 任何 Participating 出现 → 让 VC 解释为什么（通常是 distressed 或 bridge round 才合理）
- **Seniority stacking**：多轮融资后清算优先权会 stack。默认是 pari passu（同级）——谈判确保不是 senior stacking

### 1.4 Anti-Dilution（反稀释）

```
Broad-Based Weighted Average Anti-Dilution Protection
(or Full Ratchet, or Narrow-Based Weighted Average)
```

保护 VC 不被下轮 down round 稀释。

| 类型 | 意思 | 影响 |
|------|------|------|
| **Broad-Based Weighted Average** | 按加权平均调整 VC 股数 | **标准**。温和保护 VC |
| **Narrow-Based Weighted Average** | 加权平均但分母小 | 🚩 红旗。对创始人更不利 |
| **Full Ratchet** | Down round 价格直接成为 VC 的 effective price | 🚩🚩🚩 **严重红旗**。Down round 时 VC 不受稀释，创始人全额承受 |

**博弈**：
- Broad-Based 是底线
- Full Ratchet 只在 distressed / bridge round 出现，正常融资拒绝
- Pay-to-play（投资人必须参与下轮才保留反稀释权利）= **对创始人有利的条款**，可主动提出

---

## Part 2：Control（权力）

### 2.1 Board of Directors（董事会）

```
Board Size: [X] members
Composition: [X] elected by common; [Y] elected by preferred; [Z] independent
```

| 阶段 | 健康结构 | 危险结构 |
|------|---------|---------|
| **Seed** | 2 founder + 1 independent (or 0 board) | 1 founder + 1 VC (VC 50% 投票) |
| **Series A** | 2 founder + 1 VC + 1-2 independent | 2 founder + 2 VC（平手僵局） |
| **Series B** | 2 founder + 2 VC + 1-2 independent (odd total) | 2 founder + 3 VC（创始人少数） |
| **Series C+** | 2-3 founder + 3-4 VC + 2-3 independent | 任何 setup 让创始人 < 40% |

**博弈规则**：
- **Independent 席位最重要**——由谁选 independent 决定谁控制
- 「由 common 和 preferred 共同同意」选 independent = 两边有 veto
- 「由 CEO 推荐 board approve」选 independent = CEO 主导但可被 board 否决
- **创始人被 fire 的最常见路径**：VC 多数 + independent 跟 VC 投票 → CEO 被替换

**融资阶段不应做的事**：
- Seed 阶段给任何 VC board seat（除非你投资人是战略级且你真的需要他）
- Series A 阶段让 VC 多数（2 founder + 2 VC + 1 VC-chosen independent = VC 有效控制）

### 2.2 Protective Provisions（保护性条款）

```
Actions requiring Preferred Majority consent:
- Liquidation, merger, sale of company
- Amendment of charter / bylaws
- Creation of new class of stock
- Payment of dividends
- Redemption of shares
- Incurring debt above $[X]
- Changing principal business
- Hiring/firing CEO
- Changing option pool size
- ...
```

Preferred（VC）对某些公司决策有一票否决权。

| 范围 | 正常 vs 不正常 |
|------|-------------|
| **重大事项**（M&A / 清算 / charter 修改） | 正常，所有 VC 都要 |
| **运营事项**（预算 / hiring / 产品方向） | 🚩 不正常，争取删除 |
| **Hire/fire CEO** | 🚩 红旗，这跟 board control 冲突 |
| **Debt above $[X]** | 正常，但确保 $X 够大（不能是 $100K） |
| **Change of business** | 正常，但争取定义「substantial change」 |

**博弈**：
- Protective provisions 是 VC 保护投资的基本权利，完全不给不现实
- 关键是 **范围限制** 和 **阈值合理**
- 最恶劣的 protective provisions：「Any transaction > $X」把日常运营纳入 veto 范围

### 2.3 Information Rights（信息权）

```
Information Rights for holders of [X]% or more of preferred:
- Annual audited financials
- Quarterly unaudited financials
- Monthly financials and KPIs
- Annual operating plan and budget
- Reasonable access to facilities and personnel
```

基本权利，不太需要博弈。但：
- **Monthly vs Quarterly**：monthly 合理，但 weekly 过度
- **Board observer rights**：有些 VC 要 observer 席位，这没有投票权但占坐位置 → 如果 board 人数有限制，observer 可以用
- **Inspection rights**：确保是「reasonable」，不是「at any time」

### 2.4 Drag-Along Rights（拖售权）

```
If [X]% of Preferred and [Y]% of Common approve a sale,
all other shareholders are required to vote in favor and sell.
```

VC 用来强制出售公司的工具。

| 阈值 | 对创始人影响 |
|------|-----------|
| **50% threshold** | 🚩 VC 可能强制你卖 |
| **66% threshold** | 平均 |
| **75% threshold** | 创始人友好（要求两类股东都过半） |

**博弈**：
- 要求 **Founder consent during employment period**（创始人在任时一票否决）
- 或要求 **Minimum sale price**（如果 drag-along，必须达到某个最低价格，比如 2x last valuation）
- **绝对红线**：Drag-along + 50% threshold + 无 minimum price + 无 founder consent = 任何时候 VC 联合就能把你赶出公司并卖掉

### 2.5 Right of First Refusal + Co-Sale（优先购买权 + 共同出售权）

```
Right of First Refusal: Preferred has first right to purchase shares founders want to sell
Co-Sale Right: Preferred has right to participate in founder sale pro-rata
```

限制创始人个人套现。

| 范围 | 正常 vs 不正常 |
|------|-------------|
| 所有 founder 股份 | 正常 |
| 小额（< $X）exemption | 争取，让你至少能套现一点 |
| 已 vested 的 option | 争取 exempt |

**正常值**：50% or more 创始人 equity 被 ROFR/Co-Sale 覆盖，但少量（10-20%）可以卖给第三方而不触发。

---

## Part 3：Founder-Specific

### 3.1 Vesting

```
Founder Shares: Subject to [X]-year vesting with [Y]-month cliff
Previously vested: [Z]% immediate vesting credit
```

| 维度 | 正常 vs 异常 |
|------|-----------|
| **4-year vesting, 1-year cliff** | 绝对标准，不用谈 |
| **Acceleration on termination without cause** | 正常，争取 |
| **Double-trigger acceleration** (change of control + termination) | 正常，争取 100% |
| **Single-trigger acceleration** (change of control alone) | 🚩 VC 会拒绝，因为影响 M&A 诱因 |
| **Pre-closing vesting credit** | 谈判：公司已经运营 X 年，应该 credit Y 月/X 月 |

**博弈**：
- Vesting 本身合理，不要抗拒
- 关键是 **acceleration** 和 **vesting credit**
- 如果已经 solo 创业 2 年 → 要求 2 年 credit（等于 50% 已 vested）
- **Reverse vesting trap**：如果你已经是 100% owner 然后融资，新的 vesting 会让你「reverse vest」——从 100% 被回购到 vesting 状态。要求明确 vesting 是 **前向** 不是 **反向**

### 3.2 Founder Restrictions

```
Transfer Restrictions: Founder shares cannot be transferred except...
Non-Compete: [X]-year post-termination
Non-Solicit: [Y]-year post-termination
```

| 维度 | 正常 vs 异常 |
|------|-----------|
| **Transfer restrictions** | 正常 |
| **Non-Compete 12-24 months** | CA 和一些州不可执行，其他州正常 |
| **Non-Compete > 24 months** | 🚩 过长 |
| **Non-Solicit 12-24 months** | 正常 |
| **IP assignment** | 正常，但确保定义是「work within scope of employment」，不是「any idea ever had」 |

### 3.3 Key Person Provisions

```
"Key Person" events trigger investor rights:
- Death of [founder]
- Termination of [founder]'s employment
- [founder]'s time commitment drops below [X] hours
```

| 类型 | 影响 |
|------|------|
| **Standard key person**（death/incapacity） | 正常 |
| **Time commitment triggers** | 🚩 可被滥用，可以争取删除 |
| **Key person triggers redemption right** | 🚩🚩 极端情况会出现，争取删除 |

---

## Part 4：Mechanics

### 4.1 No-Shop / Exclusivity

```
For [X] days after signing this TS, Company agrees not to solicit
other investors or proposals
```

| 时长 | 评价 |
|------|------|
| **30 days** | 正常 |
| **45 days** | 偏长 |
| **60+ days** | 🚩 过长 |
| **90 days** | 🚩🚩 你被锁住了 |

**博弈**：
- 30 days 是行业 default
- 换 30 days 去要求 VC 承诺「diligent efforts」和「milestones」
- **绝对谈**：如果 VC 主动 abandon，no-shop 立即失效

### 4.2 Expenses

```
Company will pay VC's legal expenses up to $[X]
```

| 金额 | 评价 |
|------|------|
| **$25K-$50K** | 正常（Seed/Series A） |
| **$50K-$75K** | 正常（Series B+） |
| **$100K+** | 🚩 过高 |
| **No cap** | 🚩🚩 永远不接受 |

### 4.3 Closing Conditions

```
Closing conditional upon:
- Completion of due diligence to VC's satisfaction
- Execution of [Standard documents]
- [Reference checks]
- [Technical review]
- ...
```

**陷阱**：
- 「DD to VC's satisfaction」= VC 可以任意退出。争取具体化或 time-boxed
- 「Reference checks」= 如果 reference 说你坏话，VC 可退出。确保 reference 提前打过招呼

### 4.4 Most Favored Nation（MFN）

```
If Company offers better terms to any subsequent investor in this round,
those terms are automatically extended to this investor
```

通常是合理条款，但注意：
- MFN 应该是 **this round only**，不是 future rounds
- MFN 应该是 **economic terms**，不应覆盖 governance terms

---

## Part 5：条款之间的耦合

### 组合 1：高估值 + Participating + Full Ratchet = 毒药

看起来估值高很爽，但：
- Down round 时 Full Ratchet 让 VC 不稀释
- Participating 让 VC 先拿本金再分剩余
- 结果：小退出 VC 拿大部分，创始人可能归零

**换算法则**：估值每高 20%，condition 每差一级，**实际净值可能反而低**。

### 组合 2：低估值 + Clean terms = 通常更好

- 1x Non-Participating
- Broad-based weighted average anti-dilution
- 2 founder + 1 VC + 1 independent board
- Standard protective provisions

这种 TS 即使估值低 15%，长期净值通常 > 「高估值+脏条款」的 TS。

### 组合 3：Signal 权重计算

同样的 TS，不同 VC 签署信号权重差 5-10x：

| VC Tier | 估值 Premium | 后续融资容易度 |
|---------|------------|-------------|
| Tier-1（a16z / Sequoia / Benchmark / Founders Fund） | +30-50% | 极大增幅 |
| Tier-2（Greylock / Lightspeed / NEA） | +10-20% | 中等增幅 |
| Tier-3（地区 VC / 新基金） | baseline | 小增幅 |
| Tier-4（无名天使） | -10-20% | 可能负信号 |

**策略**：如果 tier-1 和 tier-2 都 offer 你，优先 tier-1 即使估值低 20%——后续融资的 markup 会补回来。

---

## Part 6：创始人 TS 阅读 checklist

拿到 TS 后，逐条过：

- [ ] Pre vs Post money option pool 位置？
- [ ] Liquidation preference 是 1x Non-Participating？
- [ ] Anti-dilution 是 Broad-Based WA？
- [ ] Board composition 是否让创始人保留有意义的控制（种子不给 VC board seat）？
- [ ] Protective provisions 范围是否限于重大事项？
- [ ] Drag-along threshold ≥ 66%？
- [ ] Founder vesting 有 credit + acceleration？
- [ ] No-shop ≤ 45 days？
- [ ] Legal fees cap 合理？
- [ ] Closing conditions 不是开放式「to VC's satisfaction」？

任何红旗 → 至少和律师 + 1 个 founder-friendly VC（或天使）review。

---

## Part 7：常见 TS 博弈话术

| 情境 | VC 说 | 你说 |
|------|------|------|
| 期权池前置 | 「We need 20% option pool pre-money」 | 「What's the hiring plan? If it's 10% worth, let's do 10% now and refresh if needed. Otherwise I'm paying for hires I don't need.」 |
| 估值博弈 | 「Your valuation is too high」 | 「Compared to [comparable]? Let's see data. If you have a different number, let's negotiate on that」 |
| Board seat | 「We need a board seat at Seed」 | 「Happy to give observer rights at Seed. Board seat with your next check」 |
| No-Shop 过长 | 「We need 60 days」 | 「Industry standard is 30. What are you trying to do in 60 that 30 doesn't cover?」 |
| Full Ratchet | 「Full ratchet is standard for this round」 | 「Broad-based weighted average is standard. Show me 3 recent comparable TSs with full ratchet」 |
| Low valuation | 「This is a hot market, we're paying a premium already」 | 「Let me get 2 more TSs to triangulate. If market agrees with you, we have a deal. If not, we'll revisit」 |

---

## changelog

- v1.0 2026-04-17：首版。覆盖 Economics / Control / Founder-specific / Mechanics 四大块、30+ 条款、条款耦合分析、创始人 checklist、常见博弈话术。与主文件 Phase 3e 绑定。
