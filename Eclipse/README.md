#Ubuntu安装Eclipse
### 1. 安装JDK；（详情见Ubuntu安装JDK：）
---
### 2. 安装Eclipse
> 1. 下载好Linux版本的Eclipse的安装包，我这里下载的是eclipse-inst-linux64.tar.g；  
https://www.eclipse.org/downloads/eclipse-packages/?osType=linux&release=undefined
![image](http://note.youdao.com/yws/api/personal/file/6F24800BAD824093B0DBA9F530DFDB4E?method=download&shareKey=d9da85e8c9f587a59d67e76bf707258e)
> 2. 解压Eclipse  
打开终端并使用命令：cd /opt/ && sudo tar -zxvf ~/下载/eclipse-inst-linux64.tar.gz（cd /opt/是解压目标文件夹）
解压完成后，就可以在 /opt/目录中看到Eclipse；  
![image](http://note.youdao.com/yws/api/personal/file/B392D6E468024DA9B0457F1F3CCD9DE4?method=download&shareKey=56076f35bffa46b9fba37b4615e30bcb)
![image](http://note.youdao.com/favicon.ico)
---
### 2. 创建Eclipse快捷方式
> 1. 在终端执行如下命令：
cd 桌面  
sudo touch eclipse.desktop  
sudo vim eclipse.desktop  
输入以下内容：  

        [Desktop Entry]  
        Encoding=UTF-8   
        Name=eclipse   
        Comment=Eclipse IDE   
        Exec=/usr/local/eclipse/eclipse_SDK/eclipse   
        Icon=/usr/local/eclipse/eclipse_SDK/icon.xpm   
        Terminal=false   
        StartupNotify=true   
        Type=Application  
        Categories=Application;Development;    
> Exec=/usr/local/eclipse/eclipse_SDK/eclipseIcon=/usr/local/eclipse/eclipse_SDK/icon.xpm 这个地方要修改为你的eclipse安装目录。  
保存。  
执行:sudo chmod u+x eclipse.desktop 将其变为可执行文件.  
---
