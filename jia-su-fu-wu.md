---
description: >-
  提醒：用户使用中要注意国外网站资源的安全性、以及可能产生的费用情况。面向公众的服务，有法律规定可能不能私自搭建代理，所以考虑后面在所里提供离线安装包、或者建所内的镜像源，以这样方式满足部分最有必要的需求点。
---

# TODO: 加速服务

### 加速服务支持范围 <a href="#undefined" id="undefined"></a>

* [huggingface.co](http://huggingface.co/)
* [github.com](http://github.com/)
* [githubusercontent.com](http://githubusercontent.com/)
* [githubassets.com](http://githubassets.com/)

### &#x20;开启加速 <a href="#undefined" id="undefined"></a>

```
source /etc/proxy/net_prox (TODO)
```

### 关闭加速 <a href="#undefined" id="undefined"></a>

```
unset https_proxy && unset http_proxy
```
