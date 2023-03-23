![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/wbhiRD1.webp)

```
"registry-mirrors": [ "https://dockerproxy.com" ]
```

本机开发调试

```
PG_HOST=pg

REDIS_HOST=redis
```

修改为

```
PG_HOST=127.0.0.1

REDIS_HOST=127.0.0.1

```

并注释掉 `NODE_ENV=production`

## 配置文件

`ops/docker/wac/.env`

redis、postgresql 的密码都默认生成了。需要配置下 MAIL 的 SMTP 发信。
