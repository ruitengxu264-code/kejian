# Git Version Control Basics / Git 版本控制入门

**Course / 课程**: Empirical Methods in Economics and Business  2026 Spring
**Theme / 主题**: A practical introduction to Git for research workflows / 面向研究工作流的 Git 实用入门

## Why Git? / 为什么要学 Git？

Without version control, research files often become a mess.没有版本控制时，研究文件很容易变得混乱。

- `paper_final.docx`
- `paper_final_v2.docx`
- `paper_final_v2_REAL_FINAL.docx`

Git gives us a better workflow.Git 提供了一种更清晰、更可追溯的工作方式。

- every change has a record每一次修改都有记录
- we can go back to an earlier version我们可以回到任意历史版本
- collaboration becomes safer多人协作时更不容易互相覆盖
- code, notes, and results become easier to manage
  代码、笔记和结果更容易统一管理

In short, Git is the "time machine" of research projects.
简而言之，Git 就是研究项目的“时光机”。

## What Git Tracks / Git 适合管理什么？

Git is best for:Git 最适合跟踪以下内容：

- code files: `.py`, `.R`, `.do`, `.jl`, `.m`代码文件：`.py`、`.R`、`.do`、`.jl`、`.m`
- notebooks and markup files: `.ipynb`, `.md`, `.qmd`notebook 和标记文档：`.ipynb`、`.md`、`.qmd`
- small configuration files小型配置文件
- writing projects
  论文和写作项目

Git is usually not ideal for:Git 通常不适合直接管理：

- very large raw datasets非常大的原始数据文件
- temporary output files临时输出文件
- compiled files such as `.pdf`, `.html`, `.log`, `.aux`
  编译生成文件，如 `.pdf`、`.html`、`.log`、`.aux`

These files should often be excluded with `.gitignore`.
这类文件通常应该通过 `.gitignore` 排除。

## Core Ideas / 核心概念

### Repository / 仓库

A repository is a project folder with version history.
仓库就是一个带有版本历史记录的项目文件夹。

### Commit / 提交

A commit is a saved checkpoint with a message explaining what changed.
一次 commit 就是一个带说明文字的“版本检查点”。

### Remote / 远程仓库

A remote is the online copy of the repository, such as on Gitee or GitHub.
远程仓库是仓库的在线版本，例如 Gitee 或 GitHub 上的仓库。

### Branch / 分支

A branch is a separate line of work. Beginners can start on the main branch and learn branching later.
分支表示一条独立的开发线路。初学者完全可以先在主分支上工作，之后再学习分支协作。

## The Minimum Useful Workflow / 最小可用工作流

```bash
git status
git add .
git commit -m "describe your change"
git push
```

What these commands do:这些命令的作用分别是：

- `git status`: shows what changed`git status`：查看哪些文件发生了变化
- `git add .`: stages changes for the next commit`git add .`：把改动加入下一次提交
- `git commit -m "..."`: creates a version checkpoint`git commit -m "..."`：创建一个带说明的版本记录
- `git push`: sends local commits to the remote repository
  `git push`：把本地提交推送到远程仓库

## A Better Everyday Workflow / 一个更稳妥的日常工作流

For research projects, this is often safer:
对于研究项目来说，下面这种做法通常更稳妥：

```bash
git status
git add code/02_analysis.do notes/summary.md
git commit -m "fix: use robust standard errors in baseline regression"
git push
```

This is better than blindly using `git add .` because you stay aware of what you are committing.
这比无脑使用 `git add .` 更好，因为你会清楚自己到底提交了哪些内容。

## Typical Student Workflow in VS Code / 学生在 VS Code 中的典型流程

1. Open your project folder in VS Code.在 VS Code 中打开你的项目文件夹。
2. Make one small, meaningful change.做一个小而明确的修改。
3. Run `git status` in the terminal.在终端中运行 `git status`。
4. Stage the files you want to save.把你想保存的文件加入暂存区。
5. Write a clear commit message.写一个清楚的 commit message。
6. Push to Gitee or GitHub.
   推送到 Gitee 或 GitHub。

If you do this regularly, your work becomes much easier to track and explain.
如果你能持续这样做，项目过程就会更容易追踪、复现和解释。

## Useful Commands / 常用命令

### Check the current state / 查看当前状态

```bash
git status
```

### See what changed / 查看改动内容

```bash
git diff
```

### Stage one file / 暂存单个文件

```bash
git add script.do
```

### Stage all changes in the current folder / 暂存当前目录中的改动

```bash
git add .
```

### Commit with a message / 带说明地提交

```bash
git commit -m "add data cleaning steps for firm panel"
```

### Push to the remote repository / 推送到远程仓库

```bash
git push
```

### Pull the newest remote changes / 拉取远程最新改动

```bash
git pull
```

### View recent history / 查看最近的提交记录

```bash
git log --oneline -5
```

## Good Commit Messages / 如何写好的提交说明

Bad examples / 不好的例子：

- `update`
- `fix`
- `changes`

Better examples / 更好的例子：

- `add notebook for Stata basics`
- `fix variable label typo in survey cleaning script`
- `revise DID example and add clustered standard errors`

A good commit message should help your future self understand the purpose of the change.
一个好的 commit message，应该能帮助未来的你快速理解“这次改动是为了什么”。

## A Simple Research Example / 一个简单的研究场景例子

Suppose you changed a Stata file after discovering heteroskedasticity:
假设你在发现异方差问题之后，修改了一个 Stata 文件：

```bash
git add code/02_analysis.do
git commit -m "fix: switch to robust SE after heteroskedasticity test"
git push
```

This is much better than editing the file and hoping you will remember what happened later.
这显然比“改完文件然后寄希望于自己以后还记得为什么改”要好得多。

## Git and Reproducible Research / Git 与可重复研究

Git works especially well with a clean project structure:Git 和清晰的项目结构搭配使用时效果最好：

- `data/` for datasets`data/` 用来放数据
- `code/` for scripts`code/` 用来放脚本
- `output/` for tables and figures`output/` 用来放表格和图片
- `notes/` for research notes
  `notes/` 用来放研究笔记

Recommended principles:推荐遵循的基本原则：

- raw data should be read-only when possible原始数据尽量保持只读
- scripts should be saved in logical order脚本尽量按分析逻辑保存和命名
- outputs should be reproducible from code输出结果应尽量由代码自动再生成
- Git should track the evolution of the project
  Git 应用于记录项目的演进过程

## Common Mistakes to Avoid / 常见错误

- Do not commit random temporary files.不要把杂乱的临时文件提交进仓库。
- Do not wait until the end of the semester to commit.不要等到学期末才一次性提交。
- Do not use commit messages that say nothing.不要写没有信息量的提交说明。
- Do not mix many unrelated changes into one huge commit.不要把很多无关改动塞进一个超大的 commit。
- Do not treat Git as backup only. It is also a thinking and documentation tool.
  不要只把 Git 当备份工具，它也是整理思路和记录过程的工具。

## Suggested First Habit / 建议你先养成的第一个习惯

1. finish one small task完成一个小任务
2. run `git status`运行 `git status`
3. commit with a meaningful message写一个有意义的提交说明并提交
4. push
   推送到远程仓库

If you repeat this pattern, your project history will stay clean and useful.
如果你反复坚持这个模式，你的项目历史就会保持清晰而且有用。

## One-Line Summary / 一句话总结

Git helps you save, explain, recover, and share the history of your research work.
Git 能帮助你保存、解释、恢复并分享你的研究工作历史。
