# MedPen / 捉刀 — 临床医学论文撰写助手

<p align="center">
  <b>🩺 AI 驱动的临床研究写作伴侣</b><br>
  <i>从研究设计到期刊投稿 — 为临床医生和医学研究者打造的一站式技能</i>
</p>

<p align="center">
  <a href="./README.md">English</a> ·
  <a href="#-快速开始">快速开始</a> ·
  <a href="#-功能特色">功能特色</a> ·
  <a href="#-prompt-库">Prompt 库</a> ·
  <a href="#-快速开始">快速开始</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-v0.9.0--preview-blue" alt="Version">
  <img src="https://img.shields.io/badge/license-MIT-green" alt="License">
  <img src="https://img.shields.io/badge/language-中英双语-brightgreen" alt="Language">
</p>

---

## 📖 为什么叫"捉刀"？

> **"捉刀"** — 典出《世说新语》，曹操命崔琰代己接见匈奴使者，自己持刀立于旁。后引申为"代笔"之意。

撰写临床医学论文绝非易事。你需要：
- 驾驭复杂的研究设计（RCT、队列研究、病例对照...）
- 遵循严格的报告规范（CONSORT、STROBE、PRISMA、CARE...）
- 满足不同期刊的特定要求（NEJM、Lancet、JAMA、BMJ、Stroke、Neurology...）
- 在中英文写作之间自如切换
- 处理统计分析与数据可视化
- 准备投稿材料（Cover Letter、Rebuttal...）

**MedPen（捉刀）** 是一个综合性 AI 技能，通过 **21 个专业 Prompt** 为你提供从研究设计到期刊投稿的全流程指导，专为临床医学场景量身定制。

---

## ✨ 功能特色

### 🎯 全流程覆盖

| 阶段 | Prompt | 功能说明 |
|------|--------|----------|
| **研究设计** | #1-2, #11 | RCT/队列/病例对照设计、样本量计算、统计方案规划 |
| **论文撰写** | #3-7, #13-14, #20 | 结构化摘要、IMRaD 各章节、病例报告、系统综述 |
| **翻译润色** | #8-10 | 中英互译、自然学术表达润色、学术语气优化 |
| **统计与图表** | #11-12 | 分析方案设计、医学图表推荐（KM 曲线、森林图...） |
| **投稿准备** | #15-17, #19 | 期刊选择、Cover Letter、投稿前自查清单 |
| **审稿回复** | #17 | Rebuttal 撰写、审稿人意见处理 |
| **质量审查** | #18-19 | 模拟审稿人、投稿前检查清单 |
| **基础研究** | #20-21 | 实验方法撰写、公开数据集分析（TCGA、SEER、MIMIC...） |

### 🌍 中英双语支持

- **英译中**：为中文期刊投稿（中华医学杂志等）提供地道翻译
- **中译英**：为国际期刊投稿（NEJM、Lancet 等）提供专业润色
- **自然学术表达润色**：将草稿打磨为流畅、地道的学术表达

### 📋 医学报告规范内置

- **CONSORT 2025** — 随机对照试验
- **STROBE** — 观察性研究
- **PRISMA 2020** — 系统综述与 Meta 分析
- **CARE** — 病例报告
- **TRIPOD** — 预测模型
- **STARD** — 诊断准确性研究

### 🏥 期刊覆盖范围

MedPen 提供的写作指导兼容广泛的医学期刊谱系，从综合性医学顶刊到各专业领域的临床与基础研究期刊均适用。结构化报告、伦理合规与统计透明等核心原则具有普适性，具体的格式要求可根据目标期刊灵活调整。

---

## 🚀 快速开始

### Trae / OpenClaw 用户

1. **克隆**本仓库：
```bash
git clone https://github.com/Neuro-S/MedPen.git
```

2. **复制**技能文件夹到技能目录：
```bash
# Trae
cp -r MedPen ~/.trae/skills/

# OpenClaw
cp -r MedPen ~/.openclaw/skills/
```

3. **重启** IDE 或发送 `/reload`

4. **开始使用** — 直接说：
   - *"帮我设计一个临床研究"* → 触发 Prompt #1
   - *"把我的中文草稿翻译成英文"* → 触发 Prompt #8
   - *"我有初稿了，帮我准备投稿"* → 触发子流程：#15→#16→#19
   - *"帮我回复审稿人"* → 触发 Prompt #17

### Cursor 用户

1. **克隆**本仓库：
```bash
git clone https://github.com/Neuro-S/MedPen.git
```

2. **复制** `.cursor/rules.md` 文件（如有）或直接在 Cursor 的 composer/chat 中打开 `references/prompts.md`。

3. **开始使用** — 提及 Prompt 编号或用自然语言描述任务。

### Claude Code 用户

1. **克隆**本仓库：
```bash
git clone https://github.com/Neuro-S/MedPen.git
```

2. **复制**技能文件夹到 Claude Code 技能目录：
```bash
# macOS / Linux
cp -r MedPen ~/.claude/skills/

# Windows (PowerShell)
cp -r MedPen "$env:USERPROFILE\.claude\skills\"
```

3. **开始使用** — Claude Code 会根据你的请求自动检测技能。

### GitHub Copilot 用户

1. **克隆**本仓库：
```bash
git clone https://github.com/Neuro-S/MedPen.git
```

2. **复制** `.github/copilot-instructions.md`（如有）到你的仓库，或在 Copilot Chat 中引用 `references/prompts.md`。

3. **开始使用** — 在 Copilot Chat 中描述你的任务。

### 手动使用（任意 AI 工具）

1. 打开 [`references/prompts.md`](./references/prompts.md)
2. 复制你需要的 Prompt
3. 粘贴到 Claude、ChatGPT、Cursor 等任意 AI 助手
4. 填入你的内容并运行

---

## 📋 Prompt 库

### 模块一：研究设计与方案

| # | Prompt | 触发语 |
|---|--------|--------|
| 1 | 临床研究设计咨询 | "帮我设计一个研究" |
| 2 | 样本量计算指导 | "计算样本量" |

### 模块二：论文结构化撰写

| # | Prompt | 触发语 |
|---|--------|--------|
| 3 | 医学论文结构化摘要 | "写摘要" |
| 4 | 引言撰写 | "写引言" |
| 5 | 方法撰写 | "写方法" |
| 6 | 结果撰写 | "写结果" |
| 7 | 讨论撰写 | "写讨论" |

### 模块三：中英双语翻译与润色

| # | Prompt | 触发语 |
|---|--------|--------|
| 8 | 中文学术论文英译（医学专用） | "翻译成英文" |
| 9 | 英文学术论文中译（医学专用） | "翻译成中文" |
| 10 | 自然学术表达润色（英文） | "润色学术表达" |

### 模块四：统计分析与数据呈现

| # | Prompt | 触发语 |
|---|--------|--------|
| 11 | 医学统计分析方案设计 | "设计统计方案" |
| 12 | 医学图表制作指导 | "推荐图表" |

### 模块五：病例报告与特殊文体

| # | Prompt | 触发语 |
|---|--------|--------|
| 13 | 病例报告撰写（CARE 规范） | "写病例报告" |
| 14 | 系统综述/Meta 分析撰写（PRISMA 规范） | "写系统综述" |

### 模块六：投稿准备与审稿回复

| # | Prompt | 触发语 |
|---|--------|--------|
| 15 | 期刊选择与投稿策略 | "推荐期刊" |
| 16 | Cover Letter 撰写 | "写投稿信" |
| 17 | 审稿人意见回复（Rebuttal） | "回复审稿人" |

### 模块七：论文质量审查

| # | Prompt | 触发语 |
|---|--------|--------|
| 18 | 模拟医学期刊审稿人 | "审我的论文" |
| 19 | 医学论文投稿前自查清单 | "投稿前检查" |

### 模块八：医学基础研究辅助

| # | Prompt | 触发语 |
|---|--------|--------|
| 20 | 基础医学论文方法撰写 | "写实验方法" |
| 21 | 公开医学数据集分析论文指导 | "分析公开数据集" |

---

## 📁 项目结构

```
MedPen/
├── README.md              # 英文版
├── README_CN.md           # 本文件（中文版）
├── LICENSE                # MIT 许可证
├── SKILL.md               # 轻量任务路由器
├── .gitignore             # Git 忽略规则
├── docs/                  # 文档
│   ├── USAGE.md           # 详细使用指南
│   ├── ROADMAP.md         # 未来开发路线图
│   └── images/            # 截图 / 示意图
└── references/            # 核心规则与 Prompt 库
    ├── safety-and-compliance.md
    ├── minimum-inputs.md
    ├── quality-gates.md
    ├── statistical-anti-misuse.md
    ├── journal-requirements.md
    ├── medical-terminology.md
    └── prompts.md
```

---

## 🎯 子流程快速入口

无需从头开始，直接跳转到任意子流程：

| 子流程 | 触发语句 | Prompt 链 |
|--------|----------|-----------|
| **翻译→投稿** | "我有中文初稿，帮我翻译并准备投稿" | #8 → #10 → #15 → #16 → #19 |
| **仅翻译润色** | "帮我翻译/润色这段论文" | #8 或 #9 或 #10 |
| **仅投稿准备** | "帮我准备投稿材料" | #15 → #16 → #19 |
| **仅审稿回复** | "帮我回复审稿人意见" | #17 |
| **仅质量审查** | "帮我审查这篇论文" | #18 或 #19 |
| **仅统计咨询** | "帮我设计统计方案" | #11 → #12 |
| **仅病例报告** | "帮我写病例报告" | #13 |
| **仅系统综述** | "帮我写系统综述" | #14 |

---

## 🛡️ 安全边界

- ❌ 绝不编造患者数据、实验结果或统计值
- ❌ 绝不伪造伦理审批号或临床试验注册号
- ❌ 绝不捏造参考文献
- ✅ 所有 AI 生成内容需经作者核实
- ✅ 临床决策不能仅基于 AI 建议
- ✅ 涉及患者信息时必须去标识化

---

## 🔮 扩展路线图

MedPen 采用模块化设计，预留扩展接口：

| 模块 | 功能 | 技术路线 |
|------|------|----------|
| 模块九 | 参考文献管理（自动格式化、DOI 补全） | Python + Crossref/PubMed API |
| 模块十 | 医学数据预处理（Table 1 自动生成） | Python/R |
| 模块十一 | 统计图表自动生成（KM 曲线、森林图等） | Python/R |
| 模块十二 | 报告规范合规检查 | Python 规则引擎 |
| 模块十三 | 期刊格式自动适配 | Python + 期刊模板库 |
| 模块十四 | 医学术语智能校对 | Python + MeSH 词典 |
| 模块十五 | 公开数据集接口（SEER、MIMIC、TCGA） | Python + 数据集 API |

详见 [docs/ROADMAP.md](./docs/ROADMAP.md)。

---

## 🤝 贡献指南

欢迎贡献！你可以通过以下方式参与：

1. **提交 Issue**：报告问题或建议新功能
2. **提交 PR**：改进现有 Prompt 或添加新模板
3. **分享案例**：提交使用案例和最佳实践

### 贡献流程

```bash
# 1. Fork 本仓库
# 2. 创建分支
git checkout -b feature/your-feature

# 3. 提交更改
git commit -m "Add: 新增 XXX 功能"

# 4. 推送到分支
git push origin feature/your-feature

# 5. 创建 Pull Request
```

---

## 📄 许可证

本项目采用 [MIT 许可证](./LICENSE)。

你可以：
- ✅ 自由使用、修改、分发
- ✅ 用于商业目的
- ✅ 用于学术研究

要求：保留原作者署名和许可证声明。

---

## 🙏 致谢

- 灵感来源于 [awesome-ai-research-writing](https://github.com/Leey21/awesome-ai-research-writing)
- 参考了 [research-writing-skill](https://github.com/alfonso0512/research-writing-skill)
- 参考了 [academic-writing-skills](https://github.com/bahayonghang/academic-writing-skills)
- 为全球临床医生、医学研究者和研究生而构建

---

<p align="center">
  <b>MedPen / 捉刀</b> — 以医者之笔，成学术之佳。
</p>
