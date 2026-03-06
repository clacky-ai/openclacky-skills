# OpenClacky Skills

[English](README.md)

---

OpenClacky AI 编程 Agent — 在非交互式终端中自主完成所有开发任务，支持全栈开发、调试、重构、测试、部署等。开发网站/Web 应用时，推荐使用 Rails 全栈脚手架：`openclacky agent -m "/new <项目描述>"`。

## 目录结构

```
skills/
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
openclacky agent --path [repo dir] -m "[任务描述]"
```

**继续上次会话：**
```bash
openclacky agent --path [repo dir] -c -m "[后续指令]"
```

**附加图片（UI 设计稿 / Bug 截图）：**
```bash
openclacky agent --path [repo dir] -m "[描述]" -i /path/to/screenshot.png
```

**构建网站（Rails 全栈）：**
```bash
openclacky agent -m "/new [项目描述，如有冲突请使用不同的项目名]"
```

## 示例

### 修复 Bug
```bash
openclacky agent --path /projects/myapp -c \
  -m "登录后跳转失败，报 404 错误，请排查并修复。"
```

### 构建全栈应用
```bash
openclacky agent -m "/new build a blog platform with posts and comments, use a different project name if conflict"
```

## License

MIT
