Git is a version control system.
Git is free software.
git has a mutable index called stage.
git tracks changes.
window下安装git
1、在官网地址：http://msysgit.github.io下载window版本并安装（默认即可）
2、安装完成后设置环境变量 如：path= D:\Program Files\Git\bin
3、设置账号信息
	git config --global user.name "你的github用户名"
	git config --global user.email "你的github邮箱地址"
4、ssh认证
	打开git bash终端，键入：ssh-keygen -t rsa -C "邮箱地址"，一路回车，就OK了
	在c盘，当前用户文件夹下，有个.ssh 文件夹，在里边 找到 id_rsa.pub文件，用记事本打开，复制其中的全部内容。
	登陆你的GitHub账户，依次点击Account Settings > SSH Public Keys > Add another public key，把id_rsa.pub中的内容拷贝进去 。

5、创建版本库
	$git init
6、关联远程库
	$git remote add origin git@github.com:ZuMingDai/srs-orxyd.git
	注意：
7、把远程代码pull下来
	$git pull origin master


    修改代码后，需要把代码push在服务器上
8、把修改的文件加到代码库
	$git add .或git add  file 
9、把新加的文件提交到代码库
	$git commit -m "注释"
10、把更新的内容push到服务器
	$git push origin master
