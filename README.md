# git
Git（读音为/gɪt/）是一个开源的分布式版本控制系统，可以有效、高速地处理从很小到非常大的项目版本管理。 也是Linus Torvalds为了帮助管理Linux内核开发而开发的一个开放源码的版本控制软件。

目前市面主流的代码管理工具 有两种
1. 集中式代码管理(svn) 3%
2. 分布式代码管理(git) 96%

项目(源代码)管理工具 主要用于管理开发环境的源码

git官网:
https://git-scm.com/
git是一个跨平台的版本管理工具(windows linux unix osx)

### git基本操作
#### 全局用户配置
```bash
### 全局用户设置 每台电脑只需要执行一次
$ git config --global user.name 'Zhang Jun'
$ git config --global user.email 'root@rootbk.cn'
```

1. 项目构建 在项目根目录(README.md .gitignore)
2. 在项目根目录执行`$ git init` 来初始化本地仓库
3. 填写git忽略列表(.gitignore)
4. 初始化项目 `$ npm init -y`

### git指令
```bash
# 查看状态
$ git status      

# 添加管理(将文件或目录添加到本地仓库的暂存区)
$ git add filename  # 将指定的文件添加到暂存区
$ git add path/     # 将指定的目录添加到暂存区
$ git add .         # 将当前目录所有内容(文件和文件夹)添加到暂存区
$ git add --all     # 将当前目录所有内容(文件和文件夹)添加到暂存区

# 将文件移出暂存区
$ git rm --cached filenamed

# 将暂存区的内容提交到本地仓库
$ git commit -m 'msg'

# 查看提交日志
$ git log

# 恢复历史版本
$ git reset --hard hash(前六位)

# 查看帮助
$ git --help

# 恢复文件
$ git checkout filename
```


### https://github.com/
它是全球最大的IT开源社区 提倡编程社交
它是全球最大的同性交友网站

github 它和 git 是没有关系的
但是它提供了免费的git仓库(public)
github也提供了私有仓库 收费

开源大法好
非常多成功的开源项目 诞生于github
jQuery
Bootstarp
Vue
React
Angular
ANTD
...

2018年10月 微软收购github
收购完成的当天宣布 私有仓库免费

### Git远程仓库操作
```bash
# 添加远程仓库地址 并取名 origin
$ git remote add origin https://github.com/jxsrzj0325/mi.com.git

# 创建并切换到 main 分支
$ git branch -M main

# 将本地仓库推送到远程仓库
$ git push -u origin main

# 克隆远程仓库(从无到有)
$ git clone https://github.com/jxsrzj0325/mi.com.git

# 从远程仓库拉取分支(更新)
$ git pull origin master
```

### 分支操作
```bash
# 查看分支
$ git branch

# 创建分支
$ git branch 分支名

# 切换分支
$ git checkout 分支名
```