# UEFI模式安装Ubuntu
windows系统下安装Linux双系统
## 工具
> - 4g左右的U盘；
> - 预备做U盘系统盘的软件和设置开机引导项的软件：软碟通；
> - Linux系统的镜像文件；
## 工具下载
### 软碟通：
- 官网下载地址：https://cn.ultraiso.net/xiazai.html
- 百度云分享：链接：http://pan.baidu.com/s/1nvuVrHv 密码：2mna
---
### EasyBCD：
- 百度云分享：链接：http://pan.baidu.com/s/1dFamNp3 密码：0zom
---
### Linux系统镜像文件：
- Linux中国开源社区：https://linux.cn/article-4130-1.html
> 打开浏览器输入上方连接
![image](http://note.youdao.com/yws/api/personal/file/B69EBB9548B446B1878BEC36CC0F713D?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
> 找到本文导航，然后找你想要的Linux版本
> 
> 这里以ubuntu 17.04为例：
> 
> 点击到指定位置然后根据需要选择下载；
![image](http://note.youdao.com/yws/api/personal/file/0C2EA475E414465A9C0A9C58CA0552C4?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
![image](http://note.youdao.com/yws/api/personal/file/C00AB9FB6F0347379A0231EAF0EE39FB?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
>
> 点击上面的连接下载ubuntu。
---
- ubuntu 官网下载:
进入ubuntu中文官网http://cn.ubuntu.com/
> 点击最上方的下载，进入下载页面，找到你所需要的版本进行下载。
![image](http://note.youdao.com/yws/api/personal/file/B3B5DF62F9B04BE1897C9F4A63D25A7F?method=download&shareKey=3096833220dd5e4745eaa210e6a433f6)
---
- Linux官网下载：进入Linux官网https://www.linux.org/
> ![image](http://note.youdao.com/yws/api/personal/file/F9CA2FFD448446C7AF1653788F3971A1?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
最上方找到DOWNLOAD LINUX点击进入；
![image](http://note.youdao.com/yws/api/personal/file/A40FCAE57533470A814B17EAE24E4814?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
在Download Linux区域找到ubuntu（你所需要的版本）点击进入；
![image](http://note.youdao.com/yws/api/personal/file/13DB3E3C8DEA4AEEB19283B648FE0646?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
点上图所示位置的下载图标进入下载页面，选择版本下载；
![image](http://note.youdao.com/yws/api/personal/file/ED541EAD50E74638AA70287110283FCC?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
---
## 安装步骤（注：由于本人在安装Linux的过程中有些图并没有截到，文中使用的某些图片信息是本人在其他网站搜集并按照本人的安装经验整理的，图所示的步骤没有任何问题，但是图中的数据以及所使用的软件版本与我所介绍的可能有所不同，请按照步骤执行，图仅供参考；）
### 1. 磁盘分区：
> 1. 进入系统的磁盘管理。进入磁盘管理发方式有两种。一种是通过电脑属性，进入磁盘管理。第二种是直接右键点击windows键（windows+X）选择磁盘管理。  
![image](http://note.youdao.com/yws/api/personal/file/0F500923D1D54891A5919581381E5C5F?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
![image](http://note.youdao.com/yws/api/personal/file/61BD9359AEA04ED9A5B245E431104AB4?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
![image](http://note.youdao.com/yws/api/personal/file/F75030217B2C49DDB1A2A893B03BA482?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
> 2. 进入磁盘管理之后，我们可以看到我的分区情况。然后选择你需要进行分区的磁盘，点击右键，选择“压缩卷”，如图示;
![image](http://note.youdao.com/yws/api/personal/file/99245A10395B4E2AA45A83D0DCE7D7EB?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
> 3. 系统会自动的查询压缩空间;
![image](http://note.youdao.com/yws/api/personal/file/831AD1D375064A38A5E0D679F0060566?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
> 4. 然后我们选择选择好需要压缩空间的大小。点击压缩。（这里我压缩出一个大概50G的空间）
![image](http://note.youdao.com/yws/api/personal/file/1C43F4525138403E81A5FDECBF010166?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
![image](http://note.youdao.com/yws/api/personal/file/429C7E9BFC1E4DCC82F7E2F8576CCDBB?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
---
### 2. 制作U盘系统盘
> - 1. 插入U盘，打开软碟通，打开-选择下好的系统iso文件-启动-写入硬盘映像；
![image](http://note.youdao.com/yws/api/personal/file/880FC287C99A4092A4151E9166B78547?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
> - 2. 然后如下图所示，“硬盘驱动器”选择你U盘所在的驱动器（比如我的是I盘），“写入方式”选择“USB-HDD+”；
![image](http://note.youdao.com/yws/api/personal/file/D09F127EA7474E51BE917ECEB3E71DCD?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
> - 3. 接着单击“格式化”，按默认即可（一般默认文件系统位FAT32）（如果你的U盘是个空盘这一步可以忽略）；
![image](http://note.youdao.com/yws/api/personal/file/765DD7C56E014C98BD1565E22539BF75?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
> - 4. 最后单击“写入”，耐心等会，它会显示你写入成功！；
![image](http://note.youdao.com/yws/api/personal/file/7E6ECACC19BD45D0A7AF9A946DA75699?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
![image](http://note.youdao.com/yws/api/personal/file/9DD744E9C9EA4DE68636AF4CC4388579?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
---
### 3. 注意备份电脑重要数据，避免意外；
---
### 4. 设置BIOS：
> - 1. 插入U盘，重启笔记本，启动时按F2(有的电脑是按F12，Del，Esc等等)，进入Bios界面，进入BIOS SETUP后，关闭secure boot，关闭secure boot，关闭secure boot；
> - 2. 在Boot项里选择USB HDD为首项；
> - 3. 保存设置并离开。
![image](http://note.youdao.com/yws/api/personal/file/B281D4811CBC4DDCA194FBD11B659A03?method=download&shareKey=ba2ff90dc1e2fc0776e01358cf78f963)
---
### 5. U盘安装Ubuntu
> 跟往常重装系统一样，插上U盘，根据机器找到进入Boot的快捷键;
> - 1. 找到镜像U盘，调整Priority Order，Save and Exit：
![image](http://upload-images.jianshu.io/upload_images/671333-52245da80b6a24fe.jpg?imageMogr2/auto-orient/strip%7CimageView2/2)
> - 2. 选择“安装Ubuntu Kylin”：
![image](http://upload-images.jianshu.io/upload_images/671333-930c13649fd95892.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
> - 3. 完成默认设置：
![image](http://upload-images.jianshu.io/upload_images/671333-316c38f12e231f9c.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
> - 4. 选择“其他选项”：
![image](http://upload-images.jianshu.io/upload_images/671333-efa9c15dce9a2366.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
> - 5. 为空闲磁盘分区：  
在这一步会看到我们之前分配的未使用磁盘空间，我们即将为这块空闲磁盘分区，为了更方便理解接下来的操作，这里简单介绍一下安装过程所涉及到的几个主要的Linux分区：  
/：存储系统文件，建议10GB ~ 15GB；  
swap：交换分区，即Linux系统的虚拟内存，建议是物理内存的2倍；  
/home：home目录，存放音乐、图片及下载等文件的空间，建议最后分配所有剩下的空间；  
EFI：包含系统内核和系统启动所需的文件，实现双系统的关键所在，建议不要少于500M。**注意：这里用于选择EFI系统文件，不再是Ext4**  
![image](http://upload-images.jianshu.io/upload_images/671333-efa9c15dce9a2366.jpg?imageMogr2/auto-orient/strip%7CimageView2/2)   
选定空闲磁盘，点击+，首先分配16G空间给/分区，选择“主分区”、“空间起始位置”、Ext4和“挂载点/”：
![image](http://upload-images.jianshu.io/upload_images/671333-b66a114eca0c8aee.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  
重复创建步骤，分配16G空间给swap分区，选择“逻辑分区”(主分区已满)、“空间起始位置”、用于“交换空间”：
![image](http://upload-images.jianshu.io/upload_images/671333-8e62830d2d99a979.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  
接着分配500M左右给EFI分区，选择“逻辑分区”、“空间起始位置” **注意：这里选的是逻辑分区，不是主分区，传统模式选的才是主分区**
最后将所有剩余空间分配给/home分区，选择“逻辑分区”(主分区已满)、“空间起始位置”、“Ext4”和“挂载点/home”：
![image](http://upload-images.jianshu.io/upload_images/671333-c70f4de86b3d6db5.jpg?imageMogr2/auto-orient/strip%7CimageView2/2)  
选择/boot对应的盘符作为“安装启动引导器的设备”，务必保证一致：
![image](http://upload-images.jianshu.io/upload_images/671333-f4cecdad1256398f.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  
将改动写入磁盘，耐心等会；
![image](http://upload-images.jianshu.io/upload_images/671333-e60e325a26327ab6.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  
进入最后的设置：
![image](http://upload-images.jianshu.io/upload_images/671333-611c071e24380048.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  
![image](http://upload-images.jianshu.io/upload_images/671333-cc8b9e0e50fefef9.jpg?imageMogr2/auto-orient/strip%7CimageView2/2)  
![image](http://upload-images.jianshu.io/upload_images/671333-159aa5ed54bb2977.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  
![image](http://upload-images.jianshu.io/upload_images/671333-abe8611d11530843.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  
![image](http://upload-images.jianshu.io/upload_images/671333-0829a0d732bb9991.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  
重启系统，进入Windows bios设置进入boot你就会看到windows和Ubuntu的引导项此时你就可以打开secure boot了。这个时候，你可以在boot设置中选择默认开机的系统是windows还是Ubuntu了。**注意，这里不需要使用EasyBCD等引导工具去设置开机引导项，想要切换系统只需要在刚开机时按F12（我的电脑是F12，有些电脑不是可以自己查一下boot选项的按键）就可以选择想要进入的系统；**
（**很抱歉我装系统时没有截图和拍照，我尽快补齐图**）
---

















































