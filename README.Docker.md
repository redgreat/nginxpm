# Nginx代理Web控制台Docker镜像


This is a Docker container for [Nginx Proxy Manager](https://nginxproxymanager.com).


官方介绍
---

Nginx Proxy Manager enables you to easily forward to your websites running at
home or otherwise, including free SSL, without having to know too much about
Nginx or Letsencrypt.

---

## 运行
```shell
docker run -d \
    --name=nginxpm \
    -p 8181:8181 \
    -p 8080:8080 \
    -p 4443:4443 \
    -v /docker/appdata/nginx-proxy-manager:/config:rw \
    redgreat/nginxpm
```
映射文件包含各种配置、日志等
`/docker/appdata/nginx-proxy-manager` 

浏览器打开 `http://your-host-ip:8181`

## 文档

[官方文档](https://github.com/jlesage/docker-nginx-proxy-manager)

