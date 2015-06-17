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
    $ git reset --hard HEAD^(或 commit id)
    ## 查看文件内容
    $ cat fileName
    ## 


# 五. 相关概念
    Git中版本使用head表示。当前版本即是HEAD，上一个版本是HEAD^,上上一个是HEAD^^,多个写成HEAD~n
