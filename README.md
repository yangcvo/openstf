
## openstf

* 这是stf官网：https://openstf.io

* stf-github源码：https://github.com/openstf/stf


### Centos Install STF

* Reference link：[STF 安装](http://blog.yangcvo.me/2016/06/28/Cento6-7安装WEB端批量移动设备管理控制工具STF的环境搭建和运行/)


### centos 安装SDK方法：

*这里我参考Google这篇文档：[sdk参考文档](http://7dot9.com/2012/12/13/centos-64%E4%BD%8D%E6%9C%BA%E5%99%A8%E9%85%8D%E7%BD%AEandroid-sdk%E5%92%8Cndk%E7%8E%AF%E5%A2%83/)


### Shared link：

* [RPM 安装GLIBC下载包](https://rpmfind.net/linux/rpm2html/search.php?query=glibc)
* [RPM 安装GLIBC下载包](http://www.filewatcher.com/m/glibc-2.14.1-6.x86_64.rpm.3504537-0.html)

这里我已经下载好了，可以到我这上面下载。

### Installation method:

``` bash
 [root@openstf ~]# rpm -ivh --force glibc-2.15-22.6.4.x86_64.rpm
warning: glibc-2.15-22.6.4.x86_64.rpm: Header V3 RSA/SHA256 Signature, key ID 3dbdc284: NOKEY
Preparing...                ########################################### [100%]
   1:glibc                  ########################################### [100
   ```
   
   
### 安装RethinkBD
* 参考链接：[Reference article](https://www.rethinkdb.com/docs/install/centos/)


###安装GraphicsMagick
* 最新版本包地址：http://sourceforge.net/projects/graphicsmagick/files/graphicsmagick/


最好推荐环境：Ubuntu15.04(desktop-64bit) 

* 这里参考文档: [STF的环境搭建和运行](http://www.open-open.com/lib/view/open1437967814581.html)
