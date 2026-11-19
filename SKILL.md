---
name: novel-writing
description: 小说与故事创作全流程路由。写小说、写故事、短篇、长篇、连载、章节、大纲、人物设定、世界观、去AI味、改稿、审阅、扫描拆解、封面、导入素材时使用。
---

# 小说创作路由

原 oh-story 系列 12 个分技能与 webnovel 插件已归档，不再常驻注入。按任务类型读取对应原文，读完按其流程执行。

## 路由表

| 任务 | 读取文件 |
| --- | --- |
| 短篇：拆解参考作品 | `D:/Claude/配置/.claude/skills/oh-story-claudecode/.agents/skills/story-short-analyze/SKILL.md.disabled` |
| 短篇：扫描素材 | `.../story-short-scan/SKILL.md.disabled` |
| 短篇：正式写作 | `.../story-short-write/SKILL.md.disabled` |
| 长篇：拆解参考作品 | `.../story-long-analyze/SKILL.md.disabled` |
| 长篇：扫描素材 | `.../story-long-scan/SKILL.md.disabled` |
| 长篇：正式写作 | `.../story-long-write/SKILL.md.disabled` |
| 通用入口/流程说明 | `.../story/SKILL.md.disabled` |
| 审阅与修改 | `.../story-review/SKILL.md.disabled` |
| 去 AI 味 | `.../story-deslop/SKILL.md.disabled` |
| 封面生成 | `.../story-cover/SKILL.md.disabled` |
| 导入外部素材 | `.../story-import/SKILL.md.disabled` |

基础环境搭建仍保留为独立技能 `story-setup`，需要时直接调用。

`...` 均为 `D:/Claude/配置/.claude/skills/oh-story-claudecode/.agents/skills` 的简写。

## 执行约定

1. 先判断是短篇还是长篇、是拆解还是写作，再读对应文件；不要一次读多个。
2. 读完严格按原文流程执行，不自行简化步骤。
3. 涉及具体项目时，遵守项目 CLAUDE.md 的命名与存档规则。
