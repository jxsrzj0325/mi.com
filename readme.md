### git
Git（读音为/gɪt/）是一个开源的分布式版本控制系统，可以有效、高速地处理从很小到非常大的项目版本管理。 也是Linus Torvalds为了帮助管理Linux内核开发而开发的一个开放源码的版本控制软件。

市面主流的项目管理软件 分为两大类
1. 集中式代码管理工具(svn) 10%
2. 分布式代码管理工具(git)  90%

代码管理工具的作用是用于管理项目的 源代码(你自己写的代码)
https://git-scm.com/

git是一个跨平台(操作系统)的项目管理工具

集中式的项目管理工具 代码集中存放在服务器(必须有网)
分布式项目管理工具 代码分布在各个位置 在有网络的情况时 进行 同一数据(和服务器进行同步)


### 基本操作
```bash
# 全局配置
$ git config --global user.name 'Zhang Jun'
$ git config --global user.email 'root@rootbk.cn'
```

### 本地仓库操作
### 准备好项目目录
1. 创建一个 .gitignore
2. 创建一个 readme.md
3. 在 .gitignore 放入需要忽略的目录
4. 初始化项目仓库 `$ git init`

# 本地仓库操作
```bash
$ git status   # 查看状态

$ git add .    # 将当前目录中所有的内容添加到本地仓库的暂存区

$ git commit -m 'message'  # 将当前暂存区的内容 提交到本地仓库

$ git log    # 查看提交日志

$ git reset --hard 提交id前6位   # 恢复到指定版本

$ git checkout filename  # 恢复文件
```

### 远程仓库操作


```bash
# 设置远程仓库的地址
$ git remote add origin https://gitee.com/jxsrzj/mi.com.git

# 将本地仓库推送到远程仓库
$ git push -u origin "master"

# 查看所有源
$ git remote 

# 查看远程仓库地址
$ git remote get-url origin


```