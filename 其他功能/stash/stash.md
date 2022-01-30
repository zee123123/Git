stash v. 储藏, 隐藏
___
# What?
用来保存当前的 working记录, 这样当你 create 其他 branch, 可以切换回来; 不用担心 mess it up;
>`git stash` temporarily shelves (or _stashes_) changes you've made to your working copy so you can work on something else, and then come back and re-apply them later on. Stashing is handy if you need to quickly switch context and work on something else, but you're mid-way through a code change and aren't quite ready to commit
>来源:
>https://www.atlassian.com/git/tutorials/saving-changes/git-stash
___
# How?
`git stash`
(其实是`git stash save` 的缩写)
也可以`git stash save "MESSAGE"` 
会把你所有的 uncommitted changes 进行进行保存
`git stash pop`
删除你的 stash
___
会将你的修改放到 git stash 中
___
# Why?
用来保存你不想要 commit 的东西! 不想要上传, 但是还是要保存一下
___
# Options
`git stash apply` 用来应用你的apply, work as a merge
___
## 查看Stashes
___你可以有多个 stash___, 用 `git stash list` 来查看所有 stash
![[Pasted image 20220123220842.png]]
后面的是 commit, 代表着你的 stash 在哪个 commit 上
___
# pop
`git pop`会 pop 出最近的一个 stash, 但是会apply 所有其他的 stash
如果想要apply 特别的哪一个, 需要:
`git stash apply stash@{2}`
___
## Delete 一个特定的 stash
`git stash drop stash@{2}`
##  Delete 所有的 stash
`git stash clear`
____
