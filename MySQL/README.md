# Ubuntu安装MySQ
### 1. Ubuntu下安装MySQL
Ubuntu上安装MySQL非常简单只需要几条命令就可以完成。

>  1.sudo apt-get install mysql-server  
2.apt-get isntall mysql-client  
3.sudo apt-get install libmysqlclient-dev  
安装过程中会提示设置密码什么的，注意设置了不要忘了，安装完成之后可以使用如下命令来检查是否安装成功：  
sudo netstat -tap | grep mysql   
通过上述命令检查之后，如果看到有MySQL 的socket处于 listen    状态则表示安装成功。  
---
### 2. Ubuntu下MySQL的简单操作
> 登陆MySQL数据库可以通过如下命令：  
mysql -u root -p  
-u 表示选择登陆的用户名， -p   表示登陆的用户密码，上面命令输入之后会提示输入密码，此时输入密码就可以登录到mysql。  
![image](https://ss0.baidu.com/6LVYsjip0QIZ8Aqbn9fN2DC/timg?pa&quality=100&size=w4096&sec=1503890544&di=33e7864193e7e18211e567b27579b052&ref=http%3A%2F%2Fwww%2Elinuxidc%2Ecom%2FLinux%2F2016%2D07%2F133128%2Ehtm&src=http%3A%2F%2Fwww%2Elinuxidc%2Ecom%2Fupload%2F2016%5F07%2F160713215251881%2Ejpg)  
然后通过 show databases; 就可以查看当前的数据库。  
我们选择 MySQL数据库就行  
下一步操作，使用use mysql   命令，显示当前数据库的表单：show tables  
![image](https://ss0.baidu.com/6LVYsjip0QIZ8Aqbn9fN2DC/timg?pa&quality=100&size=w4096&sec=1503890544&di=07494bf9d1a7abf4226f61a4dbc3d447&ref=http%3A%2F%2Fwww%2Elinuxidc%2Ecom%2FLinux%2F2016%2D07%2F133128%2Ehtm&src=http%3A%2F%2Fwww%2Elinuxidc%2Ecom%2Fupload%2F2016%5F07%2F160713215251882%2Ejpg)  
---
    
