# 参与 Cola Pages

通过分支和 Pull Request（PR）提交修改，便于查看差异和保留修改说明。

## 本地准备

```bash
git clone https://github.com/StephanieLIzy/cola-pages.git
cd cola-pages
git switch -c docs/describe-change
```

已有本地仓库时，先切换到 `main`，确认没有未提交的修改，再执行 `git pull --ff-only`，最后创建新分支。请为新分支使用能描述修改内容的名称。

## 提交修改

1. 在分支中完成一项清楚、完整的修改。
2. 用 `git diff` 检查内容；文档中的链接和命令应与实际文件一致。
3. 用 `git add <文件路径>` 暂存相关文件，再运行 `git diff --cached` 检查将提交的内容。
4. 执行 `git commit -m "docs: describe the change"`，然后用 `git push -u origin <分支名>` 推送。
5. 在 GitHub 创建以 `main` 为目标的 PR，说明修改原因、内容和验证方式。
6. 确认差异和检查结果后合并 PR。

## 验证与敏感信息

- 文档修改：检查 Markdown 显示、相对链接和命令是否正确。
- 若后续增加可运行代码，请同时说明启动方式和相应的验证步骤。
- 不要提交 API 密钥、访问令牌、密码或其他私人信息。
