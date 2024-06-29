# 创建实例

### 步骤1：选择集群

选择集群（**优先模式分析与学习集群**），并命名任务。

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

### 步骤2：任务配置

选择所需的GPU数量（建议1到2张卡），并选择镜像，初次使用平台选择`ubuntu20.04_cuda11.2_torch1.11_python3.7_PAL`。该PAL镜像已预装了tmux等常用工具，并设置了root密码为123456，可作为基础镜像使用。

<figure><img src=".gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>



### 步骤3：选择任务释放时间及挂载存储

选择GPU使用时间（训练开始后可手动延长），挂载PAL组共享存储（pal\_share）及个人存储。

<figure><img src=".gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

以上步骤完成后，点击**提交申请**
