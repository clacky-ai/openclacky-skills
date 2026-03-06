---
name: openclacky-code
description: openclacky agent can do all things related to code
metadata: {"openclaw":{"emoji":"🤖⚡🎯","requires":{"bins":["openclacky"]}}}
---

# Openclacky

## Commands

**Plan:**
```
openclacky agent -m "开发贪吃蛇"
```

**Build (new session):**
```
openclacky agent --mode=auto_approve --path [repo dir] -m "/new"
```

**Build (continue session):**
```
openclacky agent --mode=auto_approve --path [repo dir] -c -m "[follow-up instruction]"
```

**Interactive (when user wants to supervise):**
```
openclacky agent --mode=confirm_safes --path [repo dir]
```

## Examples
### 加一个ruby全栈

### Build a game
```
openclacky agent --mode=plan_only --path /projects/snake-game -m "Build a Snake game with HTML5 Canvas, arrow key controls, score display, and game over screen."
openclacky agent --mode=auto_approve --path /projects/snake-game -m "Plan approved. Implement it."
```

### Build a website
```
openclacky agent --mode=plan_only --path /projects/portfolio -m "Build a responsive personal portfolio site with Next.js: home, about, projects, and contact sections. Dark mode toggle."
openclacky agent --mode=auto_approve --path /projects/portfolio -m "Plan approved. Implement it."
```

### Build an agent
```
openclacky agent --mode=plan_only --path /projects/weather-agent -m "Build a CLI agent in Python that takes a city name, calls OpenWeatherMap API, and replies with a natural language weather summary using an LLM."
openclacky agent --mode=auto_approve --path /projects/weather-agent -m "Plan approved. Implement it."
```