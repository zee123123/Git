# How
discard uncommited changes 抛弃所有的change (回到上一个commit 的状态)
___
# 实现方法:
## 1. checkout
`git checkout HEAD <filename>` or `git checkout -- <file>`
filename 是你想要 discard change 的文件
(checkout HEAD 就是回到 HEAD 指向的这个 commit 的 状态)
## 2. restore:
`git restore <filename>`
restore 文件到 head 所在 commit 的版本
`git restore --source HEAD~1 <Filename>`
指定哪一个 restore 到离 head上第几个commit
___
删除的是在你的 working directory 中 modified changes, 如图:
![[Pasted image 20220205221013.png]]