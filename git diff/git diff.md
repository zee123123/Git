# What?
`git diff` 是用来 show 和你当前的 staging area 与  上一次 commit 的 difference
默认情况下(没有 option), ___比较的是当前代码(staging )与最近一次的 commit___
___
得到这样的 output:
![[Pasted image 20220116142811.png]]
a 和 b 的意思是两个不同的版本
蓝色字代表着那几行有改变
`-`代表消除的, 	`+` 代表 add in 的
第一个数字代表着开始 modified 的line, 后面的数字代表着一共更改了几行
![[Pasted image 20220116143545.png]]
___
# Options
`git diff HEAD`
show 所有与 HEAD的不同
`git diff --staged` = `git diff --cashed`
show  与 staging area 与 last commit 之间的 difference
`git diff --staged FILENAME_1 FILENAME_2`
show specific 文件的 difference
`git diff BRANCH1 BRANCH2`
show 这两个 branch 的区别
`git diff COMMIT_HASH_NAME_1 COMMIT_HASH_NAME_2`
show两个 commit 之间的区别
commit 的 hash code 可以通过 `git log`来 check
___
![[Pasted image 20220130154029.png]]

      