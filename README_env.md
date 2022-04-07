# nginx和fastDFS-nginx-module
## 安装FastDFS
### 安装libfastcommon
安装FastDFS之前要先安装它的依赖库libfastcommon,
``` git clone https://github.com/happyfish100/libfastcommon.git
``` cd libfastcommon
``` ./make.sh
``` ./make.sh install


### 安装FastDFS
``` https://github.com/happyfish100/fastdfs.git
tar -xzf FastDFS_v5.08.tar.gz
cd FastDFS
./make.sh
./make.sh install

### 安装fastdfs-nginx-module
``` git clone https://github.com/happyfish100/fastdfs-nginx-module/
cd nginx
./configure --add-module=/usr/local/fastdfs-nginx-module/src
make
make install

说明：/usr/local/fastdfs-nginx-module/src根据自己的文件目录来配