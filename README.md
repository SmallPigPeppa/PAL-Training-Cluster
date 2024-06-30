# 管理员需求

### 需求1：用户管理需求

团队管理员需要对组内普通用户的使用进行监控和管理。

* 监控功能：需要团队管理员能够查看组内普通用户正在执行的任务（包含任务名称、占用卡数等信息）。
* **管理功能：需要团队管理员能够杀死普通用户某个正在执行的任务。**
* **卡时管理：需要团队管理员能够给普通用户设置固定时间的固定卡时限额（例如：每两周每个普通用户仅有200元的卡时，两周限额定期刷新）。**

监控功能：当前平台支持该功能。

管理功能：团队管理员停止普通用户任务功能（技术可行，需要开发）。

卡时管理：管理员配置团队下用户卡时限制功能（技术可行，需要开发）。



### 需求2：团队存储需求

* 存储拓展：团队成员的个人系统盘容量为200GB，**建议拓展为500GB。**
* 共享存储：为应对大规模数据和预训练模型的存储需求，需要**创建一个容量更大的团队共享数据盘（`/mnt/pal_share`）**。
* 权限控制：为防止数据误删除，应限制数据盘的访问权限，保证普通用户只有读权限，管理员可根据需要**临时授权普通用户写权限以上传数据**。

存储拓展：当前平台支持该功能，购买存储需要等到7月份。

存储拓展：当前平台支持该功能，团队管理员可以创建超过200GB共享存储。

权限控制：探索技术方案的可行性，一种替代方法是由管理员负责上传数据。

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

### 需求3：团队镜像需求

* 镜像隔离：建议采取措施实现用户镜像隔离，仅共享的镜像对所有用户可见，以增强数据安全性和隐私保护。**各用户私有镜像互不可见。**
* 镜像管理：管理员可以**制作并发布团队镜像。**

镜像隔离：技术可行，需要开发。

镜像管理：技术可行，需要开发。

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
