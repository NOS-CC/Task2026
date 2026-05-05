# 2026春季学期实践周实践报告



## 学习资源链接 

[Git与远程仓库协作入门](https://www.bilibili.com/video/BV1d6XVYqEuy?vd_source=542e1e39b0a90f209166f30678b7c053) 

> 部分操作与AI协同完成


## 实践流程

1. 安装Git
    - 官网链接安装：[https://git-scm.com/install/windows](https://git-scm.com/install/windows)
    - 启动setup文件，按提示安装
2. 创建远程代码仓库
    - 打开GitHub账号，创建一个新的仓库
    - 仓库名称：Task2026
    - 仓库描述：2026春季学期实践周项目
    - 仓库设置：公开
    - 仓库链接：<https://github.com/NOS-CC/Task2026>
3.  配置Git环境
    - 设置用户名`git config --global user.name "NOS-CC"` 
    - 设置邮箱`git config --global user.email "nos1cc@qq.com"` 
    - 验证配置`git config --list`
4. 创建本地仓库
    - 创建本地目录Task2026
    - 创建本地仓库`git init`
    - 绑定本地仓库到远程仓库`git remote add origin https://github.com/NOS-CC/Task2026.git`
5. 获取PAT令牌
    - 进入Github账号设置
    - 点击"Developer settings"
    - 点击"Personal access tokens"
    - 点击"Generate new token"
    - 填写令牌描述，选择权限范围，点击"Generate token"
    - 复制令牌，保存到安全的地方
6. 上传本地测试代码
    - 在本地目录Task2026下创建一个测试文件test.py并编写代码
    - 暂存所有文件`git add *`
    - 提交所有文件`git commit -m "first commit"`
    - 推送所有文件到远程仓库`git push -u Task2026 main`