# KHHOME2026

> 团队代码与文档协作空间。

## 这是什么
KHHOME2026 是团队用于上传、维护代码与文档的 GitHub 组织。所有项目以**多仓库**方式管理,每个项目一个独立仓库。

## 协作约定(适用于所有仓库)
- 统一的贡献流程见 [CONTRIBUTING](https://github.com/KHHOME2026/.github/blob/main/CONTRIBUTING.md)。
- 一律走 **Pull Request** 合并,`main` 分支受保护,禁止直接推送。
- 提交信息建议遵循 Conventional Commits(`feat:` / `fix:` / `docs:` 等)。

## 团队与权限
| 团队 | 权限 | 说明 |
|------|------|------|
| owners | 组织管理 | 管理组织、计费、成员 |
| maintainers | maintain | 管理仓库、合并 PR、配置分支保护 |
| developers | write | 推送分支、发起 PR |

## 新建仓库怎么做
1. 由 maintainer 在组织内创建仓库(默认 **Private**)。
2. 创建后运行分支保护脚本保护 `main`。
3. 仓库内目录结构由该项目的 developer 自行决定。

## 安全红线
- **严禁提交任何密钥/凭证**(API key、`.env`、令牌等)。
- 内部项目仓库一律设为 **Private**。
