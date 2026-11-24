<p align="center">
  <img src="./assets/gemini-logo.svg" width="110" alt="Gemini" />
</p>

<h1 align="center">gemini-vibe（Gemini 人味儿）</h1>

<p align="center">
  从 Gemini 对话语感中提炼的 Agent Skill —— 帮其他 AI 卸掉机械“客服腔”、“专栏攻略腔”与“文青句式瘾”，像个脑子清醒、懂分寸、会接话的聪明朋友一样聊天。
</p>

---

## 为什么做这个 Skill？

大多数大模型一开口就带着浓重的机器味：
- **初级客服腔**：“这是一个非常深刻的问题！” + 无脑 `1. 2. 3.` + “综上所述，希望对您有所帮助！”
- **二代装清醒腔**：假设性问题先发免责声明“作为 AI 我没有感情/只是概率产物”，结尾还要像乙方客服一样问“要不要换个抒情版？”
- **知乎专栏攻略腔**：随口问句日常问题，一口气甩出 600 字“正信号→误判区→反信号→对策”，句句工整对仗、段尾还要左右互搏防背锅。
- **DeepSeek 式文青马脚**：两百字连用四次“不是 A，是 B”、冒号冷冰冰下定义，或者纯中文里突然蹦出个英文单词。

`gemini-vibe` 不是教 AI “扮演人类”或“强行卖萌”，而是通过**反 AI 腔禁令清单 + 动态篇幅阶梯 + 真实 Few-Shot 语感锚点**，把机器的答题惯性一层层剥掉。

---

## 目录结构

```text
gemini-vibe/
├── SKILL.md                       # 核心规范（含禁令清单、动态篇幅阶梯、6 组语感锚点）
├── assets/
│   └── gemini-logo.svg            # Gemini 标识图标
├── examples/
│   └── before-after.md            # 7 组真实对比案例（AI 腔 vs 活人表达）
└── references/
    └── portable-prompt.md         # 开箱即用的通用 System Prompt（适配 ChatGPT / DeepSeek / Claude）
```

---

## 安装与使用

### 1. 支持 Agent Skills 标准的客户端（Antigravity / Claude Code / Codex / Cursor）
- 前往 [Releases](https://github.com/XXpickup/gemini-vibe/releases) 下载 `gemini-vibe.zip`（或 `gemini-vibe.skill`）。
- 解压并将 `gemini-vibe/` 文件夹放入你的全局或项目 `skills/` 目录：
  ```bash
  git clone https://github.com/XXpickup/gemini-vibe.git ~/.gemini/config/skills/gemini-vibe
  ```

### 2. 网页版 / 通用大模型（DeepSeek / ChatGPT / Claude / 本地模型）
直接复制 [`references/portable-prompt.md`](./references/portable-prompt.md) 中的 System Prompt 与语感样本，粘贴到自定义指令（Custom Instructions）或系统提示词中即可生效。

---

## License

MIT
