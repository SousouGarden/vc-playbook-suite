# Bridge Round Playbook — 融资不达标时的桥梁轮博弈

> v2.0 新增。与主文件 Phase 4「融后过渡」绑定使用。

**本文件解决什么问题**：
- 正常融资不达标怎么办？
- 下轮机构不给 term sheet，现有股东要求续血怎么办？
- 如何用 SAFE / Convertible Note / bridge preferred 桥过这 6-12 个月？
- 什么时候放弃桥过、接受 down round？

**为什么需要独立文件**：
bridge round 是 **融资博弈中最多陷阱的一类**——定义上是「临时方案」，实际上决定创始人 1-2 年后的控制权。大部分 bridge round 的创始人没预料到三件事：
1. 现有股东的 pro-rata 和 anti-dilution 会 stack
2. Bridge discount + cap 的组合会比 down round 稀释更大
3. 「bridge 到下一轮」的假设通常 fail，然后 bridge 变成最后一轮

---

## Bridge Round 的典型场景

### 场景 A：PMF 不足但 runway 用完
- 已融 seed，原计划 18 月到 Series A
- Month 15 PMF 信号还不够 strong
- 需要 6 月 extension 来 push metrics
- **典型融资量**：$2-5M 为 6-9 月 extension

### 场景 B：Series A 价差过大
- 现有 post-money $30M 从 Series A
- Series B 市场给你 $40M pre（即 down round 或 flat）
- 希望等 12 月后市场/估值修复再融
- **典型融资量**：$5-15M 为 12 月 runway

### 场景 C：Down round 但大股东挽救
- 市场下跌 / 公司 miss milestone
- 下轮估值会是 last round 的 0.5-0.7x
- 现有股东（领投）宁愿给 bridge 也不 down round
- **典型融资量**：$3-10M 为 6-12 月

### 场景 D：战略等待期（pre-IPO）
- Series C 已经完成
- 计划 12 月后 IPO
- 需要 extension 打 Q4 数字更好看
- **典型融资量**：$20-100M 为 12 月

---

## Bridge 工具选择

### 工具 1：SAFE（Simple Agreement for Future Equity）

**适合场景**：Seed 阶段 bridge、小金额快速关闭

**Key terms**：
- **Post-money SAFE（YC v2）**：$X valuation cap，X% discount (或 cap 或 discount)
- **Pre-money SAFE（YC v1）**：已过时，不要用

**优点**：
- 法律文档简短（通常 2-4 页）
- closing 快（1-2 周）
- 不需要 pricing round

**陷阱**：
- **Cap 会 convert 成稀释**——$20M SAFE cap + raise Series A at $50M → SAFE investor 以 $20M price convert，你实际稀释超过你想象
- **Multiple SAFEs 会 stack**——如果你 Year 1 做了 3 个 SAFE，每个不同 cap，合计稀释 >30% 可能
- **MFN clause trap**——第二个 SAFE 如果有 MFN，会 retroactively 改变第一个

**定价策略**：
- Cap 建议 = 你对下轮估值的 pessimistic 预测 × 0.8（给 SAFE investor 稍微优惠）
- Discount 默认 20%

### 工具 2：Convertible Note

**适合场景**：早期有 debt 优势（如 bridge 到可能的 strategic acquisition）

**Key terms**：
- **Valuation cap**（与 SAFE 类似）
- **Discount**（与 SAFE 类似）
- **Interest rate**（通常 5-8%，compounding）
- **Maturity date**（通常 18-24 月）
- **Conversion trigger**（通常是 qualified financing ≥ $X）

**优点**：
- Debt 性质给 lender 优先权
- 清算时 preferred to equity

**缺点**：
- Maturity 到期但没 trigger → 需要 repay or extend（谈判痛苦）
- Interest accrues 增加稀释
- 在一些 state 可能被认定为 loan，需要 legal 仔细处理

**2026 现实**：Convertible Note 大部分场景被 SAFE 取代，除非你需要 debt senior 或 tax 原因

### 工具 3：Bridge Preferred（"Pre-A" or "Series Seed-2"）

**适合场景**：Bridge 金额大（>$3M）、现有股东主导、走向 priced round

**Key terms**：
- **Valuation**（通常 == last round valuation，即 "flat round"，或 small bump）
- **Liquidation preference**（1x non-participating standard）
- **Pro-rata rights**（所有 bridge investors）
- **Anti-dilution**（broad-based weighted average）

**优点**：
- Pricing 明确，不 stack
- 后续融资更简单（term sheet 已有模板）
- Governance 正式（board / information rights 清晰）

**缺点**：
- 关闭需要 4-8 周（vs SAFE 1-2 周）
- Legal fees $50K+
- Valuation 公开，影响下一轮定价

### 工具 4：Venture Debt

**适合场景**：有 ARR 的 SaaS 公司 bridge / extend runway without dilution

**Key terms**：
- **Principal amount**（通常 2-4x MRR 或 30-50% of last equity raise）
- **Interest rate**（5-15% 取决于 risk）
- **Warrants**（通常 5-10% of principal as equity warrants）
- **Covenants**（revenue milestones / cash minimums）

**Provider**：SVB (Deep-Ops)、Bridge Bank、Hercules、Runway Growth

**优点**：
- Low dilution（warrants 比 equity 稀释小得多）
- 配置 runway extension

**缺点**：
- Covenants 可能 trigger default（miss revenue 时最糟糕）
- Interest 是真金白银 cash outflow
- Warrants 稀释虽小但 stack

**关键 caveat**：Venture debt 不是「替代融资」，是「补充融资」。如果你 raise 失败，venture debt 会加速死亡（不减缓）

---

## Bridge 稀释实算

### 案例 1：多个 SAFE stack 的稀释陷阱

**假设**：
- Seed $3M at $10M post-money → VC 持 30%，founder 持 70%
- Bridge 1: SAFE $1M @ $15M cap（6 月后）
- Bridge 2: SAFE $1.5M @ $12M cap（10 月后）
- Series A: $10M at $40M pre-money

**Series A 时 conversion**：

| 投资人 | 投资金额 | Conversion price | 所得股份 | 稀释 |
|-------|---------|----------------|---------|------|
| SAFE 1 | $1M | $15M cap | $1M / $15M = 6.67% | 6.67% |
| SAFE 2 | $1.5M | $12M cap | $1.5M / $12M = 12.5% | 12.5% |
| Series A | $10M | $40M | 20% | 20% |

**Total SAFE + Series A 稀释**：6.67% + 12.5% + 20% = **39.2%**

如果跳过 SAFE 直接 Series A：
- Founder 被稀释 20% 直接

**结论**：2 个 SAFE ($2.5M 桥) 让你 **额外稀释 19.2%**。如果只是为了 6 月延长 runway，这个 cost 可能大于收益。

### 案例 2：Bridge Preferred vs Down Round

**假设**：
- Series A: $20M post-money，VC 25%，founder 75%
- Series B 市场给 $30M pre-money（flat），但 milestone miss，VC 要求 $15M（down round 0.75x）
- Alternative: Bridge Preferred $5M at flat $20M

**Option A：Down Round $15M**（raise $5M）
- Pre-money $15M + raise $5M → post $20M，new VC 25%
- 加上 anti-dilution trigger（broad-based weighted average），Series A VC 被 reprice
- **Founder 稀释**：from 75% → ~55-60%（取决于 anti-dilution 具体计算）
- **Psychology**：Down round 在招聘和 PR 中是负信号

**Option B：Bridge Preferred $5M flat**
- Pre-money $20M + raise $5M → post $25M，new bridge 20%
- 不触发 Series A anti-dilution
- **Founder 稀释**：from 75% → 60%
- **Psychology**：flat round 可以 present as "interim"

**结论**：Bridge 稀释类似 down round，但 **心理和 signaling cost 大不同**。如果你有 confidence 6-12 月后能 raise above $30M pre，bridge 是更好选择。

---

## Bridge Round 的关键谈判点

### 谈判点 1：Valuation / Cap

**现有股东视角**：cap 越低对他们越好（以低价 convert）
**新 bridge 投资人视角**：cap 越低对他们越好
**创始人视角**：cap 越高越好

**博弈策略**：
- 提出 **next round 预测 × 0.8 cap**（给 bridge 投资人 20% discount on future round）
- 如果多人参与 bridge，用 tranching（每个 tranche 不同 cap）

### 谈判点 2：Participation Rights

- Bridge 投资人是否有 Series A pro-rata？
- 默认：是（pro-rata on bridge amount as % of post-bridge cap table）
- 博弈：限制 pro-rata 只在 Next round，不在所有后续

### 谈判点 3：Liquidation Preference Stack

- Bridge preferred 的 liquidation 是 senior 还是 pari passu 于 Series A？
- 默认要求：**Pari passu**（同级）
- 红旗：Bridge 要求 senior stacking → 如果公司以中等价格卖出，bridge 先拿 → 创始人拿不到

### 谈判点 4：Governance

- Bridge 投资人是否有 board seat？
- 默认：否（如果 flat/extension bridge）
- 博弈：如果必须给，给 observer rights，不给投票权

### 谈判点 5：Information Rights

- Bridge 投资人是否有 monthly reports + budget access?
- 默认：是，但不 additional 于现有 info rights
- 博弈：避免 bridge-specific 的 quarterly business review

### 谈判点 6：Milestones / Covenants

- Bridge 是否 tied to milestones（revenue / cash burn / hire）？
- 默认：**No milestones**
- 红旗：「Bridge of $5M, $2M at signing, $3M on revenue milestone $X」→ 如果 miss，你拿不到后 tranche，但承担了 expectations

---

## Bridge Round 的"时机不对"信号

有时 bridge 不应该做，应该接受 down round 或 sell company：

### 信号 1：Bridge 3 次以上
- 第一次 bridge 通常合理
- 第二次是警告
- 第三次 = 你的公司在 slow-motion death spiral
- 决策：stop bridging，要么 raise real round 要么 sell

### 信号 2：每次 bridge 金额递减
- Bridge 1: $3M
- Bridge 2: $1.5M
- Bridge 3: $500K
- 这说明现有股东越来越不 believe
- 决策：准备 sell

### 信号 3：No new investor joins
- 如果所有 bridge 都是 inside round (现有股东)，新 VC 不进
- Market signal: 外部不 believe
- 决策：或者 pivot，或者 sell，不要继续 bridge

### 信号 4：Cash burn 大于 revenue
- Bridge 给你 runway，但 burn rate 依然 > revenue
- 你在用 bridge 续命，不是 bridge 到 new milestone
- 决策：cut burn 50%，或 sell

### 信号 5：最大 customer / 员工离开
- Key customer churn + key engineer 离职 + bridge → triple warning
- 决策：sell 或关闭

---

## Bridge 失败后的选项

### 选项 A：Down Round
- 接受市场估值
- 处理 anti-dilution 再融新轮
- 对 PR / 招聘负面但可恢复

### 选项 B：Asset Sale / Acquihire
- 你 + 核心团队 + IP 卖给大公司
- 投资人通常拿回 1x 或 0.5x
- 创始人可能拿到 earn-out + new package

### 选项 C：Wind Down
- 关闭公司
- 还剩 cash 退还投资人（pro-rata）
- 创始人可以 walk away 去做下一个创业

### 选项 D：Personal guarantee / debt
- **永远不要做这个**
- 创始人个人承担公司债务，家庭财务 meltdown 风险

---

## Bridge Round checklist

开始 bridge 讨论前：

- [ ] 我是否清楚知道 bridge 后的下一个 milestone 和 timeline？
- [ ] 我是否有 realistic plan 在 bridge 期结束前 raise real round 或 exit？
- [ ] Bridge 金额是否 **够到 real round**（不是 halfway）？
- [ ] Bridge 是否让我 reach 一个 meaningfully different 的 narrative（不只是「更多 runway」）？
- [ ] 我是否算过 bridge 后的 cap table + 稀释场景？
- [ ] 所有现有 investor 是否参与 bridge（如果没有，为什么）？
- [ ] Bridge 工具（SAFE vs preferred）的选择是否正确？
- [ ] Bridge 的 term 是否 clean（没 senior stacking、没 harsh milestones）？
- [ ] 我是否有 PLAN B（raise 失败的话）？
- [ ] 我是否准备好 honest conversation with board / investors？

---

## 典型的 bridge 剧本

### 剧本 A：从 loss of momentum 反弹
```
Month 14: 意识到 PMF 不足，Series A 不可能
Month 15: 对齐 board，提议 bridge $3M for 9 月 extension
Month 16: Close bridge (SAFE at $15M cap)
Month 17-22: Focus on 3 metrics, ignore everything else
Month 23: Series A at $25M pre (market 认可 metric 改善)
结果：稀释 $3M/$15M = 20% + $10M/$35M = 28.6%，合计 ~48%
但如果 bridge 不做：Month 17 关闭公司
```

### 剧本 B：从 market downturn 等待回暖
```
Month 18: Series B 市场给 flat round（$50M post == last round）
Month 19: board 讨论 - flat 不合理，先 bridge 12 月
Month 20: Close bridge preferred $8M at $50M pre
Month 21-32: 执行 plan，保持 burn 可控
Month 33: Series B at $80M pre (market 回暖)
结果：稀释 $8M/$58M = 13.8% + $15M/$95M = 15.8%，合计 ~29%
直接 down round 可能 triggering anti-dilution 更大损失
```

### 剧本 C：从 death spiral 到 acquihire
```
Month 15: Seed runway 不足，bridge 1: SAFE $1M
Month 18: Bridge 不够，bridge 2: SAFE $500K（inside only）
Month 20: No new bridge available，burn rate > revenue
Month 22: Strategic 买家 approach，offer acquihire $5M + earn-out
Month 23: Close acquihire，投资人拿回 0.8x，创始人拿到 $2M earn-out
结果：不理想但 graceful exit，创始人可以做下一个 project
```

---

## 给创始人的 3 个 hard-earned lessons

### Lesson 1：Bridge 是 narrative 不是 runway
- 工具本身不改变公司命运
- Bridge 给你**时间和金钱**去改变 narrative
- 如果 narrative 不会变（比如 PMF 已经 3 年没 improve），bridge 只是延迟死亡

### Lesson 2：Inside round 听起来温情，实则高成本
- 现有股东给 bridge 是「保护他们原有投资」
- 但他们会 price it hard（低 cap / senior terms）
- 外部 VC 愿意进入 bridge = strong signal 公司 viable
- 如果没外部 VC 进，你应该质疑

### Lesson 3：Best bridge is no bridge
- 如果你能避免 bridge（通过 cost cutting / revenue push / small milestone），不要做
- Bridge 每一轮都让你 cap table 更 complicated、negotiation 更 weakened
- 很多创始人把 bridge 当作「延缓痛苦」但实际是「放大后续痛苦」

---

## changelog

- v1.0 2026-04-17：首版。覆盖 4 种 bridge 场景、4 种 bridge 工具（SAFE/Note/Preferred/Venture Debt）、稀释实算案例、6 大谈判点、5 个危险信号、3 种 bridge 后选项、3 个典型剧本。与主文件 Phase 4「融后过渡」绑定。
