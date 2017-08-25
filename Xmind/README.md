# Ubuntu系统安装XMind
### 安装XMind
> 下载好Linux版本的XMind的安装包，我这里下载的是xmind-7-linux-amd64.deb    
https://www.xmind.cn/download/linux/  
打开终端，使用cd命令进入保存安装包的目录下，我的包放在了下载目录，如图所示  
之后输入：sudo dpkg -i xmind-7-linux-amd64.deb 回车等待一会就安装成功了
![image](http://note.youdao.com/yws/api/personal/file/CF011E8AC8D14E91AA0E380DCC349B6C?method=download&shareKey=56076f35bffa46b9fba37b4615e30bcb)
![image](http://note.youdao.com/yws/api/personal/file/F44874BB754C4347A196A5A07663BC07?method=download&shareKey=56076f35bffa46b9fba37b4615e30bcb)
如果安装过程中出现下面的问题：  
我们可一看到，它提示的问题都是关于Java的，由于XMind依赖于Java的某些包，而我们还没有安装这些包所导致的，此时我们只需要先安装jdk，然后再安装XMind就可以了(安装JDK的方法见Ubuntu安装JDK：)
![image](http://note.youdao.com/yws/api/personal/file/EBF0660327294CDBA7C4A4E0A45D96C0?method=download&shareKey=56076f35bffa46b9fba37b4615e30bcb)


