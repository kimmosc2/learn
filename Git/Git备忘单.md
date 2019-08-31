Git备忘单  
===
GitHub官方资料:https://github.github.com/training-kit/downloads/zh_CN/github-git-cheat-sheet/  
  
回退版本  
`git reset --hard commit_id(HEAD^和HEAD~1)`  
  
提交历史
`git log [--pretty=oneline]`  
  
提交历史  
`git reflog`  
  
查看工作区和版本库里面最新版本的区别  
`git diff HEAD -- filename`  
  
放弃在工作区的修改  
`git checkout -- filename`  
  
撤销在暂存区的修改  
`git reset HEAD filename`  
  
删除文件  
`git rm filename`  

关联远程库  
`git remote add origin git@server-name:path/repo-name.git`  
  
第一次推送master分支的所有内容  
`git push -u origin master`  
  
提交内容到远程仓库  
`git push origin master`  
  
查看分支  
`git branch`  
  
创建分支  
`git branch <name>`  
  
切换分支  
`git checkout <name>或者git switch <name>`  
  
创建+切换分支  
`git checkout -b <name>或者git switch -c <name>`  
  
合并某分支到当前分支  
`git merge <name>`  
  
删除分支  
`git branch -d <name>`  