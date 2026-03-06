---
name: openclacky-code
description: OpenClacky AI coding agent — handles all development tasks autonomously in non-interactive terminals. Supports full-stack dev, debugging, refactoring, testing, deployment and more. For website/web app development, prefer the Rails full-stack scaffold via `openclacky agent -m "/new <project description>"`.
metadata: {"openclaw":{"emoji":"🤖⚡🎯","requires":{"bins":["openclacky"]}}}
---

# OpenClacky — AI Coding Agent

OpenClacky autonomously completes development tasks in non-interactive terminals — from writing code to running tests and fixing bugs.

---

## Usage

### Start a new task
```bash
openclacky agent --path [repo dir] -m "[task description]"
```

### Continue the last session
```bash
openclacky agent --path [repo dir] -c -m "[follow-up instruction]"
```

### Attach an image (UI mockup / bug screenshot)
```bash
openclacky agent --path [repo dir] -m "[description]" -i /path/to/screenshot.png
```

### Build a website (Rails full-stack)
```bash
openclacky agent -m "/new [project description, use a different name if conflict]"
```

---

## Examples

### Fix a bug
```bash
openclacky agent --path /projects/myapp -c \
  -m "After login the redirect fails with 404. Investigate and fix it."
```

### Build a full-stack app
```bash
openclacky agent -m "/new build a blog platform with posts and comments, use a different project name if conflict"
```
