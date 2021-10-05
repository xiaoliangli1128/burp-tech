# burp-tech
记录一些burpsuite使用的技巧
## 1. 过滤不需要的网站，不走代理
Burp Suite > Proxy > Options > TLS Pass Through settings:
![图片](https://user-images.githubusercontent.com/66862331/136058410-e80762b9-8664-49e3-9682-06e127a75628.png)

```txt
.*\.google\.com
.*\.gstatic\.com
.*\.googleapis\.com
.*\.pki\.goog
.*\.mozilla\..*
```
以上匹配的网站不会再proxy日志中出现，也不会拦截
