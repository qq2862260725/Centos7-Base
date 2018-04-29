# Centos7-Base
## Nginx Node Git
### centos7基本配置
#### Nginx配置
##### 1、安装依赖软件
- yum -y install gcc gcc-c++ autoconf automake make
- yum -y install zlib zlib-devel openssl openssl-devel pcre pcre-devel
##### 2、安装Nginx
- wget http://nginx.org/download/nginx-1.13.7.tar.gz
- tar zxvf nginx-1.13.7.tar.gz
- mkdir -p /usr/local/nginx
- cd nginx-1.13.7/
- ./configure
- make && make install
##### 3、启动Nginx
- cd /usr/local/nginx/sbin
- ./nginx

#### Node安装
##### 1、下载Node
- wget http://nodejs.org/dist/v0.10.30/node-v0.10.30.tar.gz
- tar xzvf node-v* && cd node-v*
##### 2、安装编译软件
- sudo yum install gcc gcc-c++
- ./configure
- make
- sudo make install
##### 3、测试安装是否成功
- node --version

#### Git安装
##### 1、Git下载
- yum install git
- yes
##### 2、检查是否安装成功
- git --version