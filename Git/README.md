# Ubuntu系统安装使用Git
## 1. 安装
### 1.1 通过Apt安装：

> 官网上提供的命令是：  
$ sudo add-apt-repository ppa:git-core/ppa   
![image](http://img.blog.csdn.net/20160228155200518)
中间暂停时，按回车键Enter继续安装。   
$ sudo apt-get update   
$ sudo apt-get install git    
安装下载完成后，可以使用下面的命令行，确认git的版本  
$ git --version   
![image](http://img.blog.csdn.net/20160228160601102)
---
### 1.2 通过Source安装
> 首先，安装一些git依赖的软件：  
$ sudo apt-get install build-essential libssl-dev libcurl4-gnutls-dev libexpat1-dev gettext unzip  
安装完成后，可以在GitHub上公布的Git Project，选择Tags中的最新版本2.7.2： 
![image](http://img.blog.csdn.net/20160228161158323)  
复制下压缩文件的下载链接（Downloads按钮鼠标右键）： 
![image](http://img.blog.csdn.net/20160228161251490)  
使用命令行下载：  
$ wget https://github.com/git/git/archive/v1.9.2.zip -O git.zip  
解压，并路径转换到git下：  
$ unzip git.zip  
$ cd git-*  
编译源码：  
$ make prefix=/usr/local all  
$ sudo make prefix=/usr/local install  
编译完成后，同样可以利用上述的语句查看git版本。   
如果，后面还想继续更新，可以这样：  
$ git clone https://github.com/git/git.git  
访问的链接（URL）可以在上述的GitHub项目中拷贝：  
![image](http://img.blog.csdn.net/20160228162714641)  
然后像上面一样，编译源码：  
$ make prefix=/usr/local all  
$ sudo make prefix=/usr/local install    
就会在git安装位置重装和重编译新的版本（会将旧版本覆盖掉）。  
---
## 2. Git入门
首先在Ubuntu下git的命令截图  
![image](http://img.blog.csdn.net/20160906163314568)  
这些就是Git的基本命令了  
下面就是跟着步骤一步一步的学习这些命令  
### 1. 新建一个数据库
> 在任意目录新建一个文件夹，然后把这个文件夹放到Git的管理之下。  
具体操作步骤就是  
新建一个文件夹  
$ mkdir file_git  
切换到这个文件夹  
$ mkdir file_git  
把他放在Git的管理下面  
$ git init  
这个样几完成了一个数据库建立  
可以执行ls -l 查看一下这个数据库都有什么文件  
![image](http://img.blog.csdn.net/20160906163923617)  
$ cd .git/  
切换到.git目录下，可以看下在初始化数据库后，.git目录下都有什么文件  
![image](http://img.blog.csdn.net/20160906164045879)  
到这里为止，就完成了本地空数据库的建立和初始化  
下面就是在数据库中添加一个新的文件，在文件中添加一些测试文本  
![image](http://img.blog.csdn.net/20160906164533011)  
网上说，在这里需要执行  
$ git status   
下面是截图执行上面命令的截图：  
![image](http://img.blog.csdn.net/20160906164739170)  
这里需要吧文件添加到Git的索引目录中，一个文件只要添加一次就可以了；
添加文件到Git索引中，需要用到命令 add，用空格分割，可以指定多个文件，使用 git add . 可以将所有文件都加入到索引；  
$ git add sample.txt   
![image](http://img.blog.csdn.net/20160906165046925)  
剩下的就是同步数据了，在同步数据之前，这个文件其实是在一个临时的文件，还没有真实的添加到Git的数据库中，需要使用commit明赖来提交 ；   
commit命令格式如下  
$ git commit -m ""  
这里出现了一个问题   
![image](http://img.blog.csdn.net/20160906165609407)  
显示我需要我告诉Git我是谁  
需要执行下面两行代码来配置Git  
$ git config --global user.email "dream_dag@163.com"  
$ git config --global user.name  "DreamLife"    
完成后执行 git commit就可以了  
$ git commit -m "sample.txt first commit"  
![image](http://img.blog.csdn.net/20160906165858861)  
剩下的，我们要查看一下我们的提交记录  
执行 git log命令就可以   
$ git log  
![image](http://img.blog.csdn.net/20160906170200146)

