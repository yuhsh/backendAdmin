# backendAdmin
后端管理


## 本地启动注意事项
### 启动redis
1. 搜索redis资源
    `docker search redis`
2. 拉取
    `docker pull redis`
3. 查看reids镜像
    `docker images`
4. 运行
    `docker run -d --name myredis -p 6379:6379 redis:latest`