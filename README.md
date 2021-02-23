##PHP+NGINX docker-compose
* 基于 centos:centos7 官方镜像
* 使用 163 源
* php 版本为 [5.6.40](https://www.php.net/distributions/php-5.6.40.tar.gz)
* nginx 始终为最新版本
* 数据库相关的, 一般来说, 开发中都会使用同一个, 故个人不进行集成

##目录说明
* conf.d
    * nginx 的配置文件放在这里, default.conf 只是一个参考例子, 根据需要自行配置
* etc
    * php nginx 的配置文件要放于这里, 可在 docker-compose.yml 文件中添加 volumns 进行映射
* logs
    * php nginx 的日志文件
* tmp
    * 映射容器的 tmp
* www
    * 放置您的项目源码

##使用
* 安装 [docker](https://docs.docker.com/get-docker/) 与 [docker-compose](https://yeasy.gitbook.io/docker_practice/compose/install)
* sudo docker-compose up -d
