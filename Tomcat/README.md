# Ubuntu安装Tomcat
### 1. 下载Tomcat7
         打开Tomcat官网   
         http://tomcat.apache.org
         在左边的导航栏的“Download"中找到Tomcat7.0目录，
         点击后进入Tomcat7的页面，选择 tar.gz这个文件类型，然后下载。
### 2. 解压文件
        下载到本地目录（本人存放的目录是/home/xu/Downloads/)后，我们来解压这个文件。
        打开终端，操作如下：  
        $:sudo tar zvxf  ~/Downloads/apache-tomcat-7.0.32.tar.gz  
        这样就可以解压出来了。

### 3. 配置环境
 

         tomcat7需要在两个地方配置环境。打开终端，操作如下：
         
         1）打开系统配置文件，加入环境变量
         
          $:sudo gedit /etc/profile
          
         这时就打开了系统环境配置文件，在文件后面加上以下几句：
         
          export CLASSPATH=$CLASSPATH:%JAVA_HOME/lib/tools.jar
          
          export TOMCAT_HOME=/home/xu/apache-tomcat-7.0.32
          
          export CATALINA_HOME=$TOMCAT_HOME
          
          export PATH=$PATH:$TOMCAT_HOME/bin
          
          
         保存退出。
         
         2）进入tomcat7解压文件夹中的bin目录
         
         $:cd /home/xu/apache-tomcat-7.0.32/bin
         
         $:sudo gedit catalina.sh
         
         这时tomcat7自身配置文件就打开了。我们找到 
         
         cygwin=false这一句，然后在这一句上面加入:
         
         JAVA_HOME=/home/xu/Java/jdk1.6.0_35
         
         保存退出即可。
### 4. 运行Tomcat7
         进入Tomcat的bin目录，执行下列语句：
         
         启动Tomcat的命令：
         
         $sudo ./startup.sh
         
         关闭Tomcat的命令：
         
         $sudo ./shutdown.sh
         
### 5. 检验Tomcat7是否在运行
         $: ps -ef|grep tomcat
         如果出现有Tomcat的进程，那就是在运行了。
         
         打开浏览器，在址址栏输入：http://localhost:8080
         
         如果出现Tomcat7页面，恭喜，安装成功！
