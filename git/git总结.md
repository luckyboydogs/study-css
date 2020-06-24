1.1 添加远程库

1. git init 
   + 初始化，变成一个本地仓库
2. git remote add origin URL 
   + 把本都库和远程库关联，URL是远程仓库的地址，设置一个变量origin（英文中库的意思）来保存远程库在本地的引用，remote是关键字，英文意思是远程，
   + git remote remove origin 取消本地仓库关联远程仓库，
3. git push -u origin master
   + 把本地库的所有内容推送到远程库上面， 加上-u参数，git不但会把本地的master分支内容推送到远程的master分支上，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令。（origin代表远程库）
4. git push origin master
   + 此后推送最新的修改，就可以简化了。

1.2 克隆仓库

 	1. git clone url
     + git的clone命令会为你自动将远程仓库命名为origin，拉取她的所有数据，创建一个指向他的master分支的指针，并且在本地将其命名为origin/master (origin/master可以看作远程仓库master分支在本地仓库中的一个镜像)。同时git也会给你一个与origin/master分支在指向同一个地方的本地master分支