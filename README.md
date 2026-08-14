<div align="center">

<img src="assets/logo.svg" alt="Modex" width="160" />

# Modex · MH Agent

### AI 全自动数学建模智能体 · 兼顾科研全流程

**一条命令,从赛题到竞赛级论文 —— 建模、求解、编程、绘图、成文,一夜跑完。**
**国赛 / 美赛 / 华为杯全流程覆盖,同样能做文献调研到投稿级论文的科研全流程。**

[![数学建模](https://img.shields.io/badge/数学建模-CUMCM_|_MCM/ICM_|_华为杯-e11d48)](#-数学建模竞赛支持)
[![Platform](https://img.shields.io/badge/平台-Windows_桌面软件-2563eb)](#-快速开始)
[![Skills](https://img.shields.io/badge/Skill-90%2B_可组合-8b5cf6)](#-90-个可组合-skill)
[![Website](https://img.shields.io/badge/官网-mingheng.xin-16a34a)](https://www.mingheng.xin)

[**🌐 官网**](https://www.mingheng.xin) · [**📥 下载**](#-快速开始) · [**📖 使用说明**](#-使用说明) · [**💬 问题反馈**](../../issues)

> ⚠️ 本仓库为**产品展示与问题反馈仓库**,只包含说明文档,不含产品源码。

</div>

---

## ✨ 核心能力

- **数学建模竞赛全流程** —— 读题拆解 → 数学建模 → 求解计算 → 编程实现 → 数据图表 → 竞赛级论文 → 编译合规检查,交题时一道赛题,收工时一份论文。
- **科研全流程** —— 文献调研、Idea 发现、新颖性验证、实验部署、自动审稿、论文写作到投稿级 PDF,端到端自动化。
- **跨模型对抗式协作** —— Claude 负责执行,GPT / GLM / MiniMax 等模型负责审稿,两个模型互不评自己的作业,形成真正的对抗式反馈。
- **实时工作流监控** —— WebSocket 秒级推送步骤进度与日志,关键决策点设检查点,支持确认 / 改意见 / 单步重跑。
- **在线 LaTeX 编辑器** —— 三栏布局(文件树 + 代码 + PDF 预览),对话式 AI 编辑,10 项格式自动检查,一键编译。
- **90+ 可组合 Skill** —— 每个是纯 Markdown `SKILL.md`,任何 LLM 都能读懂,自由混搭或串联成流水线。

---

## 🚀 快速开始

Modex 是一个 **Windows 桌面软件**,开箱即用,无需自己配环境。

1. 前往 [**官网 mingheng.xin**](https://www.mingheng.xin) 下载安装包
2. 安装后启动(内已封装 Python / Node / Git / TeXLive / MiKTeX / Pandoc / draw.io / Claude CLI 全套运行时)
3. 首次使用在设置页填入模型配置(执行者 Claude + 评审者 API),一键测试连接
4. 选一个模板(数模竞赛 / 科研工作流),填参数,开跑

软件支持自研增量更新,新版本自动提示。

---

## 🏆 数学建模竞赛支持

每种竞赛都有完整流水线:**赛题分析 → 建模求解 → 编程实现 → 图表生成 → 论文撰写 → 编译合规检查**,关键步骤设检查点。支持上传赛题 PDF/Word 自动提取文本,支持 `output_format=docx`(走 Word 导出,跳过 LaTeX 编译)。

| 竞赛 | 语言 | 页数 | 模板 | 特色 |
|------|------|------|------|------|
| 国赛 (CUMCM) | 中文 | 20 | cumcmthesis | 完整竞赛论文结构 |
| 美赛 (MCM/ICM) | 英文 | 25 | mcmthesis | Summary Sheet 优先 |
| 华为杯 | 中文 | 30 | gmcmthesis | 严格字体要求 |
| MathorCup | 中文 | 30 | ctexart 自定义 | 含目录页 |
| APMCM | 英文 | 25 | — | 承诺书单独提交 |
| 统计建模 | 中文 | 30 | — | 自拟题目,自采数据 |

---

## 🧠 跨模型对抗式协作

Modex 区别于普通 AI 写作工具的根本设计:**绝不用单模型自我博弈。**

```
┌─────────────────┐         审稿反馈          ┌──────────────────┐
│   Claude Code    │  ◀───────────────────    │   评审模型         │
│   (执行者)        │                          │  GPT / GLM /      │
│  写代码/求解/成文   │  ───────────────────▶    │  MiniMax / Kimi   │
└─────────────────┘         提交产物          └──────────────────┘
      两个模型互不评自己的作业 → 真正的对抗式反馈,天然更难被 game
```

同一个模型审自己的输出会有系统性盲区。跨模型审稿,就像 adversarial bandit vs stochastic bandit,天然更难被欺骗。**模型自由组合**:不限于 Claude + GPT,支持 GLM、MiniMax、Kimi、DeepSeek 等任意 OpenAI 兼容 API,甚至可通过 ModelScope 零成本接入。

---

## 🧩 90+ 个可组合 Skill

每个 Skill 就是一个 `SKILL.md` 文件,纯 Markdown,任何 LLM 都能读懂。可自由混搭,也可串联成完整流水线。

- **科研类** —— 文献调研 · Idea 发现 · 新颖性验证 · 外部评审 · 实验规划/部署 · 结果分析 · 论文写作 · PDF 编译 · 自动审稿循环
- **竞赛类** —— 赛题分析 · 建模求解 · 编程实现 · 中/英论文撰写 · 编译合规检查
- **写作类** —— 开题报告 · 文献综述 · 课程论文 · 人文社科写作 · 基金申请书 · 会议幻灯片 · 会议海报 · 定理证明
- **图表类** —— AI 架构图 · Mermaid · draw.io / TikZ · Nature 风格配图 · 数据驱动图表

---

## 📖 使用说明

1. **安装启动** —— 从[官网](https://www.mingheng.xin)下载安装包,安装后直接启动,全套运行时已内置,无需额外配置。
2. **配置模型** —— 首次进入在设置页填入模型配置:执行者(Claude)+ 评审者(GPT / GLM / MiniMax 等任意 OpenAI 兼容 API),点一键测试确认连通。
3. **新建工作流** —— 选一个模板(数模竞赛 / 科研工作流),按引导填参数:竞赛类型、语言、赛题 PDF/Word(可上传自动提取)、是否开启改进循环等。
4. **监控与干预** —— 工作流实时显示每步进度和日志;在关键决策点会自动暂停等你确认,可以「确认继续 / 提交修改意见 / 单步重跑」。
5. **查看产物** —— 论文、图表、PDF 等产物按步骤分组展示,核心产物高亮;可用内置在线 LaTeX 编辑器进一步调整并一键编译。

---

## ⚠️ 注意事项

- **需自备模型 API** —— 软件本身不含模型额度。需要你自己的 Claude(执行者)与评审模型 API Key,调用会产生相应费用。可通过 ModelScope 等接入免费额度降低成本。
- **需要联网** —— 文献检索、模型调用、引用核对都依赖网络,请保持网络畅通(国内环境部分服务可能需要代理)。
- **产出务必人工复核** —— AI 生成的内容可能存在错误或不准确之处,论文结论、数据、引用在使用前请自行核实,不要直接照搬。
- **遵守学术规范** —— 本软件是辅助工具。竞赛投稿、论文发表请遵守相应的学术诚信与参赛规则,对最终成果负责的是使用者本人。
- **运行耗时** —— 完整流水线(尤其含实验、多轮审稿、LaTeX 编译)可能耗时较长,建议在空闲时段运行。
- **首次运行** —— Windows 下个别杀毒软件可能误报,如遇拦截请添加信任;安装路径建议避免过深或含特殊字符的中文目录。

---

## 📚 文档

- [使用说明](#-使用说明) —— 安装、配置、运行流程
- [注意事项](#-注意事项) —— 使用前必读
- [官网](https://www.mingheng.xin) —— 下载、使用指南、更新日志

---

## 💬 问题反馈

在本仓库的 [**Issues**](../../issues) 提交:

- 🐛 Bug 报告(附复现步骤、系统环境、日志)
- 💡 功能建议
- ❓ 使用疑问

---

## 📧 联系我们

- 邮箱:[support@mhcoding.ai](mailto:support@mhcoding.ai)
- 官网:[mingheng.xin](https://www.mingheng.xin)

---

## 🙏 参考与致谢

本项目的理念、工作流方法论与部分 Skill 素材,受益于以下开源项目,在此致谢:

**核心方法论参考**
- [wanshuiyin/Auto-claude-code-research-in-sleep](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep) —— 自动化科研工作流理念来源

**社区 Skill / 模板**
- [WUBING2023/PaperSpine](https://github.com/WUBING2023/PaperSpine) —— 论文骨架 Skill
- [huangwb8/ChineseResearchLaTeX](https://github.com/huangwb8/ChineseResearchLaTeX) —— 中文科研 / NSFC LaTeX 模板
- [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) —— 科研 Agent Skill 集
- [ganzhi-black/humanities-thesis-skill](https://github.com/ganzhi-black/humanities-thesis-skill) —— 人文社科论文写作 Skill
- [Doryoku1223/lunwen-skill](https://github.com/Doryoku1223/lunwen-skill) —— 中文论文写作 Skill

以及底层执行器 [Anthropic Claude Code](https://github.com/anthropics/claude-code)。各项目版权归其原作者所有,遵循各自的开源许可证。

---

<div align="center">

**Modex · MH Agent** —— 让 AI 做重复性工作,你专注于真正需要人类洞察的部分。

*Copyright © 明珩科技 (MH Coding) · 保留所有权利*

</div>

