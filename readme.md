# readme文档
- 项目说明文档
- 一般都与项目放一起

# git操作

## 初始化版本库
- git init
- 初始化成功后，目录后面有(master)
- 初始化成功后当前目录下有个影藏文件.git(不用管，知道有就行，不要操作)

## 工作区
- 持有实际文件
- 我们平时增删改查的文件都是工作区的内容

## 暂存区

- 可以理解为我们看不到的一个地方
- 本地仓库的一个主要组成部分

## 本地仓库
- 可以理解为我们看见的地方
- 也是存在于用户电脑中的
- 用于存储项目代码及版本项目记录等信息

## 提交到暂存区
- git add 文件名
- 将工作区的变动提交到暂存区
- git add .将所有变动提交到暂存区

## 查看工作区和暂存区的状态
- git status
- 查看工作区和暂存区的状态(增删改)

## 提交到本地仓库
- git commit -m '提交注释'
- 将代码提交到本地仓库
- git status 查看状态提升:工作区是干净的，没有任何东西

## 本地操作关键步骤
1. git init(第一次需要)
2. git add .
3. git commit -m '注释'

## 查看日志
- git log 查看完整日志
- git reflog 查看简单日志

# 版本回退
- git reset --hard HEAD^ 回退到上一个版本
- git rest --hard 版本
- 注意先把当前的代码提交

## 修改变动
- gif diff 文件名
- 会列出改文件前后的差异

## 创建远程文件仓库
- 进入 github官网
- 创建一个新的远程从仓库

## 将本地仓库与远程仓库关联
- git remote add origin 你的远程地址
- git remote -v 查看本地仓库关联的远程地址

## 将本地仓库提交到远程仓库关联
- git push -u origin master 第一次 提交到远程
- git push 将本地仓库提交到远程仓库
- -u origin master 设置默认的提交地址

## 修改关联的远程仓库地址
- git remote rm origin
- git remote add origin ssh地址

## 更新代码
- 确保自己的工作区的代码先提交到本地仓库
- 然后在从远程到本地
- git clone 远程仓库地址  克隆代码到本地

## 其他人修改
- 你好呀
- 你好你好

## 分支操作
- git branch 查看当前所有分支
- 当前分支名有一个星号
- git branch 分支名 创建一个分支
- git checkout 分支名 切换分支
- git merge 分支名 合并某分支到当前分支
- git branch -d 分支名 删除某分支
- git push origin 分支名

## fetch和pull的区别
1. 他们都用于从远程更新到本地
2. fetch不会自动合并到当前分支(不会merge)
3. pull会自动合并到当前分支(会merge)

## test分支
- 添加内容。。。。
