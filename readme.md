# 给命令行加别名

## 教程

- 当执行 `ls -al` 可设置别名简化输入：如
  - `la`
- 修改 `~/.bashrc` 加入
  - `alias la='ls -al'`



## 我的做法

1. 打开 `Git Bash` 并进入了 `vim ~/.bashrc` 文件

2. 在这个文件中输入了 `alias la='ls -al'` 并用 `:wq` 退出了文件 

3. 然后我输入了 `ls -al` 命令可以将目录下的信息显示出来，但是用 `la` 则出现了以下提示：

   ```
   bash: la: command not found
   ```

所以为什么没有找到这个 `la` 命名呢？是我漏掉了哪一步骤吗？

