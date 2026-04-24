# CompTIA A+ Core 2 Wrong Answers

用于记录 Core 2 错题、易混概念、简短中文解释和记忆口诀。
后续新错题默认追加到这里。

---

## 使用说明
- 保留题目原文（或浓缩版）
- 保留原题截图
- 记录正确答案
- 写中文简短解析
- 尽量附一句口诀

---
---

## 跨 Windows / macOS / Linux 最广兼容先想 FAT32 + exFAT，不是 NTFS
![Cross-platform filesystems FAT32 exFAT question](images/2026-04-24-core2-cross-platform-filesystems-fat32-exfat.jpg)

**题干：** Which file systems offer the broadest cross-platform compatibility across Windows, macOS, and Linux systems? (Select 2 answers)

|  |  |
| --- | --- |
| ❌ 我的答案 | NTFS |
| ✅ 正确答案 | FAT32 / exFAT |

### 这题最该先抓的核心
题目问的是：
## **broadest cross-platform compatibility**

也就是：
### **跨 Windows、macOS、Linux 最通用、最容易都能认的文件系统**

所以正确答案是：
## **FAT32**
## **exFAT**

---

## 为什么不是 NTFS
**NTFS** 当然在 Windows 里很常见，
功能也强，
但它不是“最广跨平台兼容”那组答案。

因为：
- Windows 对 NTFS 支持最好
- macOS / Linux 对 NTFS 的原生读写兼容性没有 FAT32 / exFAT 那么自然、那么通用

所以题目如果在考：
## **谁最跨平台、最通用**
那优先就不是 NTFS。

---

## 为什么 FAT32 对
### **FAT32 = 老牌通用格式**
它的最大优势就是：
## **兼容性特别广**

几乎各种系统、设备、U 盘、老机器都认。

缺点你也要顺手记：
- **单个文件不能超过 4GB**

所以 FAT32 你可以记成：
## **最老最通用，但有 4GB 限制。**

---

## 为什么 exFAT 对
### **exFAT = 为闪存/移动存储更现代、更方便的大文件方案**

它也很强调：
## **跨平台、移动存储、兼容性强**

相比 FAT32，
它最大的记忆点是：
### **支持更大的文件，不受 4GB 单文件限制**

所以 exFAT 你可以记成：
## **现代 U 盘/移动硬盘跨平台通用格式。**

---

## 为什么其他几个不对
### ext4
- Linux 常见文件系统
- 不属于三大桌面系统里“最广通用”的答案

### APFS
- Apple File System
- 苹果自己的文件系统
- 不是跨 Windows/macOS/Linux 最广兼容

---

## 最简单记忆法
### 跨平台最广兼容就记两兄弟：
## **FAT32 + exFAT**

### 再压缩成一句
- **FAT32** → 老牌万能，但 4GB 限制
- **exFAT** → 现代万能，大文件更友好

---

## 一句话口诀
## **老通用选 FAT32，大文件跨平台选 exFAT；NTFS 强在 Windows，不是最广兼容。**

### 给你一个最好背的版本
## **跨平台看 FAT 家族：FAT32 老万能，exFAT 新万能。**

**一句话：**
这题以后直接这样背：**问最广跨平台兼容，就先想 FAT32 和 exFAT；问 Windows 本地强功能，再想 NTFS。**
---

## Core 2：跨系统共享数据先看文件系统兼容；企业桌面最广泛采用通常还是 Windows
![Cross-platform compatibility and Windows business workstation](images/2026-04-24-core2-cross-platform-and-windows-business.jpg)

### 题 1：不同操作系统之间共享数据，最常见兼容问题来源
**题干：** What is the primary cause of compatibility issues when sharing data between different operating systems?

|  |  |
| --- | --- |
| ❌ 我的答案 | Variations in hardware requirements |
| ✅ 正确答案 | Differences in file system formats |

#### 为什么答案是 file system formats
这题问的是：
## **sharing data between different operating systems**

最根本、最常见的兼容问题之一就是：
### **文件系统格式支持不同**

比如：
- Windows 常见 **NTFS**
- macOS 常见 **APFS**
- Linux 常见 **ext4**
- 跨平台更常见 **FAT32 / exFAT**

所以题目如果在问：
## **跨系统共享数据的 primary cause of compatibility issues**
优先想到：
## **Differences in file system formats**

#### 最短记忆
## **跨系统先看文件系统，不先看硬件。**

---

### 题 2：企业环境里最广泛采用的 workstation OS
![Windows business workstation question](images/2026-04-24-core2-windows-business-workstation-question.jpg)

**题干：** Which workstation operating system is most widely adopted in business environments due to its strong compatibility with enterprise applications, management tools, and network infrastructure?

✅ **正确答案：Windows**

#### 为什么答案是 Windows
这题不是在问：
- 哪个系统最自由
- 哪个系统技术最强
- 哪个最适合服务器

而是在问：
## **企业桌面 / workstation 环境里谁最普及**

在这个语境里，
最标准答案就是：
## **Windows**

因为它在企业桌面生态里的优势是：
- 企业软件兼容性广
- 管理工具成熟
- 和域控/AD/组策略/办公环境整合强

#### 顺手对比
- **Windows** → 企业桌面/workstation 最常见
- **Linux** → 服务器、开发、云、运维更强势
- **macOS** → 设计、创意、Apple 生态、类 Unix 体验更有优势

#### 最短记忆
## **桌面企业看 Windows，服务器开发看 Linux。**

---

## 你顺手问的：那 macOS 的优势是什么？
这个可以这样简短记：

### macOS 常见优势
#### 1. Apple 生态整合好
- iPhone / iPad / AirDrop / iCloud / Handoff 配合顺

#### 2. 界面和体验稳定统一
- 硬件软件一体化
- 机器和系统配合通常比较顺手

#### 3. 创意/设计类用户很多
- 设计、视频、音乐、内容创作人群常见

#### 4. 兼顾桌面易用性 + Unix 底子
- 图形桌面友好
- 底层又有类 Unix 环境，开发者也喜欢

### 一句话记法
## **Windows 强企业桌面，Linux 强服务器开发，macOS 强 Apple 生态与创意体验。**

**一句话：**
这两题你可以一起记：**跨系统共享先看文件系统格式；企业桌面最广泛采用通常是 Windows。与此同时，macOS 的优势更多在 Apple 生态整合、体验统一，以及创意工作和类 Unix 开发环境。**
---

## 分区的好处：整理数据、支持 multiboot、也更方便备份恢复；不会让硬盘“变大”
![Partitions benefits backup recovery question](images/2026-04-24-core2-partitions-benefits-backup-recovery.jpg)

**题干：** What are the key benefits of dividing a storage drive into multiple partitions? (Select 3 answers)

|  |  |
| --- | --- |
| ✅ 我答对的 | Improved data organization |
| ✅ 我答对的 | Support for multiboot environments |
| ❌ 我的错误答案 | Larger physical disk capacity utilization |
| ✅ 漏掉的正确答案 | Simplified backup and recovery |

### 这题最容易错的点
你前两个其实已经抓得很准：
- **Improved data organization** ✅
- **Support for multiboot environments** ✅

你错在把：
- **Larger physical disk capacity utilization**
当成了分区的好处。

但分区：
## **不会让硬盘物理容量变大，也不会凭空提高物理容量利用率。**

---

## 为什么 Simplified backup and recovery 是对的
因为分区后你可以把：
- 系统
- 数据
- 其他用途

分开存放。

这样带来的一个实际好处就是：
## **备份和恢复更方便**

比如：
- 只备份数据分区
- 系统坏了重装时不一定要动数据分区
- 恢复系统和恢复资料可以分开处理

所以：
### **Simplified backup and recovery**
是合理的分区好处。

---

## 为什么 physical disk capacity 那项不对
因为分区只是：
## **把同一块盘切成逻辑区域**

它做的是逻辑划分，
不是物理扩容。

所以：
- 500GB 分成 2 个分区，还是 500GB
- 1TB 分成 4 个分区，也还是 1TB

### 分区能改善组织方式
### 但不能增加容量本身

---

## 为什么 faster data transfer speeds 也不对
分区本身不是加速技术。
它不会天然让：
- 磁盘变快
- 传输速率上升

所以这项也不是标准好处。

---

## 最简单记忆法
### 分区三大好处先记：
## **好整理**
## **能多系统启动**
## **更方便备份恢复**

不要乱加：
## **容量变大**
## **速度变快**

---

## 一句话口诀
## **分区帮你分门别类、双系统启动、备份恢复更轻松；但不加容量，也不直接加速。**

### 再压缩一句
## **分区管组织，不管扩容。**

**一句话：**
这题以后就这样背：**partition 的好处是整理、multiboot、备份恢复方便；它不会让硬盘容量更大，也不是提速手段。**
---

## 安装系统时 NVMe 盘检测不到：先想安装程序缺驱动，题库标准答案是加载第三方 NVMe 驱动，不是先刷 BIOS
![NVMe OS install load third-party drivers question](images/2026-04-24-core2-nvme-os-install-load-third-party-drivers.jpg)

**题干：** A technician is attempting to install a new operating system on a recently assembled custom workstation. During the installation process, the installer fails to detect the installed NVMe solid-state drive, preventing the installation from proceeding. All physical connections to the NVMe drive have been verified as secure. What should the technician do to resolve this problem?

|  |  |
| --- | --- |
| ❌ 我的答案 | Update the workstation's BIOS/UEFI firmware |
| ✅ 正确答案 | Load the appropriate third-party NVMe drivers from external media |

### 这题为什么容易错
因为你看到：
- **recently assembled custom workstation**
- **installer fails to detect NVMe SSD**

很容易第一反应就怀疑：
## **BIOS/UEFI 太旧，不支持 NVMe**

这个现实里不是完全没可能，
但这题题库更标准的落点是：
## **安装程序缺少对应 NVMe 驱动**

所以标准答案是：
### **Load the appropriate third-party NVMe drivers from external media**

---

## 为什么正确答案是“加载驱动”
题目说的是：
## **during the installation process, the installer fails to detect the drive**

这类题在考试里常常是在考：
- 安装程序本身缺少存储控制器/NVMe 驱动
- 需要手动从外部介质加载驱动

也就是说：
### **盘可能物理上没问题，BIOS 也未必有问题，只是安装器暂时不认它。**

这时候最标准的动作就是：
## **load third-party NVMe drivers**

---

## 为什么 BIOS/UEFI firmware 这题没中
### Update the workstation's BIOS/UEFI firmware
这在现实故障排查里是一个合理方向，
但不是题库这里最直接、最优先的标准答案。

因为题目没有明确给你：
- 主板过旧
- 固件版本过老
- NVMe support 缺失

它更像是在考：
## **安装阶段识别不到存储设备 → 先补驱动**

所以这题先不要把脑子带到“刷 BIOS”上。

---

## 为什么 boot order 不对
因为现在的问题不是：
### **从哪块盘启动**

而是：
### **安装程序压根没看到那块 NVMe 盘**

既然安装器都看不到，
那先调 boot order 没有解决核心问题。

---

## 为什么选不同 drive 不对
因为题目没有说：
- 还有别的可用目标盘
- 当前盘不适合安装

而是在问：
### **怎么解决 NVMe 盘检测不到的问题**

所以“换盘选”不是核心处理。

---

## 最简单记忆法
### 安装系统时遇到：
- **installer 看不到 NVMe / storage device**
- **物理连接已确认没问题**

优先想到：
## **先加载存储/NVMe 驱动**

不要第一反应就：
## **刷 BIOS**

---

## 一句话口诀
## **安装器不认盘，先补驱动；能进系统后再谈固件。**

### 再压缩一句
## **看不到 NVMe 先想驱动，不先想 BIOS。**

**一句话：**
这题以后直接这样背：**安装系统时如果 installer 检测不到 NVMe，而物理连接已确认正常，题库标准处理优先是加载第三方 NVMe 驱动。**
---

## 对，这题和 NVMe 那题同一路：安装器看不到 RAID，先加载 RAID 驱动，不先换控制器
![RAID OS install load third-party drivers question](images/2026-04-24-core2-raid-os-install-load-third-party-drivers.jpg)

**题干：** During the installation of a new operating system on a custom-built PC, the installer fails to detect the RAID array configured on the system. What is the most appropriate action to resolve this issue?

|  |  |
| --- | --- |
| ❌ 我的答案 | Replace the RAID controller with a compatible model |
| ✅ 正确答案 | Load the appropriate third-party RAID drivers from external media |

### 对，这题和上一题本质是同一路
你这个总结是对的：
## **安装器看不到 RAID / NVMe 这类存储目标时，题库很爱考“先加载驱动”。**

也就是：
- **看不到 NVMe** → 先补 NVMe 驱动
- **看不到 RAID array** → 先补 RAID 驱动

---

## 为什么答案是加载 RAID 驱动
题目最关键的词是：
- **during the installation of a new operating system**
- **installer fails to detect the RAID array**

这很像在说：
## **安装程序本身没有对应 RAID controller / storage driver**

所以最合适的动作就是：
### **Load the appropriate third-party RAID drivers from external media**

也就是让安装器先“认得出”这个 RAID 阵列。

---

## 为什么不是更换 RAID controller
你选的是：
### **Replace the RAID controller with a compatible model**

这个太重了，
也不是 first / most appropriate action。

因为题目没有说：
- RAID controller 损坏
- controller 不兼容
- 阵列配置错误

它更像是在考：
## **安装程序缺驱动，暂时识别不到控制器/阵列**

所以直接换控制器属于：
### **过度处理**

---

## 为什么 BIOS update 也没中
和上一题 NVMe 很像。

更新 BIOS 当然有时现实里可能有帮助，
但题库更标准的答案通常是：
## **先加载存储控制器驱动**

因为题目重点落在：
### **installer fails to detect**
不是：
### **固件完全不支持**

---

## 为什么“选别的盘”不对
因为题目不是在问：
- 还有没有别的安装目标

而是在问：
### **如何解决 installer 看不到 RAID array 的问题**

所以换盘不是根本解决思路。

---

## 最简单记忆法
### 安装系统时如果：
- 看不到 **NVMe**
- 看不到 **RAID array**
- 物理层/阵列已配置好

优先想到：
## **加载第三方存储驱动**

---

## 一句话口诀
## **安装器不认存储目标，先补控制器驱动；别一上来刷 BIOS，更别直接换硬件。**

### 再压缩成一句
## **OS 安装看不到盘，先加载驱动。**

**一句话：**
对，这题你可以和上一题绑着背：**安装系统时如果 installer 看不到 RAID 或 NVMe，题库标准答案通常是先从外部介质加载对应第三方驱动。**
---

## 恢复出厂设置且不靠外部介质，先想 recovery partition；system restore 不是重置到 factory settings
![Recovery partition vs System Restore question](images/2026-04-24-core2-recovery-partition-vs-system-restore.jpg)

**题干：** Which of the following answers refers to a built-in solution for restoring an operating system to its factory settings without the use of external media?

|  |  |
| --- | --- |
| ❌ 我的答案 | System restore |
| ✅ 正确答案 | Recovery partition |

### 这题最容易混的点
你会选 **System restore** 很正常，
因为它听起来就像：
## **恢复系统**

但题目问得更具体：
### **restoring an operating system to its factory settings**
而且还强调：
### **without the use of external media**

这两个关键词一组合，
标准答案就变成：
## **Recovery partition**

---

## 为什么答案是 recovery partition
### **Recovery partition = 恢复分区**
它通常是机器/系统预先内建在本地磁盘上的恢复环境，
用来：
- 恢复出厂设置
- 重置系统到初始状态
- 不需要额外 U 盘 / 光盘 / 外部安装介质

所以题目说：
## **built-in solution**
## **factory settings**
## **without external media**

这就是 recovery partition 的经典描述。

---

## 为什么 system restore 不对
### **System Restore**
更像是：
## **把系统状态回滚到之前的一个还原点**

它主要恢复的是：
- 系统文件
- 注册表
- 某些配置状态

它不是：
## **把系统恢复到出厂设置**

也就是说：
- **System Restore** → 回到之前某个系统状态
- **Recovery Partition** → 回到更接近出厂/初始恢复环境

所以这题不能选 System Restore。

---

## 为什么 disk imaging 不对
### **Disk imaging**
更像：
- 做整盘镜像备份
- 用镜像恢复系统

但题目强调的是：
## **built-in solution without external media**

它不是在问“备份镜像技术”，
而是在问机器本机自带的恢复机制。

---

## 为什么 shadow copy 不对
### **Shadow copy**
更偏：
- 文件/卷快照
- 版本副本
- 便于恢复某些文件版本

它不是“恢复到 factory settings”的标准答案。

---

## 最简单记忆法
### 题目如果问：
- **factory settings**
- **built-in solution**
- **no external media**

优先想到：
## **Recovery partition**

### 顺手区分
- **System Restore** → 还原点回滚
- **Recovery Partition** → 出厂恢复/重置系统
- **Disk Imaging** → 镜像备份恢复
- **Shadow Copy** → 快照/文件版本

---

## 一句话口诀
## **还原点选 System Restore，恢复出厂选 Recovery Partition。**

### 再压一句
## **factory settings 不看 restore point，看 recovery partition。**

**一句话：**
这题以后直接这样背：**System Restore 是回滚到还原点，不是恢复出厂；问 built-in factory reset without external media，就选 Recovery Partition。**
---

## 无盘工作站每次开机都从网络拉系统镜像，先想 PXE；SMB/NFS 是共享协议，不是“网启”本身
![PXE network boot diskless workstations question](images/2026-04-24-core2-pxe-network-boot-diskless-workstations.jpg)

**题干：** An organization wants to automate the deployment of operating systems on dozens of diskless workstations that do not have any local storage. The workstations must boot directly from the network every time they power on, retrieving the OS image from a central server without any local media involved. Which technology allows this network boot and OS loading process?

|  |  |
| --- | --- |
| ❌ 我的答案 | SMB |
| ✅ 正确答案 | PXE |

### 这题最关键的词
- **diskless workstations**
- **boot directly from the network every time**
- **retrieving the OS image from a central server**
- **without any local media**

只要看到：
## **从网络启动 / 网启 / boot directly from the network**

第一反应就该是：
## **PXE**

---

## 为什么答案是 PXE
### **PXE = Preboot eXecution Environment**
它就是用来：
## **通过网卡启动系统，并从网络获取启动/安装映像**

这题里无盘工作站：
- 没本地存储
- 没本地介质
- 每次都从网络开机

这完全就是 PXE 的经典应用场景。

---

## 为什么你选的 SMB 不对
### **SMB = Server Message Block**
它是：
## **文件共享协议**

也就是说 SMB 更偏：
- 共享文件夹
- 访问共享目录
- 传文件

但它不是：
## **让机器开机时通过网卡直接启动的技术**

所以这题不能选 SMB。

---

## 为什么 NFS 也不对
### **NFS = Network File System**
和 SMB 一样，
它也是：
## **网络文件共享协议**

它能共享文件，
但不是“网络引导启动机制”本身。

---

## 为什么 WDS 这题也没中
### **WDS = Windows Deployment Services**
它和网络部署 Windows 确实有关，
但题目问的是：
## **哪一种 technology allows this network boot and OS loading process**

更底层、更核心的“网络启动”技术是：
## **PXE**

你可以这样区分：
- **PXE** → 网启机制
- **WDS** → 利用 PXE 等方式进行 Windows 部署的服务

---

## 最简单记忆法
### 看到这些词：
- **network boot**
- **diskless workstation**
- **boot from network**
- **no local media**

优先想到：
## **PXE**

### 顺手区分
- **PXE** → 网络启动
- **SMB / NFS** → 文件共享
- **WDS** → Windows 部署服务

---

## 一句话口诀
## **网启看 PXE，共享看 SMB/NFS，Windows 批量部署才想 WDS。**

### 再压一句
## **从网络开机 = PXE，不是共享协议。**

**一句话：**
这题以后直接这样背：**无盘工作站每次从网络开机、拉系统镜像，核心技术就是 PXE；SMB/NFS 只是共享协议，不是网启本身。**
---

## Multiboot 不是“同时运行多个系统”，而是开机时选一个系统；常见用途是不同系统做不同任务
![Multiboot use case specific tasks question](images/2026-04-24-core2-multiboot-use-case-specific-tasks.jpg)

**题干：** What is the most common use case for a multiboot configuration?

|  |  |
| --- | --- |
| ❌ 我的答案 | Running multiple operating systems simultaneously |
| ✅ 正确答案 | Utilizing different operating systems for specific tasks |

### 这题你错的根本原因
你把：
## **multiboot**
和
## **virtualization / multiple OS simultaneously**
混了。

这是非常常见的错法。

---

## 为什么正确答案是“for specific tasks”
### **Multiboot** 的意思是：
- 一台机器装多个操作系统
- **开机时选其中一个进去**
- 不是同时并行运行

所以它的最常见用途就是：
## **不同系统做不同任务**

比如：
- Windows 打游戏 / 跑某些办公软件
- Linux 做开发 / 安全实验 / 学习
- 老版本系统保留某些特定用途

这就是：
### **Utilizing different operating systems for specific tasks**

---

## 为什么“simultaneously”不对
你选的是：
### **Running multiple operating systems simultaneously**

这个更像：
## **虚拟化（virtualization）**

也就是：
- host OS 里再跑 guest OS
- 多个系统同时在线
- 同时运行

但 multiboot 不是这样。

### Multiboot 的关键词是：
## **boot 时选一个，不是一起跑。**

---

## 为什么其他两个不是最常见 use case
### Keeping legacy software operational in a controlled environment
这个也可能是用途之一，
但题目问的是：
## **most common use case**

更通用、更标准的答案还是：
### **不同 OS 处理不同任务**

### Isolating potentially harmful software away from the main OS
这更像：
- sandbox
- VM
- 隔离测试环境

不是 multiboot 最典型的 primary use case。

---

## 最简单记忆法
### Multiboot 就记一句：
## **一台机器多个系统，但一次只进一个。**

### 顺手对比
- **Multiboot** → 开机选一个系统
- **Virtualization** → 多系统可同时运行

---

## 一句话口诀
## **多系统同时跑看虚拟化，开机选一个看 multiboot。**

### 再压缩一句
## **Multiboot 管“切换”，不是管“同时”。**

**一句话：**
这题以后直接这样背：**multiboot 最常见用途是让不同操作系统承担不同任务；如果题目说 simultaneously，那通常更像 virtualization，不是 multiboot。**

