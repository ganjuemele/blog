# git 远程仓库
用SSH地址，复制ssh地址
```
ssh-keygen -t rsa -b 4096 -C 你的邮箱
cat ~/.ssh/id_rsa.pub                           # 得到公钥内容
ssh -T git@github.com
git remote add origin git@xxxxxxx
git push -u origin master
```
*新建了一个名为 ’19-12-26’的公钥*
 id_rsa和id_rsa.pub
* git remote add origin git@XXXXXX
在本地添加远程仓库
origin是远程仓库的默认名字，可以换，建议不换
不要使用https地址，因为每次都需要密码
电脑上存放私钥，github留下公钥
上传代码是用私钥加密，github用公钥解密
* git push -u origin master
推送本地master分支到远程 origin的master 分支
⚠️如果 提示 应该git pull…，那就git pull 一下
git pull是先把远程分支合并到本地对应的分支
如果远程分支没有更新过，才能省略 git pull
-u origin master 的意思是设置上游分支
之后就不用设置上游分支课，直接git pull；git push；
