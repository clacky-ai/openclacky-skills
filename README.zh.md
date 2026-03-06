# OpenClacky Skills

[English](README.md)

---

OpenClacky AI 编程 Agent — 在非交互式终端中自主完成所有开发任务，支持全栈开发、调试、重构、测试、部署等。

## 目录结构

```
code-skills/
  openclacky-code/
    _meta.json   # 平台元数据（ownerId、slug、version、publishedAt）
    SKILL.md     # 技能定义（YAML frontmatter + Markdown 指令）
```

## 快速开始

### 前置条件

- 安装 [openclacky](https://github.com/clacky-ai/open-clacky) CLI 工具

### 使用方式

**开始新任务：**
```bash
openclacky agent --mode=auto_approve --path [repo dir] -m "[任务描述]"
```

**继续上次会话：**
```bash
openclacky agent --mode=auto_approve --path [repo dir] -c -m "[后续指令]"
```

**附加图片（UI 设计稿 / Bug 截图）：**
```bash
openclacky agent --mode=auto_approve --path [repo dir] -m "[描述]" -i /path/to/screenshot.png
```

## 示例

### 修复 Bug
```bash
openclacky agent --mode=auto_approve --path /projects/myapp -c \
  -m "登录后跳转失败，报 404 错误，请排查并修复。"
```

### 构建全栈应用
```bash
openclacky agent --mode=auto_approve --path /projects/myapp \
  -m "用 Next.js、Tailwind CSS 和 PostgreSQL 构建任务管理应用，包含用户登录、任务列表 CRUD 和标签筛选，完成数据库 Schema、API 路由和前端页面。"
```

## License

MIT
