一般来讲 head 会指向一个 branch, branch 会指向最近的一个 commit 
![[Pasted image 20220130190012.png]]
detached head 的 意思是 head 指向了一个 commit, 而不是一个 branch
![[Pasted image 20220130190143.png]]
___
 # 那么什么情况会造成这种情况?
 比如你 checkout 一个 commit, 此时 head 指向的是一个 commit
 ___
# how to solve detached head?
1. 就这样, 如何不用 push任何 code
2. 回到原来的 branch
3. 在这个 commit 的基础上创建一个 branch, 这个 branch 会包括这个 commit 之后的所有 commit

___
