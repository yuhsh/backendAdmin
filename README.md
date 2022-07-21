# backendAdmin
## 项目简介
前后端分离的后端管理系统

**账号/密码** `admin/123456`

## 技术框架
1. SpringBoot 2.1.0
2. SpringBoot JPA
3. JWT
4. Spring Security
5. Redis
6. Mysql
7. VUE(EL-Admin)

## 项目结构
- `backend-common` 为系统的公共模块，各种工具类，公共配置存在该模块
- `backend-system` 为系统核心模块也是项目入口模块，也是最终需要打包部署的模块
    - config 配置跨域与静态资源，与数据权限
    - modules 系统相关模块(登录授权、系统监控、定时任务、运维管理等)
        - quartz
        - security
        - system

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