# VC Playbook Suite

> **把创投圈的博弈知识，结构化到 AI 里的开源工具集。**
>
> 6 个 Claude Skill，覆盖创业者从 pitch 到 IPO 的全链条博弈——pitch 自杀测试、融资战役推演、TS 条款反打、DD 尽调模拟、董事会政变防御。
>
> 面向创业者、VC 从业者、FA、法务。

![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-v1.0-green.svg)
![Skills](https://img.shields.io/badge/skills-6-purple.svg)
![Content](https://img.shields.io/badge/content-280K%20chars-red.svg)
![Built with](https://img.shields.io/badge/built%20with-Claude%20Opus-orange.svg)

---

## 这是什么

一组 Claude Skill——**可以直接把整个文件夹塞进 Claude Desktop、Cursor、或任何支持本地文件加载的 AI 工具里**，让 AI 按照里面的方法论给你做分析。

不是知识百科（那种东西 Wikipedia 有）。

是 **博弈引擎**——你给它一个具体情境（"我收到一份天使轮 TS，帮我分析"），它吐出结构化决策（条款红/橙/黄/绿分类 + 真实估值折算 + 三项必争 + 5级让步阶梯 + 反打话术 + VC 预测 counter + 你的 counter-counter）。

**它做到的事，是一个在创投圈待了 15 年的老炮坐在你对面 3 小时能做到的事。**

## 快速开始

### 用法 1：复制粘贴（最懒，5 分钟）

打开你常用的 AI（Claude / ChatGPT / 任何能读 Markdown 的）。

1. 进入这个仓库对应的 skill 目录，比如 [`term-sheet-negotiator/SKILL.md`](./term-sheet-negotiator/SKILL.md)
2. 点 Raw → 全选 → 复制
3. 粘贴到 AI 对话框，然后说：

   > "以上是一个创投博弈方法论。请严格按照里面的流程，帮我分析这份 TS：[贴你的 TS]"

AI 会按 skill 里的 Phase 1-4 流程完整跑一遍，输出诊断报告+反打策略。

### 用法 2：Claude Desktop / Cursor 本地加载（推荐）

如果你用 Claude Desktop 或 Cursor，把整个仓库 clone 到 skills 目录，AI 会**自动加载**，对话里点名 skill 就能调用。

```bash
# Claude Desktop 用户
cd ~/Library/Application\ Support/Claude/skills/
git clone https://github.com/Sammilux/vc-playbook-suite.git

# Cursor 用户
cd ~/.cursor/skills/
git clone https://github.com/Sammilux/vc-playbook-suite.git
```

重启 AI 工具，然后对话中直接说：

> "用 term-sheet-negotiator 帮我分析这份 TS..."
> "跑一次 vc-pitch-killtest 看看我这个项目能不能过..."
> "检查一下 board-dynamics-wargame，我觉得 VC 最近在搞我..."

### 用法 3：企业级私有部署（给技术团队）

把你们公司的历史 TS、历史董事会纪要、历史投资人邮件，塞到一个**私有仓库**。然后在 `.cursor/skills/` 下同时 clone 本仓库作为公共基础层。

让 Claude 以"**贵司的创投幕僚长**"身份运作——它既懂公共方法论（本仓库），又懂你们公司的历史和人物关系（私有仓库）。

这个配置跑起来，相当于一个 **7×24 在线、永不跳槽、知道你公司所有融资历史的 VP of Corporate Development**。

---

## 六个 Skill 一览

### 1. `vc-pitch-killtest` — Pitch 自杀测试

**适用**：pre-seed 到 Series A，见 VC 前的自我压力测试。

**功能**：模拟 6 种典型 VC 人格（异端猎手/增长机器/平台玩家/品味大师/企业收割机/工程原教旨），从各自视角把你的项目狠狠骂一遍。

**输出**：10-bullet kill test + 6 persona 投票 + 反组合幽灵触发话术 + 10 个经典 kill test 案例 + 新赛道（AI Agents/Humanoid/TechBio/DePIN）权重调整。

### 2. `founder-fundraising-wargame` — 融资战役推演（美版）

**适用**：创始人在美元基金/硅谷 VC 语境下融资。

**功能**：4 个 Phase 推演完整融资战役——时间棋盘/信息战/pitch 排序/反组合幽灵利用/DD 反侦察/FOMO 设计。包含 Phase 2 美国 6 人投委会模拟 + Phase 2.5 六层融资战役。

**卫星**：term-sheet-anatomy（TS 条款字典）、us-casebook（10 个美国创投死法）、vc-persona-debate-us（对 6 persona 的应答台本）、bridge-round-playbook（桥梁轮博弈）。

### 3. `china-fundraising-wargame` — 融资战役推演（中国版）

**适用**：创始人在中国 VC 语境下融资（人民币基金 + 美元基金 + 产业 CVC + 政府引导基金）。

**功能**：三体博弈模型（创始人+VC+政府），6 层融资战役推演。包含 65 处对国资/引导基金/人民币基金/CVC/返投/战投等中国特有场景的覆盖。

**卫星**：persona-debate-scripts（中国 VC 6 人辩论）、exit-endgame（退出策略）、new-tracks-playbook（新赛道打法）、fa-countergame（FA 双面博弈+创始人画像调制器）、combat-casebook（8 个中国创投死法案例 Playbook）、BENCHMARK-TEMPLATE（空白测试框架，让读者跑自己的项目）。

### 4. `term-sheet-negotiator` — TS 条款反打

**适用**：收到 TS 之后，签字之前。

**功能**：三层博弈方法论（Opening Move 识别 + 压力点计算 + Trade-off Stack 构建）+ 4 阶段谈判流程（诊断/构建/执行/关闭）。**不是识别条款，是反打 VC 套路**。

**卫星**：clause-casebook（30 条款的 VC opening + 创始人反打 + 5 级让步阶梯 + trade 选项）。

### 5. `vc-due-diligence-simulator` — DD 尽调模拟器

**适用**：TS 签了，进入 3-week DD 阶段。

**功能**：从 VC 分析师视角模拟 3 周 DD——24 个刁钻问题（分 8 类）+ reference call 脚本（前员工/customer/industry expert）+ 10 个 red flag 识别 + 4 阶段 DD 执行流程。

**卫星**：dd-casebook（10 个 DD 案例，5 失败 + 5 成功）。

### 6. `board-dynamics-wargame` — 董事会政变推演

**适用**：融完资进董事会之后。

**功能**：CEO 去留博弈引擎——5 类 board member 分析 + 12 种 boardroom move + 12 类 coup triggers + 7 层 coup-proofing defense。

**卫星**：board-coup-casebook（15 个 CEO 去留案例深度拆解——Sam Altman/OpenAI、Travis Kalanick/Uber、Steve Jobs/Apple、Adam Neumann/WeWork、Zuckerberg/Meta 等）。

---

## 推荐使用路径

按你现在的阶段选 skill 组合：

| 阶段 | 推荐 skill 组合 |
|------|--------------|
| **还没见 VC** | `vc-pitch-killtest` 把自己狠狠虐一遍 |
| **开始见 VC** | `founder-fundraising-wargame` 或 `china-fundraising-wargame` 看整体战役布局 |
| **收到 TS** | `term-sheet-negotiator` + `founder-fundraising-wargame/term-sheet-anatomy.md` 组合使用 |
| **TS 签了 DD 中** | `vc-due-diligence-simulator` |
| **融完资进董事会** | `board-dynamics-wargame` 长期防御 |
| **融资失败要 bridge** | `founder-fundraising-wargame/bridge-round-playbook.md` |
| **全链条总览** | 读 [`EVOLUTION-INDEX.md`](./EVOLUTION-INDEX.md) |

---

## 这些 skill 是怎么来的

不是一个 AI 凭空生成的。

是一个在创投圈待了 15 年的从业者，把自己脑子里的博弈经验，借助 Claude (Anthropic Opus 4.7) 结构化而成。

**人做架构设计（哪些知识值得结构化、怎么拆分、如何差异化）**，**AI 做生产（把每一条博弈经验写成 case + 话术 + checklist）**。

3 小时做完。

完整故事见 [配套文章](https://mp.weixin.qq.com/)（公众号首发后更新链接）。

---

## 贡献指南

这个仓库欢迎以下贡献：

- **新案例**：你遇到的典型 VC/TS/董事会博弈案例（脱敏后），PR 提交到对应 skill 的 casebook
- **新话术**：你用过有效的反打话术，PR 提交到对应 clause-casebook
- **新赛道扩展**：新兴行业（AI Agents / Humanoid / Climate Tech 等）的 killtest 调整，PR 提交到 `vc-pitch-killtest/new-tracks-killtest.md`
- **翻译**：把某个 skill 翻译成英文，方便海外读者使用
- **bug 报告**：发现错误的数据（比如 "NVCA 2025 年 78% Series A 是 Non-Participating" 这种 claim 过期了），提 issue

**PR 原则**：
- 案例/数据必须有来源（公开报道、SEC 文件、创始人公开声明等）
- 话术要符合行业真实语气（不装不油腻）
- 不对号入座骂特定公司或个人（本仓库的立场是**不指名道姓但讲真话**）

---

## 免责声明

本仓库内容仅供方法论参考，**不构成法律建议或投资建议**。

- 任何具体 TS 签署前请咨询专业律师
- 融资博弈涉及双方长期关系，请结合自身情境判断，不要机械套用话术
- 本仓库作者不对使用这些 skill 产生的任何决策后果负责

---

## License

[MIT License](./LICENSE) — 你可以自由使用、修改、分发、商用，只要保留版权声明。

---

## Star & Share

如果这个仓库帮到你——

- ⭐ **Star 一下**（对我是最好的反馈）
- 🔗 **分享给正在融资的朋友**（帮一个是一个）
- 🐛 **提 Issue 告诉我哪里错了**（帮我升级）
- 🚀 **提 PR 补充你的经验**（帮整个社区升级）

**创投圈的知识民主化，从今天开始，往前推一小步。**
