# kubernetes

这是一个纯净的Docker image, 目的是方便地部署k8s环境。

## Usage

```
docker pull leothecat/kubernetes

// in someone dockerfile
FROM leothecat/kubernetes:latest
```

## 使用GitHub + DockerCloud自动更新镜像
 
 1. 登录DockerCloud
    
    > https://cloud.docker.com/swarm/leothecat/repository/docker/leothecat/kubernetes/builds
  
 2. 创建一个Repo
 
 3. 连接GitHub
 
 4. 在Builds里点击Configure Automated Builds 开启 AutoBuild （默认应该是开启的）
 
 5. 在git repo中修改Dockerfile并push到master
 
 6. 在Builds页面等待build完成，之后Docker Hub里的镜像就是最新的了
