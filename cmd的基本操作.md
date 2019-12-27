# cmd的操作
### npm i -g tldr 太长不想读

recursive 递归的
echo 回声 ::echo::
force 强制 
change 改变 cd中的::c::
directory 文件夹/目录 cd中的::d::
make ::mk::
move ::mv::
remove ::rm::
copy ::cp::
list ::ls::
link ::ln::
find ::find::
touch ::touch::
::pwd:: 展示当前的绝对路径
clear 清屏
- - - -
##### 查看文件内容
cat 路径 全部查看
head 路径 头10行
tail 路径 尾10行
less 路径 看其中一屏部分
- - - -
###### 增
touch 文件名
echo 内容 > 1.js  //新建文件并添加内容
echo 内容 >> 1.js  //追加内容到文件
echo  -e “内/n容” >> 1.js  //换行符
mkdir 创建文件夹
mkdir -p 路径 //创建深层的目录
cp 复制的文件名  新文件名
cp -r 目录名 新目录名
- - - -
###### 改
移动文件 mv 文件名 路径
重命名 mv 文件名 新文件名
touch 修改文件最后更新时间

###### 脚本文件
&& 然后
;  并且
先写一段脚本，
```
mkdir $1 //$1是当前输入的参数
cd $1
touch index.html
touch style.css
touch main.js
echo -e "<!DOCTYPE html>\n<p>标题</p>" >> index.html
```
再 chmod +x 脚本文件名
./脚本名
- - - -

## 设置直接终端命令打开webstorm
webstorm程序中 ::**Tools**  >>  **Create Command-line Launcher**::
设置完成后在终端输入cd /usr/local/bin命令，可以看到在bin文件夹下面有webstorm.
* 编辑 ::.zshrc:: 文件。vim .zshrc
* 为Webstorm添加别名。::alias ws=“webstorm”::
* 然后::source .zshrc::即可生效。
