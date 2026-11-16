# SYKI 语音标注审核

这个仓库只提供审核网页，不包含语音、标注或审核结果。审核员需要先获得私有数据仓库的协作者权限，并使用自己的 GitHub 账号令牌。

网页使用 GitHub API 读取分配任务的音频、保存审核结果。GitHub 适合小规模协作试用；仓库的写入权限并不能提供严格的逐条权限隔离。

## 连接步骤

1. 仓库所有者先邀请审核员加入私有数据仓库，审核员接受邀请。
2. 每位审核员创建自己的 [GitHub 个人访问令牌](https://github.com/settings/tokens)。仓库所有者可使用只授权数据仓库 Contents 读写的 fine-grained 令牌；其他仓库协作者可能需要带 `repo` 权限的 classic 令牌。
3. 打开 [审核网页](https://zirrtu.github.io/syki-annotation-review/)，输入自己的令牌。令牌仅保存在当前页面内存中，刷新后需重新输入；不要将令牌发给其他人。

GitHub 的 classic `repo` 令牌权限较宽，也能访问令牌持有人有权访问的其他私有仓库。建议审核员使用没有其他敏感仓库的独立账号和短期令牌，审核结束后撤销。了解更多：[GitHub 令牌说明](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)。
