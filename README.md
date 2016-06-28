
## openstf

* 这是stf官网：https://openstf.io

* stf-github源码：https://github.com/openstf/stf


### Install STF

*Reference link：


### centos 安装SDK方法：

*Reference link：


我这里有RPM的一键安装包，因为是在服务器上，所以是木有任何桌面环境的，也就木有桌面浏览器啦。用 wget 或者 curl 下载即可。下载成功后，解压，查看了下载的SDK文件目录 可是目前目录下面只有 tools 目录，没有 platform-tools 目录，这个目录下的东西可不少哦，神马 aapt、dx 等等非常重要的工具都可是在这个里头哦，通常我们都是直接通过 android 命令就可以启动 Android SDK Manager 的界面管理工具，通过勾选不同平台就可以选择性地更新哪个版本的 sdk 了。


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
With binaries
We provide binaries for both 32-bit and 64-bit CentOS 6 and 64-bit Centos 7.

To install the server, first add the RethinkDB yum repository to your list of repositories.

`For Centos 6`
```
sudo wget https://download.rethinkdb.com/centos/6/`uname -m`/rethinkdb.repo \
          -O /etc/yum.repos.d/rethinkdb.repo
sudo yum install rethinkdb
```

`For Centos 7`
```
sudo wget http://download.rethinkdb.com/centos/7/`uname -m`/rethinkdb.repo \
          -O /etc/yum.repos.d/rethinkdb.repo
sudo yum install rethinkdb
```
Compile from source on Centos 7
Get the build dependencies

Install the main dependencies:
```
sudo yum install openssl-devel libcurl-devel wget tar m4 git-core \
                 boost-static m4 gcc-c++ npm ncurses-devel which \
                 make ncurses-static zlib-devel zlib-static
```
### INSTALL OPTIONAL BUILD DEPENDENCIES

Additional build dependencies are available in the EPEL repository. Installing these will speed up the build process.
```
sudo yum install epel-release
sudo yum install protobuf-devel protobuf-static jemalloc-devel
```
### Get the source code

Download and extract the source tarball:
```
wget http://download.rethinkdb.com/dist/rethinkdb-2.3.4.tgz
tar xf rethinkdb-2.3.4.tgz
```
### Build RethinkDB

Kick off the build process:
```
cd rethinkdb-2.3.4
./configure --allow-fetch --dynamic jemalloc
make
sudo make install
```
Compile from source on Centos 6
These instructions have been tested on CentOS 6.5.

Get the build dependencies

The version of GCC included with Centos 6 is too old to compile RethinkDB. A newer version can be installed using devtoolset:
```
rpm --import http://ftp.scientificlinux.org/linux/scientific/5x/x86_64/RPM-GPG-KEYs/RPM-GPG-KEY-cern
sudo wget -O /etc/yum.repos.d/slc6-devtoolset.repo http://linuxsoft.cern.ch/cern/devtoolset/slc6-devtoolset.repo
```
### Install the main dependencies:
```
sudo yum install devtoolset-2 ncurses-devel boost-static openssl-devel \
                 libcurl-devel wget tar which m4
INSTALL OPTIONAL BUILD DEPENDENCIES
```
CentOS provides neither a protobuf-devel package nor a jemalloc-devel package. Installing these dependencies from the EPEL repositories will allow RethinkDB to build more quickly:
```
sudo rpm -Uvh http://download.fedoraproject.org/pub/epel/6/x86_64/epel-release-6-8.noarch.rpm
sudo yum install protobuf-devel jemalloc-devel
Get the source code
```
### Download and extract the source tarball:

```
wget https://download.rethinkdb.com/dist/rethinkdb-2.3.4.tgz
tar xf rethinkdb-2.3.4.tgz
Build RethinkDB
```
### Kick off the build process:

``` 
cd rethinkdb-2.3.4
scl enable devtoolset-2 -- ./configure --dynamic jemalloc --allow-fetch
scl enable devtoolset-2 -- make
sudo make install
```
Next steps: Now that you’ve installed RethinkDB, it’s time to install client drivers for your language.

[Reference article](https://www.rethinkdb.com/docs/install/centos/)


