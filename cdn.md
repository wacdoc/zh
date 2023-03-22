# cloudflare 免费绑定自定义域名


## 反向代理 backblazeb2.com

### 配置 CNAME

`CNAME` 指向 `f003.backblazeb2.com`, 其中`f003`会根据账号所在的地区不同而不同。从 backblazeb2 文件浏览中复制文件路径就可以看到对应的域名。

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/DWS_lK-.webp)

### 设置回退源和自定义主机名

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/0d6I1a-.webp)

### 设置转换规则

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/O5hgy-2.webp)

### 修改响应头

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/XsDCUWn.webp)

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/pTyGoxo.webp)

设置静态 Access-Control-Allow-Origin *

删除 backblazeb2 的头

* X-Bz-Upload-Timestamp
* x-bz-content-sha1
* x-bz-file-id
* x-bz-file-name

### SSL/TLS 加密模式为 完全

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/4xbpkc1.webp)

### 设置安全性

参见 [CloudFlare 的 recaptcha 毁了我的 Stack Overflow](https://meta.stackoverflow.com/questions/323537/cloudflare-is-ruining-stack-overflow-for-me-with-its-recaptcha)

安全级别本质上为关

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/fmnFgnb.webp)

质询通过期设置为1年

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/YExMJbY.webp)

### 设置边缘缓存

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/AeY_q3p.webp)

### 开启 HTTP3 和 0-RTT

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/GguSunk.webp)

### 配置浏览器缓存 TTL 为 1年

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/2B7xX1Y.webp)

### 开启Brotli

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/k9P4JUy.webp)

### 启用电子邮件和 Catch-all

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/9Q251XK.webp)

![](https://pub-b8db533c86124200a9d799bf3ba88099.r2.dev/2023/03/W2BUpoG.webp)



