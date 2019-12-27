# MyDockerfile
解压 jdk-8u191-linux-i586.tar.gz    
必须严格按照本文档的目录放置<br>
构建镜像命令<br>
docker build -t centos7-jdk8 .
运行镜像命令
docker run -dit --name centos7-jdk8 [id]
进入容器后使用 java javac java -version验证jdk是否安装成功