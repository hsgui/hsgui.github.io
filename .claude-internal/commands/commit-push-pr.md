# Commit, Push and Create PR

执行以下步骤完成代码提交和 PR 创建：

## 1. 检查当前状态
运行 `git status` 和 `git diff` 查看所有变更。

## 2. 创建 Commit
- 分析所有变更内容
- 生成简洁的 commit message（中文或英文，根据变更内容决定）
- 将所有相关文件添加到暂存区
- 创建 commit，message 结尾添加：
  ```
  Co-Authored-By: Claude <noreply@anthropic.com>
  ```

## 3. Push 到远程
- 检查当前分支是否有上游分支
- 如果没有，使用 `git push -u origin <branch>` 推送并设置上游
- 如果有，直接 `git push`

## 4. 创建 Pull Request
- 使用 `gh pr create` 创建 PR
- PR 标题应简洁描述变更
- PR body 格式：
  ```
  ## Summary
  <1-3 个要点描述变更>

  ## Test plan
  <测试计划或验证步骤>

  🤖 Generated with [Claude Code](https://claude.com/claude-code)
  ```

## 5. 返回结果
完成后返回 PR 的 URL 给用户。
