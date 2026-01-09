## 杂志风格信息卡片生成器

> __将文本转化为精美的社论风格信息图表__ —— 零设计门槛。

Claude Code 技能，将您的内容转化为美观的杂志风格信息卡片。适用于社交媒体、演示或知识分享。

[English](README.md)

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Claude Code Skill](https://img.shields.io/badge/Claude%20Code-Skill-blue)

---

## ✨ 示例输出

<div align="center">

### 30 秒生成，来自这段文本：

> "Claude Skills 是 Claude Code 的自定义能力扩展。主要优势：节省时间、保持一致性、高度定制化。工作流程：创建定义 → 设置触发 → 配置工具 → 添加指令。应用场景：代码生成、重构、文档自动化、测试验证、配置。"

**输出：** 4 张出版级卡片

<table>
  <tr>
    <td><img src="assets/claude-skills-card-1.png" alt="封面卡片" width="280"/></td>
    <td><img src="assets/claude-skills-card-2.png" alt="优势卡片" width="280"/></td>
  </tr>
  <tr>
    <td><img src="assets/claude-skills-card-3.png" alt="工作原理卡片" width="280"/></td>
    <td><img src="assets/claude-skills-card-4.png" alt="应用场景卡片" width="280"/></td>
  </tr>
</table>

_零设计技能。一键导出。出版级质量。_

</div>

---

## 为什么需要这个技能？

内容创作者面临普遍问题：

- __设计太难__ —— 不是每个人都能创作专业视觉内容
- __工具昂贵__ —— Figma、Canva 和 Adobe 都需要订阅
- __时间稀缺__ —— 学习设计会挤占内容创作时间
- __一致性差__ —— 每次设计风格都不统一

这个技能用一个命令解决所有问题。

## 解决方案

描述需求 → 获得出版级 HTML 卡片 → 导出为 PNG

```
您: "制作关于 Tailwind CSS 裁员的信息图"
↓
Claude 创建: 4 张精美卡片，包含数据、引用和分析
↓
点击: "导出所有卡片" → 下载 4 张高清 PNG
```

## 有什么不同？

| 特性 | 本技能 | 传统工具 |
|---------|-----------|-------------------|
| __学习曲线__ | 零（只需描述） | 陡峭 |
| __成本__ | 免费 | $10-60/月 |
| __设计时间__ | ~30 秒 | 数小时 |
| __一致性__ | 自动（设计系统） | 手动维护 |
| __导出质量__ | 2 倍分辨率 PNG | 参差不齐 |

## 安装

### 方式 1: 直接克隆（推荐）

```bash
# 进入 Claude Code 技能目录
cd ~/.claude/skills  # 或您的自定义技能路径

# 克隆此技能
git clone https://github.com/YOUR_USERNAME/editorial-card-generator.git
```

### 方式 2: 手动安装

1. 下载或复制 `editorial-card-generator` 文件夹
2. 放入您的 Claude Code 技能目录：
   - macOS/Linux: `~/.claude/skills/`
   - Windows: `%USERPROFILE%\.claude\skills\`

### 验证安装

在 Claude Code 中，当您以下操作时技能会自动激活：

- 要求"制作海报"、"创建卡片"或"设计信息图"
- 提到"可视化内容"或"信息图表"
- 请求"杂志风格设计"或"社论布局"

## 使用方法

### 示例 1: 科技新闻

```
制作关于此内容的信息图：

Tailwind CSS 裁员 75% 员工。收入下降 80%，因为
开发者使用 Cursor 等 AI 工具而非阅读文档。
旧商业模式（文档 → 流量 → 销售）已崩塌。
```

**输出：** 4 张卡片，包含大胆的数据可视化、深色数据卡片和行业分析

### 示例 2: 教育内容

```
制作可视化卡片解释：

什么是 Docker？
1. 容器将应用与依赖打包
2. 在任何地方一致运行
3. 比虚拟机快，比裸机更隔离
```

**输出：** 清晰的编号列表卡片，包含定义和用例

### 示例 3: 社交媒体线程

```
将这条推特线程转为卡片：

[关于生产力技巧的线程...]
```

**输出：** 每条推文成为一张可分享卡片，风格统一

---

## 🎨 设计系统

每张卡片遵循严格设计原则：

### 风格
- **流派**：现代社论风 + 瑞士国际主义风格
- **理念**：秩序、对比、大字号排版、纸媒质感
- **尺寸**：600px × 800px（3:4 比例）—— 完美适配 Instagram、Twitter

### 配色
```
背景: #f2efe9  (暖米白纸张)
文字: #1a1a1a  (深炭灰)
强调: #d95e00  (爱马仕橙)
```

### 字体
- **Noto Serif SC** (700, 900) — 标题
- **Noto Sans SC** (400, 500, 700) — 正文
- **Oswald** (500, 700) — 数字和英文

### 质感
- SVG 噪点叠加（透明度 0.06）营造纸感
- 深邃阴影（25px 模糊）制造悬浮效果
- 微妙渐变和透明度变化

## 卡片类型

技能智能地将内容分配到 3-6 张卡片：

### 第 1 张：封面
- 超大百分比或关键数字
- 粗体标题（48-56px）
- 简短标语

### 第 2-N 张：内容
- **列表卡片**：编号章节（01/02/03）
- **数据卡片**：深色背景、大号数据、关键引用
- **混合布局**：文字 + 视觉元素

### 第 N 张：封底
- 总结或行动呼吁
- 充裕留白
- 精心收尾

## 文件结构

```
editorial-card-generator/
├── SKILL.md        # 核心指令（Claude 阅读的内容）
├── examples/       # 实际输出示例
│   └── tailwind-crisis/
│       └── index.html
├── README.md       # 英文文档
├── README.zh.md    # 中文文档（本文件）
└── LICENSE         # MIT
```

## 技术栈

- **Tailwind CSS** — 实用优先样式
- **FontAwesome** — 图标
- **html2canvas** — HTML 转 PNG 导出
- **Google Fonts** — Noto 字体
- **SVG Filters** — 噪点纹理

## 适用场景

__非常适合：__

- 社交媒体内容（Instagram、Twitter、LinkedIn）
- 教育材料和教程
- 演示文稿
- 新闻简报视觉
- 知识分享
- 线程总结

__不适合：__

- 复杂数据可视化（使用图表）
- 视频内容
- 交互元素

## 致谢

- **瑞士国际主义风格** — Josef Müller-Brockmann 和巴塞尔学派
- **Google Fonts** — Noto 字体系列
- **html2canvas** — Niklas von Hertzen
- **Anthropic** — Claude Code 和 Agent Skills 框架

## 贡献

欢迎贡献！请：

1. Fork 仓库
2. 创建特性分支
3. 提交 Pull Request

贡献建议：
- 新配色主题
- 额外卡片布局
- 更多示例
- 设计系统改进

## 许可证

MIT License — 可自由使用、修改和分发。

## 致谢

感谢所有 star、fork 和使用此技能的人 —— 谢谢。好的设计应该对每个人开放，而不仅限于拥有设计工具或训练的人。

如果这个技能帮助您创造了美好事物，那就是我想要的。

---

**用 ❤️ 为 Claude Code 打造**
