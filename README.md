# wiki-series-skill

VitePress Wiki 原创系列文章生成技能。用于产出图文并茂的技术解读系列，支持网站截图、SVG 架构图、Mermaid 流程图、AI 生图等多种视觉元素。

## 目录结构

```
wiki-series-skill/
├── SKILL.md          # 技能核心定义
├── README.md         # 本文件
├── LICENSE           # MIT License
├── .gitignore        # 忽略 output/
├── templates/        # 三种系列模板
│   ├── template-a-tool-review.md        # 工具解读型（如 jvm-tools）
│   ├── template-b-platform-analysis.md  # 平台分析型（如 iot-platform-design）
│   └── template-c-optimization-guide.md # 优化指南型（如 java-startup-optimization）
└── output/           # 草稿产出（git 忽略）
```

## 使用方法

将 `SKILL.md` 内容作为 System Prompt 提供给 AI 工具，然后：

1. 说"开一个新系列"→ 进入系列规划流程
2. 说"写一篇 XX 系列的下一篇"→ 进入单篇生成流程
3. 说"继续 XX 系列"→ 自动接续上次进度

## 适用系列类型

| 类型 | 模板 | 代表作 |
|------|------|--------|
| 工具解读 | template-a | Chris Newland JVM 工具解读（10 篇） |
| 平台分析 | template-b | 物联网平台设计解读（50 篇） |
| 优化指南 | template-c | Java 启动速度优化解读（6 篇） |

## 核心特色

- **图文并茂**：每篇至少 2 个视觉元素（截图 + SVG / Mermaid）
- **真实截图**：AI 自动访问工具网站并截取关键界面
- **SVG 架构图**：根据文章内容生成矢量架构图
- **动态开头标题**：`## 0` 标题随内容变化，避免模板化
- **结构化编号**：`## 1 → ## 2 → ## 3` 递进式章节

## 关联项目

- Wiki 站点：[yeatsliao.github.io/wiki](https://yeatsliao.github.io/wiki)
- Wiki 仓库：[github.com/YeatsLiao/wiki](https://github.com/YeatsLiao/wiki)
