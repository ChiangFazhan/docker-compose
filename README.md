## 一.说明

> 1.为了避免线下,线上环境不统一造成的BUG
> 2.采用docker-compose作为基础工具进行本地环境的统一
> 3.每个开发人员在该仓库中以自己的名字汉语拼音全拼命名目录,在里面编排自己的本地开发环境(除了基础镜像以及网段必须一致之外,其余可以自由拓展)
> 4.学习文档 https://docs.docker.com/compose/compose-file/#compose-file-structure-and-examples
> 5.所有的项目请git clone到wwwroot下面,按照组织分好
> 未完待续...
   
## 二.常用指令

> * docker-compose  --help
> * docker-compose up -d         #后台启动所有的编排服务
> * docker-compose up -d  redis  #启动redis,适合编排中追加的新服务的单独启动
> * docker-compose down          #当启动部分失败的时候，则将之前的容器删除，再执行docker-compose up -d启动;Stop and remove containers, networks, images, and volumes
> * docker-compose  restart nginx #当配置文件修改的时候需要这个指令即可
> * docker rm -f     nginx        #当nginx镜像修改的时候需要这个指令

## 三.注意事项

> 1.如果之前创建了相同子网的网络 要先删掉之前的,否则冲突
> 2.如果启动的时候指定了-p 网桥名称。那么停止或删除时也要docker-compose -p 网桥名称 stop
> ...

## 四.经典场景案例
> ...






