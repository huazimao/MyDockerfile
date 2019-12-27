# 以 centos7 为基础镜像
# daocloud.io为docker国内镜像站点
FROM daocloud.io/centos:7
MAINTAINER qinxuan_work@163.com
# 安装JDK
ADD jdk1.8.0_191 /usr/local/jdk1.8.0_191
ADD tomcat9 /usr/local/tomcat9
# 设置环境变量
ENV JAVA_HOME /usr/local/jdk1.8.0_191
ENV PATH /usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin:/root/bin:$JAVA_HOME/bin
RUN yum -y install glibc.i686
#公开端口sdf
EXPOSE 8080
#设置启动命令
ENTRYPOINT /usr/local/tomcat9/bin/startup.sh && tail -F /usr/local/tomcat9/logs/catalina.out
