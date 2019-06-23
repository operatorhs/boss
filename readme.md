
### 把我们的代码仓储门口
- `git add ./` 
`git commit -m` 

### 创建分支
- `git branch dev`
  + 创建了一个dev分支
  + 在刚创建时dev分支里的东西和master分支里的东西一样
### 切换分支
- `git checkout dev`
 + 切换到指定的分支，这里切换到名字为dev的分支
 	`git branch` 可以查看当前有哪些分支

### 合并分支
- `git merge dev`
 + 合并分支内容，把当前分支与指定的分支（dev），进行合并
 + 当前的分支值得时`git branch`命令输出的前面有*号的分支 
 
### 查看历史提交记录
- `git log --online`

### GitHub 
- 不是git，只是一个网站
- 只不过时这个网站提供了允许别人通过git上传代码的功能https://github.com/

### 提交代码到github(当作git服务器使用)
- `git push [address] master`
 + 会把当前分支的内容上传到远程的master分支上
 + 示例 `$ git push https://github.com/operatorhs/boss.git master`