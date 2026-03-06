# OpenClacky Skills

[English](#english) | [中文](#中文)

---

## English

A Clacky AI skills repository containing the `openclacky-code` skill, which delegates coding tasks to the `openclacky` CLI tool.

### Directory Structure

```
code-skills/
  openclacky-code/
    _meta.json   # Platform metadata (ownerId, slug, version, publishedAt)
    SKILL.md     # Skill definition (YAML frontmatter + Markdown instructions)
```

### Getting Started

#### Prerequisites

- Install the [openclacky](https://github.com/clacky-ai) CLI tool

#### Usage

**Plan:**
```bash
openclacky agent -m "Build a snake game"
```

**Build (new session):**
```bash
openclacky agent --mode=auto_approve --path [repo dir] -m "/new"
```

**Build (continue session):**
```bash
openclacky agent --mode=auto_approve --path [repo dir] -c -m "[follow-up instruction]"
```

**Interactive (manual confirmation):**
```bash
openclacky agent --mode=confirm_safes --path [repo dir]
```

### Examples

#### Build a Game
```bash
openclacky agent --mode=plan_only --path /projects/snake-game -m "Build a Snake game with HTML5 Canvas, arrow key controls, score display, and game over screen."
openclacky agent --mode=auto_approve --path /projects/snake-game -m "Plan approved. Implement it."
```

#### Build a Website
```bash
openclacky agent --mode=plan_only --path /projects/portfolio -m "Build a responsive personal portfolio site with Next.js: home, about, projects, and contact sections. Dark mode toggle."
openclacky agent --mode=auto_approve --path /projects/portfolio -m "Plan approved. Implement it."
```

#### Build an Agent
```bash
openclacky agent --mode=plan_only --path /projects/weather-agent -m "Build a CLI agent in Python that takes a city name, calls OpenWeatherMap API, and replies with a natural language weather summary using an LLM."
openclacky agent --mode=auto_approve --path /projects/weather-agent -m "Plan approved. Implement it."
```

---

## 中文

Clacky AI 技能仓库，包含 `openclacky-code` 技能，用于将编码任务委托给 `openclacky` CLI 工具。

### 目录结构

```
code-skills/
  openclacky-code/
    _meta.json   # 平台元数据（ownerId、slug、version、publishedAt）
    SKILL.md     # 技能定义（YAML frontmatter + Markdown 指令）
```

### 快速开始

#### 前置条件

- 安装 [openclacky](https://github.com/clacky-ai) CLI 工具

#### 使用方式

**规划阶段：**
```bash
openclacky agent -m "开发贪吃蛇"
```

**构建（新会话）：**
```bash
openclacky agent --mode=auto_approve --path [repo dir] -m "/new"
```

**构建（继续会话）：**
```bash
openclacky agent --mode=auto_approve --path [repo dir] -c -m "[后续指令]"
```

**交互模式（需要人工确认）：**
```bash
openclacky agent --mode=confirm_safes --path [repo dir]
```

### 示例

#### 构建游戏
```bash
openclacky agent --mode=plan_only --path /projects/snake-game -m "用 HTML5 Canvas 构建贪吃蛇游戏，支持方向键控制、分数显示和游戏结束画面。"
openclacky agent --mode=auto_approve --path /projects/snake-game -m "计划已批准，开始实现。"
```

#### 构建网站
```bash
openclacky agent --mode=plan_only --path /projects/portfolio -m "用 Next.js 构建响应式个人作品集网站，包含首页、关于、项目和联系方式，支持暗色模式切换。"
openclacky agent --mode=auto_approve --path /projects/portfolio -m "计划已批准，开始实现。"
```

#### 构建 Agent
```bash
openclacky agent --mode=plan_only --path /projects/weather-agent -m "用 Python 构建一个 CLI Agent，输入城市名称后调用 OpenWeatherMap API，并通过 LLM 生成自然语言天气摘要。"
openclacky agent --mode=auto_approve --path /projects/weather-agent -m "计划已批准，开始实现。"
```

## License

MIT
