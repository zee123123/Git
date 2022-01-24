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
会把你所有的 uncommitted changes 进行进行保存
`git stash pop`
删除你的 stash
___
# Why?
用来保存你不想要 commit 的东西! 不想要上传, 但是还是要保存一下
___
