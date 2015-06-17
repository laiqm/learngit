# 一. 安装Git
	Windows：直接下载安装
	Mac：Xcode集成，xcode->Prefernces->Downloads->Command Line Tools->Install
	Linux:sude apt-get install git

# 二. 全局配置
    $ git config --global user.name "Your Name"
    $ git config --global user.email "email@example.com"

# 三. 初始化目录（版本库）
    $ git init

# 四. 基本命令汇总
    ## 添加或更新文件到仓库
    $ git add file1 [file2] ...
    ## 提交
    $ git commit -m "your comment" 
    ## 查看仓库当前状态
    $ git status
    ## 对比文件版本（显示格式(Unix通用diff格式)待进一步了解）
    $ git diff fileName 
    ## 获取命令帮助
    $ git --help [command]
    ## 查看提交历史
    $ git log [--pretty=oneline]
    ## 获取版本
    $ git reset --hard HEAD^(或 commit id，windows cmd下不支持^，用引号括起来)
    ## 查看文件内容
    $ cat fileName
    ## 查看命令操作历史(不仅提交历史，可以用于查询回退版本后最新版本号)
    $ git reflog
    ## 丢弃工作区修改，获取库里(暂存区有取暂存区)最新
    $ git checkout -- fileName
    ## 撤销暂存区内容
    $ git reset HEAD fileName




# 五. 相关概念
    Git中版本使用head表示。当前版本即是HEAD，上一个版本是HEAD^,上上一个是HEAD^^,多个写成HEAD~n
    Git包含工作区，暂存区，仓库，add操作实际是把工作区内容添加到暂存区，commit操作是把暂存区内容放到仓库里
