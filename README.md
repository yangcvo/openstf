
## openstf

* 这是stf官网：https://openstf.io

* stf-github源码：https://github.com/openstf/stf


## Install STF

* 参考链接：


## centos 安装SDK方法：

* 参考链接：

``` bash 
我这里有RPM的一键安装包，因为是在服务器上，所以是木有任何桌面环境的，也就木有桌面浏览器啦。用 wget 或者 curl 下载即可。下载成功后，解压，查看了下载的SDK文件目录 可是目前目录下面只有 tools 目录，没有 platform-tools 目录，这个目录下的东西可不少哦，神马 aapt、dx 等等非常重要的工具都可是在这个里头哦，通常我们都是直接通过 android 命令就可以启动 Android SDK Manager 的界面管理工具，通过勾选不同平台就可以选择性地更新哪个版本的 sdk 了。
```

共享链接：
* [RPM 安装GLIBC下载包](https://rpmfind.net/linux/rpm2html/search.php?query=glibc)
* [RPM 安装GLIBC下载包](http://www.filewatcher.com/m/glibc-2.14.1-6.x86_64.rpm.3504537-0.html)

这里我已经下载好了，可以到我这上面下载。

## Installation method:

``` bash
 [root@openstf ~]# rpm -ivh --force glibc-2.15-22.6.4.x86_64.rpm
warning: glibc-2.15-22.6.4.x86_64.rpm: Header V3 RSA/SHA256 Signature, key ID 3dbdc284: NOKEY
Preparing...                ########################################### [100%]
   1:glibc                  ########################################### [100
   ```
   
   
