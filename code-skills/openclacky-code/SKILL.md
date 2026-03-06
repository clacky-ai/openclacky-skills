---
name: openclacky-code
description: OpenClacky AI coding agent — handles all development tasks autonomously in non-interactive terminals. Supports full-stack dev, debugging, refactoring, testing, deployment and more.
metadata: {"openclaw":{"emoji":"🤖⚡🎯","requires":{"bins":["openclacky"]}}}
---

# OpenClacky — AI Coding Agent

OpenClacky autonomously completes development tasks in non-interactive terminals — from writing code to running tests and fixing bugs.

---

## Usage

### Start a new task
```bash
openclacky agent --mode=auto_approve --path [repo dir] -m "[task description]"
```

### Continue the last session
```bash
openclacky agent --mode=auto_approve --path [repo dir] -c -m "[follow-up instruction]"
```

### Attach an image (UI mockup / bug screenshot)
```bash
openclacky agent --mode=auto_approve --path [repo dir] -m "[description]" -i /path/to/screenshot.png
```

---

## Examples

### Fix a bug
```bash
openclacky agent --mode=auto_approve --path /projects/myapp -c \
  -m "After login the redirect fails with 404. Investigate and fix it."
```

### Build a full-stack app
```bash
openclacky agent --mode=auto_approve --path /projects/myapp \
  -m "Build a task management app with Next.js, Tailwind CSS, and PostgreSQL. Include user login, task list with CRUD, and tag-based filtering. Set up the database schema, API routes, and frontend pages."
```
