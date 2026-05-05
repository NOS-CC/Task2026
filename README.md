# 2026春季学期实践周实践报告

---
## 学习资源链接 

**Bilibili**: [Git与远程仓库协作入门](https://www.bilibili.com/video/BV1d6XVYqEuy?vd_source=542e1e39b0a90f209166f30678b7c053) 

> 部分操作与AI协同完成

---
## 实践流程

**1. 安装Git**
- 官网链接安装：[https://git-scm.com/install/windows](https://git-scm.com/install/windows)
- 启动setup文件，按提示安装

**2. 创建远程代码仓库**
- 打开GitHub账号，创建一个新的仓库
- 仓库名称：Task2026
- 仓库描述：2026春季学期实践周项目
- 仓库设置：公开
- 仓库链接：<https://github.com/NOS-CC/Task2026>

**3.  配置Git环境**
- 设置用户名`git config --global user.name "NOS-CC"` 
- 设置邮箱`git config --global user.email "nos1cc@qq.com"` 
- 验证配置`git config --list`

**4. 创建本地仓库**
- 创建本地目录`Task2026`
- 创建本地仓库`git init`
- 绑定本地仓库到远程仓库`git remote add origin https://github.com/NOS-CC/Task2026.git`

**5. 获取PAT令牌**
- 进入Github账号设置
- 点击`Developer settings`
- 点击`Personal access tokens`
- 点击`Generate new token`
- 填写令牌描述，选择权限范围，点击`Generate token`
- 复制令牌，保存到安全的地方

**6. 上传本地测试代码**
- 在本地目录Task2026下创建一个测试文件test.py并编写代码
- 暂存所有文件`git add *`
- 提交所有文件`git commit -m "first commit"`
- 推送所有文件到远程仓库`git push -u Task2026 main`
- 上传并提交修改记录，共3次
    - 第一次提交：![1st](/commits/commit-1.png)
    - 第二次提交：![2nd](/commits/commit-2.png)
    - 第三次提交：![3rd](/commits/commit-3.png)
    > 每次提交后都进行了push

---
## 提交说明

**1. 提交测试代码与 README.md 文件**
- 提交`test.py`与`README.md`文件到远程仓库
- 提交信息：`first commit`

**2. 提交新增内容**
- 提交修改后的的代码
- 新增`commits`文件夹，存放每次提交的截图
- 提交信息：`2nd commit`

**3. 提交新增内容**
- 提交新增的代码
- 提交新增的截图到`commits`文件夹
- 提交信息：`3rd commit`

---
## 遇到的问题与解决方法

>
> **Q1:** 第一次push时，远程仓库中文件与本地仓库中文件不一致，如何解决？
> 
> **A1:** 由于远程仓库中的文件为自带文件，并不需要，所以修改指令为`git push -u Task2026 main`提交覆盖即可
> 

---
## Git学习心得

初学Git时，我被各种命令和概念搞得晕头转向，尤其是分支、合并、冲突解决这些核心操作。第一次push代码就遇到了 "src refspec main does not match any" 的错误，后来又接连碰到网络连接问题、远程仓库冲突等障碍。

通过反复实践，我总结出几点体会：
- 要理解Git的三大区域——工作区、暂存区和版本库，这是掌握所有命令的基础。
- 遇到错误不要慌，仔细阅读提示信息，Git的错误提示其实很有帮助。
- 勤用`git status`和`git log`查看当前状态，能避免很多迷茫时刻。

最重要的是，Git是工具，不必死记硬背所有命令。掌握`add`、`commit`、`push`、`pull`、`branch`这几个核心命令就能满足日常需求，遇到复杂场景再查阅文档也不迟。多动手、多犯错、多总结，自然就能熟练运用了。