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
git remote
git remote -v
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
```

### 5. pull 
基本操作 add commit push 都不说了
每次push之前，先pull检查是否有更改
pull 会合并线上代码到你的分支上

```shell
git pull online master
```
