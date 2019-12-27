# 以 centos7 为基础镜像
FROM daocloud.io/centos:7
MAINTAINER qinxuan_work@163.com
# 安装JDK
ADD jdk-8u191-linux-i586.tar.gz /usr/local/
# 设置环境变量
ENV JAVA_HOME /usr/local/jdk1.8.0_191
ENV PATH /usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin:/root/bin:$JAVA_HOME/bin
RUN yum -y install glibc.i686