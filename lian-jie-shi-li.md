# 远程连接

### 步骤1:获取IP与端口

在任务列表中点击任务详情查看GPU实例的IP和端口。如图，实例IP为172.18.129.60，端口为37348。

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

### 步骤2:通过SSH软件连接

以[Termius](https://termius.com/) 为例（兼容Windows和macOS），新建连接时输入相应的IP和端口。若使用PAL镜像，用户名和密码分别为root和123456。

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

### 步骤3:文件传输

Termius连接后，点击左侧SFTP支持拖拽上传和下载文件。

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

对于较大文件，请使用SSH命令传输，例如：

* 从本地复制到服务器

`scp -r -P port_number /path/to/local/file username@remote_host:/path/to/remote/directory`

* 从服务器复制到本地

`scp -r -P port_number username@remote_host:/path/to/remote/directory /path/to/local/file`
