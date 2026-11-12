---
id: TASK-5
title: 撤回统一 Backlog 的多项目分类
status: Done
assignee: []
created_date: '2026-11-12T14:13:00Z'
updated_date: '2026-11-12T14:14:00Z'
labels:
  - backlog
  - rollback
dependencies: []
type: chore
ordinal: 4000
---

## Description

<!-- SECTION:DESCRIPTION:BEGIN -->
用户决定按工程拆分独立 Backlog，不再使用当前数据任务库中的多项目分类。需要移除四个项目配置、清空 TASK-1 与 TASK-2 的 project 字段，并删除仅为验证创建的已归档 TASK-4；保留 TASK-3 作为历史记录并标明已撤回。
<!-- SECTION:DESCRIPTION:END -->

## Acceptance Criteria
<!-- AC:BEGIN -->
- [x] #1 Backlog 配置不再定义 projects 列表
- [x] #2 TASK-1 与 TASK-2 不含 project 字段，状态和验收记录保持不变
- [x] #3 仅用于验证的 TASK-4 被永久删除，TASK-3 留有撤回说明
<!-- AC:END -->

## Implementation Plan

<!-- SECTION:PLAN:BEGIN -->
1. 清空 TASK-1 与 TASK-2 的 project 字段。2. 删除仅用于验证的已归档 TASK-4，并在 TASK-3 记录撤回原因。3. 移除配置中的 projects 列表。4. 复核配置与历史任务状态。
<!-- SECTION:PLAN:END -->

## Implementation Notes

<!-- SECTION:NOTES:BEGIN -->
已清空 TASK-1 与 TASK-2 的 project 字段，删除 TASK-4，并移除 config.yml 的 projects 列表。
<!-- SECTION:NOTES:END -->

## Final Summary

<!-- SECTION:FINAL_SUMMARY:BEGIN -->
已撤回统一多项目分类。当前数据任务 Backlog 不再配置 projects，TASK-1 与 TASK-2 恢复为未归属项目状态，TASK-4 已删除，TASK-3 保留撤回记录。
<!-- SECTION:FINAL_SUMMARY:END -->
