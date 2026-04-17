# EVOLUTION INDEX — 全链条创投博弈 skill 地图

> 一份导览文档。告诉你**在什么阶段用哪个 skill**，以及 skill 之间的**协同方式**。

---

## 一张图看懂整个流程

```
创业者生命周期                              对应 Skill
─────────────────────────────────────────────────────────
⬇ 阶段0：idea 阶段，还没见VC             vc-pitch-killtest
⬇ 阶段1：开始融资，见第一个VC             founder-fundraising-wargame
⬇                                         china-fundraising-wargame
⬇                                         (二选一，看你面对美元基金还是中国VC)
⬇ 阶段2：多个VC同时在谈                   founder-fundraising-wargame (Phase 2.5)
⬇                                         + anti-portfolio-ghosts.md
⬇ 阶段3：收到 TS                          term-sheet-negotiator
⬇                                         + term-sheet-anatomy.md
⬇                                         + clause-casebook.md
⬇ 阶段4：TS 签了，进入 DD                 vc-due-diligence-simulator
⬇                                         + dd-casebook.md
⬇ 阶段5：融资关闭前最后一周                term-sheet-negotiator (Phase 4)
⬇ 阶段6：融完资进董事会                   board-dynamics-wargame
⬇ 阶段7：进入下一轮 / 面临 bridge          bridge-round-playbook.md
⬇ 阶段8：出现 coup 迹象                   board-coup-casebook.md
⬇ 阶段9：考虑退出 / acquire / IPO         china-fundraising-wargame/exit-endgame.md
─────────────────────────────────────────────────────────
```

---

## 6 个主 skill 的互补关系

| Skill | 核心功能 | 用在什么时候 | 姊妹 skill |
|-------|---------|-----------|-----------|
| `vc-pitch-killtest` | Pitch 前的压力测试 | 见 VC 前 1-2 周 | — |
| `founder-fundraising-wargame` | 美版融资完整推演 | 融资开始到关闭 | china-fundraising-wargame |
| `china-fundraising-wargame` | 中国版融资三体博弈 | 融资开始到关闭（中国场景） | founder-fundraising-wargame |
| `term-sheet-negotiator` | TS 条款反打兵法 | 收到 TS 到签字 | founder-fundraising-wargame/term-sheet-anatomy |
| `vc-due-diligence-simulator` | 模拟 VC 做 DD | TS 签到 closing | — |
| `board-dynamics-wargame` | 董事会政治博弈 | 融完资后长期 | — |

---

## 关键文件交叉引用图

### Pitch 阶段
- `vc-pitch-killtest/SKILL.md` — 主框架
- `vc-pitch-killtest/persona-debate-scripts.md` — 投委会内部辩论逐字稿
- `vc-pitch-killtest/anti-portfolio-ghosts.md` — 顶级 VC 的 anti-portfolio + 触发话术
- `vc-pitch-killtest/kill-test-casebook.md` — 10 个 kill test 案例
- `vc-pitch-killtest/new-tracks-killtest.md` — 新赛道调整

### 融资战役阶段
**美版**：
- `founder-fundraising-wargame/SKILL.md`
- `founder-fundraising-wargame/vc-persona-debate-us.md` — 对 6 persona 的应答台本
- `founder-fundraising-wargame/us-casebook.md` — 10 个美国创投死法

**中国版**：
- `china-fundraising-wargame/SKILL.md`
- `china-fundraising-wargame/persona-debate-scripts.md` — 中国 VC 6 人辩论
- `china-fundraising-wargame/new-tracks-playbook.md` — 新赛道打法（中国）
- `china-fundraising-wargame/exit-endgame.md` — 退出策略
- `china-fundraising-wargame/fa-countergame.md` — FA 双面博弈 + 创始人画像调制器
- `china-fundraising-wargame/combat-casebook.md` — 8 个中国创投死法案例 Playbook
- `china-fundraising-wargame/BENCHMARK-TEMPLATE.md` — 空白测试框架（让读者跑自己的项目）

### TS 阶段（最关键）
- `term-sheet-negotiator/SKILL.md` — 谈判方法论
- `term-sheet-negotiator/clause-casebook.md` — 30 条款反打
- `founder-fundraising-wargame/term-sheet-anatomy.md` — 条款字典（配合使用）

### DD 阶段
- `vc-due-diligence-simulator/SKILL.md`
- `vc-due-diligence-simulator/dd-casebook.md` — 10 DD 案例

### 融后 / 董事会阶段
- `board-dynamics-wargame/SKILL.md`
- `board-dynamics-wargame/board-coup-casebook.md` — 15 CEO 去留案例
- `founder-fundraising-wargame/bridge-round-playbook.md` — 桥梁轮

---

## 典型场景下的 Skill 组合

### 场景 A：第一次融天使轮 / 种子轮

**推荐顺序**：
1. `vc-pitch-killtest` （见 VC 前自杀测试）
2. `china-fundraising-wargame` 或 `founder-fundraising-wargame` （融资战役规划）
3. 收到 TS → `term-sheet-negotiator` + `term-sheet-anatomy`
4. 签字前 → 再跑一次 `clause-casebook` 审一遍

### 场景 B：正在谈 Series A，多个 VC 在手

**推荐顺序**：
1. `founder-fundraising-wargame` Phase 2.5（六层战役）
2. `vc-pitch-killtest` 针对每个 VC 的 persona 做差异化
3. 第一个 TS 到手 → `term-sheet-negotiator` 立刻启动
4. 同时对未出 TS 的 VC 制造 FOMO

### 场景 C：融完资后，董事会有异常信号

**推荐顺序**：
1. `board-dynamics-wargame` 主文件（识别是 Red Flag 还是 Yellow Flag）
2. `board-coup-casebook` 找类似案例
3. 如果确认 coup 正在发生 → 主文件 Phase 5 的"coup 发生时 playbook"
4. 确认后考虑是否 bridge → `bridge-round-playbook`

### 场景 D：准备退出 / 并购 / IPO

**推荐顺序**：
1. `china-fundraising-wargame/exit-endgame.md` 退出路径规划
2. `board-dynamics-wargame` 确保 board 支持退出决策
3. `term-sheet-negotiator` 用于谈判退出条款

---

## 升级版本说明

### v1.0（2026-04-17 首发）

本次发布包含：
- 6 个主 skill
- 16 个卫星文件（含案例库 + 话术库 + 场景调整 + FA 博弈 + 死法 Playbook）+ 1 个空白 Benchmark Template
- 约 30 万字中文内容 / 10000+ 行 Markdown
- 从 Seed 到 IPO 全链条覆盖

### 未来可能的升级方向

- [ ] **持续案例积累**：每个 skill 的 casebook 持续增加新案例
- [ ] **新赛道扩展**：AI Agents / Humanoid / Climate Tech / TechBio 持续更新
- [ ] **中国场景细化**：人民币基金 / 国资 / CVC 的专门卫星文件
- [ ] **翻译版本**：主 skill 的英文版本，让海外读者也能用
- [ ] **2027 市场校准**：所有 calibration anchor 根据新市场数据更新

---

## 设计哲学

### 1. 主文件 + 卫星文件 = 可扩展而不失焦

每个 skill 主文件控制在 300-500 行（只放方法论+ high-level framework），把详细案例、话术库、checklist 分别放进卫星文件。

**效果**：主文件支持"一口气读完"，卫星文件支持"按需深挖"。

### 2. 差异化定位比覆盖度更重要

skill 之间严格差异化：
- `term-sheet-anatomy`（**字典**：每条是什么）≠ `term-sheet-negotiator`（**兵法**：怎么反打）
- `vc-pitch-killtest/persona-debate-scripts`（**VC 内部辩论**）≠ `founder-fundraising-wargame/vc-persona-debate-us`（**创始人外部应答**）

没有严格差异化，六个 skill 会变成六个互相重复的"创投 101"。

### 3. 案例 + 方法论 + checklist 三角支撑

每个 skill 必须有三种内容类型：
- **方法论**（5-7 个 Phases 或 Principles）
- **案例**（10+ 个具体 scenarios）
- **Checklist**（创业者可以直接用的 20-40 项清单）

缺任何一角，skill 都是不可运行的。

### 4. 让 AI 负责"结构化的苦工"，人负责"结构决策"

skill 生产过程：
- **人**做决定——哪些知识值得结构化、如何拆分主文件与卫星、两个 skill 的 overlap 怎么处理
- **AI** 做执行——写 30 条款反打话术、写 15 个董事会政变案例、写各 persona 的应答台本

人做架构，AI 做建筑。

---

## 免责声明

本仓库内容仅供方法论参考，**不构成法律建议或投资建议**。任何具体 TS 签署前请咨询专业律师。

---

## 致谢

- [Anthropic Claude (Opus 4.7)](https://www.anthropic.com/) — 本工具集的生产伙伴
- 过去 15 年所有和我在深夜聊过 TS 的创业者朋友们——你们的每个问题都变成了这里面的一个 case
