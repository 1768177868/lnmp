# docker lnmp
#### 介绍

nginx:1.17
php7.4 
mysql5.7
redis:5.0.8
phpmyadmin:5.0.2



#### 使用说明

​	git clone https://gitee.com/wangxuancheng/lnmp.git

​    cd lnmp  

​    docker-compose up -d

​	http://127.0.0.1

​	http://127.0.0.1:888



### 服务器启动和构建命令

如需管理服务，请在命令后面加上服务器名称，例如：

```
docker-compose up -d	  以守护进程模式运行加-d选项
docker-compose ps	      列出所有运行中的容器,类似docker ps
docker-compose logs web	  查看web服务日志
docker-compose stop	      停止已运行的服务
docker-compose down	      停止并移除容器、网络、镜像和数据卷.比stop更彻底
docker-compose restart	  重启YAML文件中定义的服务
docker-compose kill	      停止服务
docker-compose rm	      删除指定已经停止服务的容器
docker-compose build	  构建或重建服务
docker-compose images	  列出所有镜像
docker-compose pull	      拉去并下载指定服务镜像
docker rmi -f $(docker images -q)  删除所有镜像


docker-compose up nginx php mysql         # 创建并且启动nginx、php、mysql的多个容器
docker-compose up -d nginx php  mysql     # 创建并且已后台运行的方式启动nginx、php、mysql容器
docker-compose start php                  # 启动服务
docker-compose stop php                   # 停止服务
docker-compose restart php                # 重启服务
docker-compose build php                  # 构建或者重新构建服务
```

