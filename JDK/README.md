# Ubuntu安装JDK
### 1. 准备源码包
> 1. 首先到官网下载JDK,
  http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html，  
我下载jdk-8u25-linux-x64.tar.gz，下载到主目录  
---
### 2. 解压源码包  
> 通过终端在/usr/local目录下新建java文件夹，命令行：  
sudo mkdir /usr/local/java  
然后将下载到压缩包拷贝到java文件夹中，命令行：  
进入jdk源码包所在目录  
cp jdk-8u25-linux-x64.tar.gz /usr/local/java  
然后进入java目录，命令行：  
cd /usr/local/java  
解压压缩包，命令行：  
sudo tar xvf jdk-8u25-linux-x64.tar.gz  
然后可以把压缩包删除，命令行：  
sudo rm jdk-8u25-linux-x64.tar.gz  

---
### 3. 设置JDK环境变量  
> 这里采用全局设置方法，它是是所有用户的共用的环境变量  
$sudo gedit ~/.bashrc  
如下图所示：  
![image](http://note.youdao.com/yws/api/personal/file/DD73FFF25FA14EAF81F5073867D94696?method=download&shareKey=56076f35bffa46b9fba37b4615e30bcb)  
Ubuntu 17.04安装JDK1.8.0_25与配置环境变量   
打开之后在末尾添加  
export JAVA_HOME=/usr/local/java/jdk1.8.0_25    
export JRE_HOME=${JAVA_HOME}/jre   
export CLASSPATH=.:${JAVA_HOME}/lib:${JRE_HOME}/lib    
export PATH=${JAVA_HOME}/bin:$PATH  
请记住，在上述添加过程中，等号两侧不要加入空格，不然会出现“不是有效的标识符”，因为source /etc/profile 时不能识别多余到空格，会理解为是路径一部分。  
![image](http://note.youdao.com/yws/api/personal/file/D92034A8F7E74A62AABD2C235F49B1F5?method=download&shareKey=56076f35bffa46b9fba37b4615e30bcb)  
然后保存。 
---
### 4. 检验是否安装成功  
> 在终端输入如下命令  
java -version  
看看是否安装成功  
成功则显示如下    
![image](http://note.youdao.com/yws/api/personal/file/122647549B1941E4B2D6C0D58D241B9A?method=download&shareKey=56076f35bffa46b9fba37b4615e30bcb)　　
也可以在终端输入java和javac测试；成功如下：
![image](http://note.youdao.com/favicon.ico)

