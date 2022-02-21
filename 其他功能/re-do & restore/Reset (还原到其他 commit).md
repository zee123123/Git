还原
___
课的链接: https://www.udemy.com/course/git-and-github-bootcamp/learn/lecture/24650478#overview
___
# What?
如果你 accidently 搞了一个 commit, 你想要还原到上几个 commit 之一
___
# How to 实现?
用`git reset <commit-hash>`
___
# How it works?
会将你commit 的文件从 repository 转移到Working directory 当中 (___你写的文件并不会消失___)
也就是说你可以接着把 switch 到另一个 branch, 然后再次进行 git add, 然后 git commit
___
___如果你也要想删除文件, 用 hard reset___
##  命令
`git reset --hard <commit>` 
此命令会将这个 commit 删除, 包括你的 local change 然后回到你想要 reset 的 commit 上
___
