`git blame [-L line_start,line_end] filename`   
追究某行代码责任人

`git diff --stat (tag/version_number)`  
图例显示代码修改

`git merge, git merge --squash, git cherry-pick`  
三种merge方式，第一为普通，第二为挤压成一条放到末端，第三为挑选需要的commit整合


`git commit -C HEAD --amend`  
对某一条commit进行错误修正，不会新增一条commit。 -C是说用同一条message，-c新写一条message

`git revert [-n] (commit编号)`  
回转到指定commit，-n表示不立即提交，而是放入暂存区。与reset的区别在于，revert不会消除commit记录，而是新增一条。reset则会丢弃已有的commit

`git reset (--hard|--soft|--mixed) (commit编号)`  
消除commit记录，hard是清除三个区域，soft是仅清除发布区，mixed是仅清除暂存和发布区

rebase可以用来修改历史，较复杂，用处不多

`git branch -r`  
查看远程的分支

`git push origin mybranch:master`  
将本地分支mybranch上的提交推送到远程master分支上

`git push origin master`  
是说将master推到远程origin上，但origin需要提前命名，命名方法就是git remote add origin xxxx
