## github

+ repository（仓库）
  + 创建
  + .gitignore(不想让git管理这个文件，让git忽略这些文件)
  + ssh设定 生成 ssh -keygen -t -C 'lsazyhh@163.com'
  + 生成的内容在 .ssh中 (id_rsa       **id_rsa.pub**      know_hosts) ssh 放在id_ rsa.pub 中
  + 代码拉下来
    + git clone
  + 代码推送
    + git push origin < branchname>
  + 本地分支跟踪服务器分支
    + git branch --set-upstream-to=origin/main main
  + 推送修改
    + git push
  + 拉取代码从远程分支上拉去代码
    + git pull
+ star(收藏)
+ fork（复制独立仓库）



+ pull request（提交更改）
+ watch（关注项目）
+ issue（讨论bug）

github主页

仓库主页

个人主页

## git 

+ 分布式
+ 版本控制
+ 软件
+ 常用命令：
  + git config --global user.name   签名
  + git config --global user. email   邮箱
  + 初始化本地库  git init 新建一个本地文件夹 用 git init初始化本地仓库 对仓库中的代码进行版本控制
  + 查看git状态 git status
  + **追加暂存区**  **git add**
  + **git  commit -m  "注释"  **
    + 两条一起用创建一个版本，多次add 一次commit
  + git relog  / git log 查看日志
  + 最新版本用HEAD指针指向着，上一版本用HEAD^，HEAD~100表示 往前推加尖括号即可
  + **版本之间的反复跳换git reset --hard HEAD^**
  + **git   reset  --hard 版本号**
  + git     reflog 查看操作history
  + 管理修改
  + 撤销修改  在工作区所做的修改不想保存在暂存区可以 用git  status 查看状态然后 git restore 撤销修改
  + 已经提交了 不适合的修改版本库时 考虑回退版本
  + 对比文件不同
    + 对比工作区和版本库的不同
    + git diff HEAD --  < file name>
    + 对比版本库里面的不同
    + git diff HEAD HEAD^ -- < file name>
  + 删除文件
    + 工作区修改 直接 git restore
    + 已提交暂存区 先返回版本git reset HEAD file  回到工作区修改场景 
    + 删除 git rm + git 
    + commit

![image-20220316220944706](C:\Users\lsazy\AppData\Roaming\Typora\typora-user-images\image-20220316220944706.png)

+ 通过新建指针创建新分支
  + git branch < branchname > 新建分支
  + git checkout  -b dev 新建dev的并切换到该分支
  + 分支切换 git checkout < branchname >
  + 合并分支 git merge < branchname >  fast merge
  
+ 解决冲突
  + 手动解决 git --graph --pretty=oneline 可以看到冲突的地方
  
+ git stach 出现紧急事件的时候暂存

+ ![image-20220320211900772](C:\Users\lsazy\AppData\Roaming\Typora\typora-user-images\image-20220320211900772.png)

  ### git 应用

  ~~~c++
  当你在 GitHub 创建一个代码仓库后，需要將其与你的本地仓库关联起来。
  在本地创建一个新仓库并关联：
  cd /path/to/repo
  touch README.md
  git init
  git add README.md
  git commit -m "First commit"
  git remote add origin git@github.com:zhaqiang/learngit.git
  git push -u origin master
  
  关联一个已存在的仓库:
  cd /path/to/repo
  git remote add origin git@github.com:zhaqiang/learngit.git
  git push -u origin master
  ~~~

  
