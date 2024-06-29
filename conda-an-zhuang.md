---
description: Conda
---

# Conda安装

**确保将Conda安装在个人磁盘路径中，例如：`/mnt/wenzhuoliu`，该路径是创建实例时个人磁盘的挂载路径。**

### 步骤1: 获取miniconda安装包路径

获取最新版Miniconda的下载链接，请访问官网（https://docs.anaconda.com/miniconda/），并从其中复制所需的Miniconda下载路径如下：

```
https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

### 步骤2: 在个人存储下安装conda

使用以下命令，通过提供的下载链接将Conda安装到个人存储。**注意修改 `/mnt/wenzhuoliu`为创建实例时个人磁盘的挂载路径**

<pre><code><strong>cd /mnt/wenzhuoliu # 这里修改为你的个人路径
</strong><strong>mkdir -p ./miniconda3
</strong><strong>wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ./miniconda3/miniconda.sh
</strong><strong>bash ./miniconda3/miniconda.sh -b -u -p ./miniconda3
</strong><strong>rm -rf ./miniconda3/miniconda.sh
</strong></code></pre>
