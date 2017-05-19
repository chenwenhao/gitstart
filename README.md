# gitstart
> 假如一个叫herry的家伙要和我一起协作开发,他拉下代码，在本地建立一个dev2的分支

### 1. Fork 
略
### 2. clone
```shell
git clone  https://github.com/herry/gitstart.git
```

### 3. remote
```shell
git remote add online https://github.com/chenwenhao/gitstart.git   //增加一个本地可操作的远程仓库  别名
git remote     //查看状态
git remote -v  //查看状态
```
### 4. branch
```shell
git checkout -b dev2   //创建一个本地分支
git push origin dev2   //在线上创建一个分支

git checkout dev2       //切换分支

/* 吭吱 吭吱 干活  merge后*/

git branch -d dev2   删除本地的分支
git branch -dr origin/dev2

git push origin --delete dev2 //删除一个线上分支
					   
git branch -a   //查看状态
git status      //查看状态
```

### 5. pull 
>基本操作add、commit、push 都不说了。
>每次push之前，先*pull检查是否有更改*.
>pull会合并线上代码到你的分支上

```shell
git pull online master
```

# 后续
1. 使用 SSH 公钥验证
2. 创建分支的命名规则,flow git 工作流
3. bare 裸仓库
4. 忽略文件 
5. Stash用法
6. fetch pull merge rebase tag log track
7. 导出文件
8. 还原代码，还原到某个版本
9. 提交写注释的规则
10. 冲突的解决
11. 理解HEAD
12. 提交日志
