
这是第五个功能
这是我们做的另一个功能

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