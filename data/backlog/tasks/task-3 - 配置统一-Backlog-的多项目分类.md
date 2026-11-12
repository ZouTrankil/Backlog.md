---
id: TASK-3
title: 配置统一 Backlog 的多项目分类
status: Done
assignee: []
created_date: '2026-11-12T14:02:00Z'
updated_date: '2026-11-12T14:03:00Z'
labels:
  - backlog
  - project-configuration
dependencies: []
type: chore
ordinal: 3000
---

## Description

<!-- SECTION:DESCRIPTION:BEGIN -->
统一任务库需要按工程维度筛选和归属任务。用户已确定四个项目：engine-data、back-monitor、channel、questdb-infra。配置应仅增加这四个有效项目值，并将现有 QuestDB 文档任务归入 engine-data，保持任务编号、状态和其他元数据不变。
<!-- SECTION:DESCRIPTION:END -->

## Acceptance Criteria
<!-- AC:BEGIN -->
- [x] #1 Backlog 配置仅包含 engine-data、back-monitor、channel、questdb-infra 四个项目值
- [x] #2 CLI 能以 --project engine-data 创建和筛选任务
- [x] #3 TASK-1 与 TASK-2 归属 engine-data，状态和验收记录保持不变
<!-- AC:END -->

## Implementation Plan

<!-- SECTION:PLAN:BEGIN -->
1. 在统一任务库配置四个用户指定项目值。2. 为已有 QuestDB 文档任务设置 engine-data。3. 创建并筛选一个临时任务验证 --project 行为，随后归档临时任务。4. 复核配置、任务归属和工作看板。
<!-- SECTION:PLAN:END -->

## Implementation Notes

<!-- SECTION:NOTES:BEGIN -->
已通过 CLI 创建带 project=engine-data 的临时任务并用 --project engine-data 筛选；临时任务 TASK-4 已归档。当前嵌套任务库在读取其它分支时会输出路径水合警告，但当前分支的配置、任务编辑和筛选均成功。
<!-- SECTION:NOTES:END -->

## Final Summary

<!-- SECTION:FINAL_SUMMARY:BEGIN -->
已启用四个统一项目分类：engine-data、back-monitor、channel、questdb-infra，并将 TASK-1、TASK-2 归入 engine-data。已验证带项目字段的创建和筛选；用于验证的 TASK-4 已归档。
<!-- SECTION:FINAL_SUMMARY:END -->
