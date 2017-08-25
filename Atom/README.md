# Ubuntu系统安装Atom
### 安装Atom
    PPA安装，打开终端使用以下命令安装：
    sudo add-apt-repository ppa:webupd8team/atom
    sudo apt-get update
    sudo apt-get install atom
---
### 卸载Atom
    sudo apt-get remove atom
    sudo add-apt-repository --remove ppa:webupd8team/atom
    以上只会卸载该软件，要卸载附加的一些软件包，请使用以下命令卸载多余的软件包：
    sudo apt-get autoremove
---
