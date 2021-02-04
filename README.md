# 道可道

![Super Linter](https://github.com/xinetzone/xinetzone-actions/workflows/xinetzone/badge.svg)

## GitHub Actions

参考：[GitHub Actions](https://docs.github.com/cn/free-pro-team@latest/actions)

**运行器**是安装了 [GitHub Actions 运行器应用程序](https://github.com/actions/runner) 的服务器。您可以使用 [GitHub 托管的运行器](https://docs.github.com/cn/actions/automating-your-workflow-with-github-actions/virtual-environments-for-github-hosted-runners) 或 [托管您自己的运行器](https://docs.github.com/cn/actions/automating-your-workflow-with-github-actions/about-self-hosted-runners)。运行器将侦听可用的**任务**，每次运行一个任务，并将进度、日志和结果报告回 GitHub。对于 GitHub 托管的运行器，工作流程中的每项任务都会在一个新的虚拟环境中运行。

GitHub 提供使用 Linux、Windows 和 macOS 操作系统的运行器。

## [工作流程运行的状态徽章](https://docs.github.com/cn/actions/guides/about-continuous-integration#status-badges-for-workflow-runs)

状态徽章显示工作流程目前状态是失败还是通过。添加状态徽章的常见位置是仓库的 `README.md` 文件，但也可将其添加到您喜欢的任何网页。默认情况下，徽章显示默认分支的状态。您也可以在 URL 中使用 branch 和 event 查询参数显示特定分支或事件运行的工作流程状态。

如果您的工作流程使用 `name` 关键词，则必须按名称引用工作流程。如果工作流程名称包含空格，您需要将空格替换为 URL 编码字符串 `%20`。有关 `name` 关键词的更多信息，请参阅“[GitHub Actions 的工作流程语法](https://docs.github.com/cn/articles/workflow-syntax-for-github-actions#name)”。

```sh
https://github.com/<OWNER>/<REPOSITORY>/workflows/<WORKFLOW_NAME>/badge.svg
```

或者，如果工作流程没有 `name`，则必须使用相对于仓库根目录的文件路径引用工作流程文件。

```sh
https://github.com/<OWNER>/<REPOSITORY>/workflows/<WORKFLOW_FILE_PATH>/badge.svg
```