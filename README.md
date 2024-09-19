主页  https://immortals007.github.io/

## 思源笔记

### 下载

```bash
# 使用docker 下载镜像
docker pull b3log/siyuan:v3.1.6
```

### 安装

```bash
# 拉取 镜像
docker pull b3log/siyuan:v3.1.6

# 运行镜像地址
docker run \
--name=siyuan \
-di \
--network=bridge \
--restart=always \
-v /volume1/docker/siyuan:/home/siyuan/SiYuan \
-p 6806:6806 \
b3log/siyuan:v3.1.6

# 注意 如果发现映射路径目录下没有生成 思源笔记相关文件, 
# 请检查  该容器的日志提示的正确工作空间路径(网上有很多安装映射路径不正确)  和  群晖的  目录权限授权
执行 
chmod 777 /目标目录
```

###
