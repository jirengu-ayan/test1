# 撤销文件过程中遇到的问题

## 教程

#### 取消变动的暂存

`git reset HEAD <file>` 来取消暂存。



#### 撤销对文件的修改

`git checkout -- [file]` 用来撤销文件的i修改。



#### 步骤：

1. `touch a.md`

2. `echo "ayan" > a.md`

   `git status` a.md 未被追踪

3. `git add a.md`

   `git status ` a.md 被追踪

4. `git reset HEAD a.md`

5. `git checkut -- a.md`

6. `cat a.md`

   `git status` a.md 未被追踪

   

## 我的做法

我是用 Git Bash 按照步骤输入的，然后在第五步的时候出现了错误：

```bash
$ git checkout -- a.md
error: pathspec 'a.md' did not match any file(s) known to git
```

这是为什么呢？

而且在过程中还遇到了下面这个错误：

```bash
$ git reset HEAD a.md
fatal: ambiguous argument 'HEAD': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'
```

