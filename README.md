# Docker-Command  
Some important and commonly used docker commands  

## 基础命令  
docker version          &emsp;#查看docker的版本信息  
docker info             &emsp;#查看docker的系统信息,包括镜像和容器的数量  
docker 命令 --help      &emsp;#帮助命令(可查看可选的参数)  


## 镜像命令  
docker images          &emsp;#查看本地主机的所有镜像  
     #解释:  
     &emsp;1.REPOSITORY &ensp;  镜像的仓库源  

     &emsp;2.TAG &ensp;  镜像的标签  

     &emsp;3.IMAGE ID &ensp; 镜像的id  

     &emsp;4.CREATED &ensp; 镜像的创建时间  

     &emsp;5.SIZE &ensp; 镜像的大小  

docker search  &emsp;#搜索镜像  

docker pull &emsp;#镜像名[:tag] 下载镜像  

docker rmi &emsp;# 删除镜像  


## 容器命令
docker pull centos  &emsp;#如拉取一个centos容器  
docker run -it centos /bin/bash &emsp;#进入centos容器  
#exit &emsp;#停止并退出容器（后台方式运行则仅退出）  
#Ctrl+P+Q  &emsp;#不停止容器退出  
docker ps &emsp;#列出当前正在运行的容器  
docker ps -a &emsp;#列出所有容器的运行记录  
docker rm 容器id  &emsp;#删除指定的容器,不能删除正在运行的容器,强制删除使用后面加-f  
docker start 容器id       &emsp;   #启动容器  
docker restart 容器id     &emsp;   #重启容器  
docker stop 容器id        &emsp;   #停止当前运行的容器  
docker kill 容器id        &emsp;   #强制停止当前容器  

## 查看日志
docker &nbsp;logs &nbsp;--tail&nbsp; [number] &nbsp;容器id  &emsp;#num为要显示的日志条数



