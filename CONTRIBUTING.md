# 贡献指南（CONTRIBUTING）

本仓库采用 **GitHub Flow** 分支模型。以下规则由分支保护 + CI 强制执行，不是建议。

## 1. 分支模型

- `main` 永远保持可发布状态，**禁止直接 push**（分支保护已封锁）。
- 任何改动（代码 / 文档 / 设计）必须从最新 `main` 切出特性分支：
  - 功能：`feature/xxx`
  - 修复：`fix/xxx`
  - 文档：`docs/xxx`
- 改动完成 → push 特性分支 → 开 PR → 评审通过 + CI 通过 → 合并回 `main`。

## 2. 提交规范（Conventional Commits）

格式：`<type>: <摘要>`

常用 type：`feat`（功能）/ `fix`（修复）/ `docs`（文档）/ `style`（格式）/ `refactor`（重构）/ `test`（测试）/ `chore`（杂项）

示例：

    docs: 落地协作规范强制文件
    fix: 修复热力图日期不刷新

## 3. PR 要求

- 按 PR 模板填写：变更目的、设计依据、测试方式。
- 至少 1 个审批；核心模块需 CODEOWNERS 中指定的 owner 审批。
- CI（`ci/quality`）必须通过。
- 评审意见必须全部解决（Resolve conversation）后才能合并。
- 合并采用 squash merge，保持 `main` 历史线性、每个 commit 可独立说明。

## 4. 设计先行

- 架构级 / 影响面大的改动，先在 `docs/design/` 提交设计文档（ADR）并作为 PR 评审通过，再开实现 PR。
- PR 模板中的「设计依据」字段必填。

## 5. 红线

- 禁止直接 push 到 `main`、禁止 force push、禁止删除保护分支。
- 禁止提交编辑器注入的元数据（如 `data-page-node-id`，CI 会拦截）。
- 禁止硬编码密钥 / token / 密码（CI 会扫描）。
