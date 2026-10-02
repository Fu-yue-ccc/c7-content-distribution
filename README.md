# C7 内容传播 · 交付仓库

> 学号：2025105400112 ｜ 挑战：C7 内容传播（`ch-20260717031536-sfz852`）｜ 截止：2026-12-31

本仓库是 C7「内容传播」挑战的完整交付包。核心工作是**持续输出 2 篇内容**，把 C1–C6 阶段的真实实践沉淀为可传播的技术文章，并用发布后的传播数据证明影响力。

---

## 一、项目简介

C7 要求"持续发布至少 2 篇"+「用数据证明影响力」+「内容必须来自 C1–C6 的真实实践」。据此确定两篇互补选题：

- **文章一（技术深度向）**：把 C4D 的本地大模型地图 Agent 与 C6 的 Web 应用串成一条完整故事线 —— 用 Ollama + Gemma 4 在本地零 API 费用运行模型，自动生成带分类标记的交互式校园地图。
- **文章二（流量干货向）**：把 C5 / C5A 的 GitHub 实践改写成零基础教程 —— 从注册账号到发布第一个开源项目，六步 30 分钟完成。

一篇展示技术能力，一篇覆盖最广受众，形成互补传播结构。

---

## 二、交付物索引（对照平台必交清单）

| 必交项 | 对应文件 | 状态 |
|--------|----------|------|
| `*文章标题*` | `Student_C7_文章标题.md`（2 篇标题 + 摘要 + 发布登记） | ✅ 已提供 |
| `*数据截图*` | `screenshots/`（每篇 6 张：已发布 / 手机效果 / 24h 数据 / 7d 数据 / 互动 / 群分享） | ⏳ 待发布后补齐 |
| `*AI日志*` | `Student_C7_AI日志.md`（7 阶段 19 轮完整协作记录） | ✅ 已提供 |

辅助文档：`Student_C7_文章链接.md`（链接登记 + 群内分享话术）、`Student_C7_拿来说明.md`（参考来源与借鉴说明）、`Student_C7_注册发布指南.md`（发布操作指引）。

---

## 三、两篇文章

### 文章一

- **标题**：零 API 费用！我用本地大模型做了一个 AI 地图生成器
- **一句话摘要**：用 Ollama + Gemma 4 在本地零费用运行 AI，自动生成带分类标记的交互式校园地图，含完整技术实现与踩坑经验。
- **正文源文件**：[`articles/article1_map_generator/article.md`](articles/article1_map_generator/article.md)
- **公众号排版版**：[`articles/article1_map_generator/article_wechat.html`](articles/article1_map_generator/article_wechat.html)
- **关联挑战**：C4D + C6

### 文章二

- **标题**：从来没用过 GitHub？这篇教你 30 分钟发布第一个项目
- **一句话摘要**：新手友好的 GitHub 入门教程，从注册账号、创建仓库、写 README、上传文件到 Fork 项目，六步 30 分钟发布第一个开源项目，附常见错误避坑指南。
- **正文源文件**：[`articles/article2_github_guide/article.md`](articles/article2_github_guide/article.md)
- **公众号排版版**：[`articles/article2_github_guide/article_wechat.html`](articles/article2_github_guide/article_wechat.html)
- **关联挑战**：C5 + C5A

---

## 四、目录结构

```
c7-content-distribution/
├── README.md                        # 本文件：项目总览与交付物索引
├── Student_C7_文章标题.md            # 必交项①：2 篇文章标题与发布登记
├── Student_C7_AI日志.md              # 必交项③：AI 协作全过程记录（19 轮）
├── Student_C7_文章链接.md            # 链接登记与群内分享话术
├── Student_C7_拿来说明.md            # 参考来源与借鉴说明
├── Student_C7_注册发布指南.md        # 公众号 / 知乎发布操作指引
├── articles/
│   ├── article1_map_generator/
│   │   ├── article.md               # 文章一正文（Markdown 源）
│   │   └── article_wechat.html      # 文章一公众号排版版（全内联样式）
│   └── article2_github_guide/
│       ├── article.md               # 文章二正文（Markdown 源）
│       └── article_wechat.html      # 文章二公众号排版版（全内联样式）
└── screenshots/
    └── README_截图说明.md            # 必交项②的采集规范（6 张 / 篇）
```

---

## 五、发布与传播计划

| 阶段 | 时间 | 动作 |
|------|------|------|
| 第 1 周 | 第 1 周 | 发布文章一 → 采集 24h / 7d 数据 |
| 第 2 周 | 第 2 周 | 发布文章二 → 采集 24h / 7d 数据 |
| 持续 | 发布后 | 班级群 / 朋友圈分享，记录互动数据 |

发布平台：微信公众号（主）/ 知乎（备）。发布后的真实数据截图按 `screenshots/README_截图说明.md` 的命名规则入库。

---

## 六、AI 协作说明

全程 7 个阶段、19 轮 AI 协作，覆盖：任务解析 → 选题策划 → 大纲设计 → 初稿撰写 → 标题优化 → 改稿润色 → 排版生成 → 文档撰写。

关键做法：AI 只负责生成候选与结构，**事实与数字全部人工回溯核验**（Ollama/Gemma 4 对照官方文档、坐标数据对照高德 POI、GitHub 操作对照官方文档、Git 命令对照 git-scm 文档）。

记录了 2 个 AI 误导案例及修正：① 公众号 HTML 需要全内联样式（class 与 style 标签会被过滤）；② AI 描述的 GitHub 按钮位置与实际界面有出入，改为用按钮文字而非位置描述。详见 `Student_C7_AI日志.md`。

---

## 七、诚实声明

- 两篇文章正文已完成，并已生成公众号可用的排版版 HTML。
- 文章的**发布与传播数据采集仍在进行中**，`screenshots/` 中的 6 类数据截图待文章实际发布后补齐。
- 本仓库**不预填任何未实际产生的传播数据**；`Student_C7_文章标题.md` 中的链接与发布日期字段在发布后回填。
