# TODO: Personal `.claude/` Template

Future plan for building a personal `.claude/` configuration template, based on Nav Toor's action guide.

> Source: [怎么开始搭建 — 非著名程序员 (知乎)](https://zhuanlan.zhihu.com/p/2023391486331430509)

## 1. Directory structure

- [ ] Create the top-level `.claude/` directory layout:
  - [ ] `CLAUDE.md` — global configuration at the top level
  - [ ] `skills/` — skills directory
  - [ ] `hooks/` — hooks directory
  - [ ] `.mcp.json` — external integrations (MCP) config

## 2. Write `CLAUDE.md` (structured, not a wall of text)

Write it like an engineering doc, in this order:

- [ ] Project architecture first
- [ ] Naming conventions and coding standards
- [ ] Boundaries — which files must not be touched, which patterns must be followed
- [ ] Routing logic — which situation triggers which workflow
- [ ] Keep it under **150 lines**
- [ ] Update it **weekly** as the workflow evolves

## 3. Skills — start with five high-value categories

- [ ] **Domain analyzer** — handles the data types you touch most often
- [ ] **Code review enforcer** — checks team-specific patterns
- [ ] **Doc generator** — generates docs in the team's format and tone
- [ ] **Deployment workflow** — handles the CI/CD pipeline end to end
- [ ] **Test automation** — writes and runs tests according to your testing philosophy

## 4. Hooks — at least three

- [ ] **Pre-commit hook** — intercepts commits containing secret/credential files
- [ ] **Bash safety guard** — blocks dangerous commands
- [ ] **Plan review gate** — requires human approval before large changes

> These three hooks convey more production awareness than a year of commit history.
