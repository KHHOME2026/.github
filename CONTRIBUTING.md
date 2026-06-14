# 贡献指南(CONTRIBUTING)

本指南适用于 KHHOME2026 组织内的所有仓库。请在参与前通读。

## 一、基本流程

1. **认领任务**:在仓库 Issues 里认领或新建 Issue,说明你要做什么。
2. **拉取最新代码**:
   ```bash
   git clone https://github.com/KHHOME2026/<仓库名>.git
   cd <仓库名>
   git checkout main
   git pull
   ```
3. **新建分支**(不要直接在 main 上改):
   ```bash
   git checkout -b feature/简短描述
   ```
4. **提交改动**(见下方提交规范)。
5. **推送并发起 Pull Request**:
   ```bash
   git push -u origin feature/简短描述
   ```
   然后在 GitHub 上对 `main` 发起 PR,关联相关 Issue。
6. **等待 Review**:至少 1 名审查者通过 + 检查通过后方可合并。

## 二、分支命名规范

| 前缀 | 用途 |
|------|------|
| `feature/` | 新功能 |
| `fix/` | 修复缺陷 |
| `docs/` | 文档 |
| `refactor/` | 重构 |
| `chore/` | 杂项/构建 |

示例:`feature/login-page`、`fix/null-pointer`。

## 三、提交信息规范(Conventional Commits)

格式:`<类型>: <简短描述>`

```
feat: 新增用户登录页面
fix: 修复空指针异常
docs: 更新部署说明
```

常用类型:`feat`、`fix`、`docs`、`style`、`refactor`、`test`、`chore`。

## 四、Pull Request 要求

- 标题简洁,说明本次改动目的。
- 描述里写清:改了什么、为什么、怎么测的。
- 关联相关 Issue(如 `Closes #12`)。
- 通过所有检查、至少 1 人 Review 后合并。
- 合并方式建议 **Squash and merge**,保持 main 历史整洁。

## 五、安全与保密(重要)

- **严禁提交任何密钥、令牌、密码、`.env` 文件**。
- 提交前自查:`git diff --staged`,确认没有敏感信息。
- 每个仓库都应有 `.gitignore` 排除 `temp/`、日志、本地配置、密钥文件。
- 若不慎提交了密钥,立即作废该密钥并通知 maintainer。

## 六、目录结构

每个项目的目录结构由该项目的 developer 决定,但建议保留:
- `README.md`:项目说明与运行方式。
- `docs/`:项目文档。
- `.gitignore`:务必排除临时文件与密钥。

## 七、遇到问题

- 技术讨论:在对应仓库的 Issues 提出。
- 权限/组织问题:联系 owners(@enochcxq)。
