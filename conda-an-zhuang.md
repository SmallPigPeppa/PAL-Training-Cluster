---
description: Conda
---

# Conda安装

**确保将Conda安装在个人存储路径中，例如：`/mnt/wenzhuoliu`，该路径是创建实例时个人存储的挂载路径。**

### 步骤1: 获取miniconda安装包路径

获取最新版Miniconda的下载链接，请访问官网（https://docs.anaconda.com/miniconda/），并从其中复制所需的Miniconda下载路径如下：

```
https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

### 步骤2: 在个人存储下安装conda

使用以下命令，通过提供的下载链接将Conda安装到个人存储。**注意修改 `/mnt/wenzhuoliu`为创建实例时个人存储的挂载路径**

```
cd /mnt/wenzhuoliu # 这里修改为你的个人路径
mkdir -p ./miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ./miniconda3/miniconda.sh
bash ./miniconda3/miniconda.sh -b -u -p ./miniconda3
rm -rf ./miniconda3/miniconda.sh
./miniconda3/bin/conda init bash
./miniconda3/bin/conda init zsh
```

### 步骤3:保存个人初始化镜像

因为Conda安装会修改Linux系统中的bash文件，所以完成安装后需要将更改保存为镜像。**在个人存储中安装Conda之后，新建的Conda环境无需再次保存新的镜像。**

在任务详情中点击“创建快照”，即可保存个人镜像。在后续创建实例时，选择此镜像继续使用。请注意为镜像规范命名，命名格式应以“\_用户名”结尾，例如：“ubuntu20.04\_cuda11.2\_torch1.11\_python3.7\_wenzhuoliu”。这样做有助于管理和识别不同用户的镜像。

<figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

&#x20;
