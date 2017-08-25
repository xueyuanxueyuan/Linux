# Ubuntu系统修改Hosts文件使用谷歌浏览器
### 修改Hosts文件
> 1. 修改系统文件需要获得root权限:  
user  $ su  
password:  
> 2. 获得权限后使用，输入如下命令打开编辑器用于编辑：
sudo gedit /etc/hosts  
> 3. 下载Hosts文件：http://pan.baidu.com/s/1dFneaDb  
> 4. 打开刚刚下载的hosts文件，找到你想要的域名代理谷歌，脸书，推特等，需要啥就往你的hosts里面复制啥，如下找谷歌的：  
![image](http://img.blog.csdn.net/20151215211705904?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQv/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)
> 5. 保存你的hosts文件并推出  
> 6. 重启网络：  
sudo /etc/init.d/networking restart    

