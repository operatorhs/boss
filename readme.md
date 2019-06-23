
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
- `git log` 查看所有的的提交次数

### GitHub 
- 不是git，只是一个网站
- 只不过时这个网站提供了允许别人通过git上传代码的功能https://github.com/

### 提交代码到github(当作git服务器使用)
- `git push [address] master`
 + 会把当前分支的内容上传到远程的master分支上
 + 示例 `$ git push https://github.com/operatorhs/boss.git master`

### `git pull [address] master`
 + 示例： `$ git pull https://github.com/operatorhs/boss.git master`
 + 把代码初始化到笨的仓库
 
### `git clone [address]` 多次执行会覆盖本地的内容
 + 示例`git clone https://github.com/operatorhs/boss.git `

### ssh 方式上传代码
- 公钥 私钥，两者之间是有关联的
- 生成公钥，和私钥（/c/Users/NI/.ssh/id_rsa）.pub文件为公钥
- `ssh-keygen -t rsa -C "operatorhs"` 示例 `$ ssh-keygen -t rsa -C "operatorhs"`
- 上传示例`$ git push git@github.com:operatorhs/ssh_test.git master`

### 本地提交先pull 在push 可以先解决冲突 把最新版本上传到服务器
- 当我们在push时，加上一个-u参数，那么下一次push时
- 我只需要写上`git push`就能上传我们的代码。(加上-u之后，git会把当前分支与远程的指定分支进行关联`git push origin master`) `-u master`

### 添加本地address 
- 创建一个origin变量代表 【address】 `$ git remote add origin git@github.com:operatorhs/boss.git`
