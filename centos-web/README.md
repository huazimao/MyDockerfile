# MyDockerfile
解压 jdk-8u191-linux-i586.tar.gz    重命名为 jdk1.8.0_191<br>
解压 apache-tomcat-9.0.0.M26.tar.gz    重命名为 tomcat9<br>
解压 HelloWorld.war    重命名为 ROOT 放在tomcat9/webapp下<br>
必须严格按照本文档的目录放置<br>
构建镜像命令<br>
docker build -t docker-helloworld .
运行镜像命令sdf
docker run -d -p 8080:8080 --name docker-web [id]
 