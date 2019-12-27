# git 本地仓库
使用github程序 >> install command line tool 来安装git
```配置
git config --global user.name 你的英文名
git config --global user.email 你的邮箱
git config --global push.default simple
git config --global core.quotepath false
git config --global core.autocrlf input
```

新建目录 >> 进入 >> git init

git add 路径 //选择哪些变动是需要提交的
.gitignore 是设置不需要提交的文件 //常见有::node_modules::; ::.DS_Store::; ::.idea::; ::.vscode::
git status 查看已经提交的文件
git status -sb s查看哪些文件有冲突
git commit -m “字符串”
git commit -v
git log 查看已提交更新的版本
```
git add .
git commit -v
```
git reset —hard a2bv7r //commit的版本号值
**⚠️运行 reset 命令前，一定要确保重要代码已经提交（commit）了，否则后悔莫及**
 git reflog	查看所有更新和回滚的版本

git checkout master  //切换到主线
git checkout X //切换到X分支
git branch X //创建分支X
git stash //通灵术

git merge X //合并分支
git branch -d X //合并完删除无用分支X
再次commit 可以不写 -m ‘message’