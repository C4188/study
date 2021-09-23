# git简易教程 #
> 创建一个Git可以管理的仓库
```{}
git init
```

> 将文件readme.txt添加到Git的暂存区
```{}
git add readme.txt
```

> 将文件提交到Git仓库
```{}
git commit -m "此次提交的说明"
```

> 查看仓库当前的状态
```{}
git status
```

> 查看一个文件的具体修改内容
```{}
git diff readme.txt
```

> 查看提交的历史纪录
```{}
git log
git log --pretty=oneline
```

> 回退到上一个版本
```{}
git reset --hard HEAD^
git reset --hard HEAD^^
```

> 回退到往上100个版本
```{}
git reset --hard HEAD~100
```

> 查看执行的Git命令记录
```{}
git reflog
```

> 丢弃工作区中对文件readme.txt的修改
- 一种是 readme.txt 自修改后还没有被放到暂存区，则撤销修改就回到版本库一模一样的状态
- 一种是 readme.txt 已经添加到暂存区后，又做了修改，则撤销后回到添加到暂存去后的状态
```{}
git checkout -- readme.txt
```

