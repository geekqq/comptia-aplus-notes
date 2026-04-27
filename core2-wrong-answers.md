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
---

## Internet-based OS installation 先想“外网/云/厂商下载”，不要和 PXE/LAN 大规模部署混掉
![Internet-based OS installation vs network deployment question](images/2026-04-24-core2-internet-based-os-installation-vs-network-deployment.jpg)

**题干：** Which of the answers listed below describe characteristics of an internet-based OS installation method? (Select 2 answers)

|  |  |
| --- | --- |
| ❌ 我的答案 | Optimized for mass deployment with standardized configuration across multiple systems |
| ❌ 我的答案 | Commonly deployed via PXE/DHCP/TFTP protocols |
| ✅ 漏掉的正确答案 | Primarily suited for single users, remote workers, or when local network infrastructure is not available |
| ✅ 漏掉的正确答案 | Relies on external servers, cloud services, or vendor websites for installation files |

### 这题为什么会错
因为你把：
## **internet-based installation**
和
## **network/PXE mass deployment**
混在一起了。

它们都带“network”味道，
所以特别容易串。

---

## Internet-based installation 真正的特征是什么
### 1. Relies on external servers, cloud services, or vendor websites for installation files
这就是最核心定义。

也就是：
- 安装文件来自外部服务器
- 来自云端
- 来自厂商网站
- 依赖互联网获取镜像/安装资源

所以：
## **external servers / cloud / vendor websites**
一定是对的。

### 2. Primarily suited for single users, remote workers, or when local network infrastructure is not available
因为这种安装方式不依赖企业内网部署体系，
所以更适合：
- 单个用户
- 远程办公用户
- 没有本地 LAN 部署环境时

所以这项也是标准答案。

---

## 为什么你选的那两项不对
### 1. Optimized for mass deployment with standardized configuration across multiple systems
这更像：
## **企业内网批量部署 / 镜像标准化部署**

也就是：
- 大规模统一装机
- 多台机器标准化配置
- IT 批量部署场景

这不是 internet-based installation 最典型的标签。

### 2. Commonly deployed via PXE/DHCP/TFTP protocols
这个更是明显在说：
## **PXE 网络部署 / 内网启动安装**

也就是：
- 本地网络
- DHCP
- TFTP
- PXE boot

这更像：
## **network-based / LAN-based deployment**

不是这题的 **internet-based**。

---

## 最简单对照记忆
### Internet-based installation
- 外部服务器 / 云端 / 厂商网站
- 单用户 / 远程用户 / 没有本地部署环境

### PXE / network deployment
- 内部服务器
- 本地网络
- PXE / DHCP / TFTP
- 批量部署

---

## 最方便记忆的方法
## **Internet-based = 从外网拿文件**
## **PXE-based = 从内网开机装系统**

---

## 一句话口诀
## **外网装系统看 cloud/vendor；内网批量装机看 PXE/DHCP/TFTP。**

### 再压缩一句
## **单机远程走互联网，批量部署走本地网。**

**一句话：**
这题以后就这样背：**internet-based OS installation 强调外部服务器/云端/厂商下载，适合单用户和远程用户；PXE/DHCP/TFTP 那套属于本地网络批量部署，不是 internet-based。**
---

## NetBT = NetBIOS over TCP/IP，这题是 True；看到 NetBT 就想到“让 NetBIOS 跑在 TCP/IP 上”
![NetBT NetBIOS over TCP/IP question](images/2026-04-24-core2-netbt-netbios-over-tcp-ip-true.jpg)

**题干：** The function of the NetBT protocol is to allow NetBIOS services to be used over TCP/IP networks.

|  |  |
| --- | --- |
| ❌ 我的答案 | False |
| ✅ 正确答案 | True |

### 这题其实就是缩写题
你只要把这个缩写拆开，
题目就几乎等于白送：

## **NetBT = NetBIOS over TCP/IP**

也就是：
### **让 NetBIOS 服务可以运行在 TCP/IP 网络上。**

所以题干说：
> allow NetBIOS services to be used over TCP/IP networks

这句话本身就是：
## **True**

---

## NetBIOS / NetBT 最简单怎么理解
### NetBIOS
是比较老的一套网络服务/接口概念，
常见和：
- 名称解析
- 会话服务
- 局域网共享

这些东西联系在一起。

### NetBT
就是把：
## **NetBIOS 这套服务搬到 TCP/IP 上跑**

所以你可以把它直接记成：
## **NetBIOS over TCP/IP 的桥梁/封装方式**

---

## 为什么这题容易反应不过来
因为如果你没把：
### **NetBT**
和
### **NetBIOS over TCP/IP**
直接绑定，
那它看起来就像一个陌生缩写。

一旦绑定之后，
这题就会变成：
## **定义题**

---

## 顺手再和相关端口一起记
如果题目再延伸到老式 NetBIOS 服务，
常见会想到：
- **137** → NetBIOS Name
- **138** → NetBIOS Datagram
- **139** → NetBIOS Session

所以你可以把它们顺手串起来：
## **NetBT = 让 NetBIOS 这些服务跑在 TCP/IP 网络里。**

---

## 最简单记忆法
## **NetBT 看到 BT，不是蓝牙；它是 NetBIOS over TCP/IP。**

### 一句话口诀
## **NetBT = NetBIOS 搭 TCP/IP。**

### 再压缩一句
## **看到 NetBT，就判断：它就是把 NetBIOS 放到 TCP/IP 上跑。**

**一句话：**
这题以后直接秒杀：**NetBT 的作用就是让 NetBIOS services 能在 TCP/IP 网络上使用，所以题目是 True。**
---

## Windows 11 最容易漏的硬性门槛：TPM 2.0；32GB 存储不是这题标准答案
![Windows 11 minimum requirements TPM 2.0 Secure Boot 64-bit CPU question](images/2026-04-24-core2-windows11-minimum-requirements-tpm-2-secure-boot-64bit-cpu.jpg)

**题干：** Which of the following are minimum requirements for installing Windows 11? (Select 3 answers)

|  |  |
| --- | --- |
| ✅ 我答对的 | UEFI firmware with Secure Boot |
| ✅ 我答对的 | 64-bit processor listed on Microsoft’s Windows 11 compatibility list |
| ❌ 漏掉的正确答案 | TPM version 2.0 support |
| ❌ 我的错误答案 | A minimum of 32 GB of available storage space |

### 这题最该先抓的门槛
## **Windows 11 = Secure Boot + TPM 2.0 + 合规 64-bit CPU**

你前两个已经抓对了：
- **UEFI firmware with Secure Boot** ✅
- **64-bit processor on the compatibility list** ✅

你最容易漏掉的就是：
## **TPM 2.0 support**

---

## 为什么 TPM 2.0 是对的
Windows 11 跟以前版本一个很明显的区别就是：
## **更强调安全硬件门槛**

其中最爱考的就是：
### **TPM 2.0**

它几乎已经成了 Windows 11 题的“招牌关键词”。

所以以后只要看到：
## **Windows 11 minimum requirements**
优先脑内跳出来：
- **TPM 2.0**
- **Secure Boot / UEFI**
- **64-bit supported CPU**

---

## 为什么 32 GB 这题没中
你选的：
### **A minimum of 32 GB of available storage space**

它看起来很像“以前 Windows 安装题”的常见选项，
所以很容易被选进去。

但这题按当前题库标准，
它没有把这项列进你这道题的正确三项里。

换句话说，
这题最稳的考法更偏：
## **Windows 11 的三大硬门槛：TPM 2.0、Secure Boot、受支持 CPU**

所以你记忆时不要让存储容量抢走注意力。

---

## 为什么 2 GB RAM 明显不对
这个你没选是对的。
因为 Windows 11 不可能只要 2 GB RAM。

这种选项一般就是拿来当干扰项。

---

## 最简单记忆法
### Windows 11 三件套直接死记：
## **TPM 2.0**
## **UEFI + Secure Boot**
## **受支持的 64-bit CPU**

### 一句话口诀
## **Win11 三道门：TPM 2.0、Secure Boot、64-bit 合规 CPU。**

### 再压缩一句
## **看到 Windows 11 requirements，先锁 TPM 2.0。**

**一句话：**
这题以后就这样背：**Windows 11 最常考的三个最低要求是 TPM 2.0、UEFI Secure Boot、以及受支持的 64-bit 处理器；TPM 2.0 是最容易漏掉的那个。**
---

## Task Manager 最核心四件事：看运行、看资源、管启动、结束卡死程序；不管计划任务和用户权限
![Task Manager functions running startup resources end task question](images/2026-04-24-core2-task-manager-functions-running-startup-resources-end-task.jpg)

**题干：** Which of the answers listed below describe(s) the function of Task Manager (taskmgr.exe) in Windows 10 and Windows 11? (Select all that apply)

**正确答案：**
- **Displays information on programs, processes, and services that are currently running on the computer**
- **Provides access to startup applications that can be enabled or disabled to launch automatically at sign-in**
- **Provides real-time reports on how a Windows-based computer is using system resources, such as CPU, RAM, Disk, Network, and GPU**
- **Allows users to close a non-responsive application in Windows**

### 你这题其实已经会了 75%
你已经选对了三项：
- **running programs / processes / services** ✅
- **startup applications** ✅
- **real-time resource reports** ✅

你漏掉的是：
- **Allows users to close a non-responsive application in Windows** ✅

这项其实也是 Task Manager 最经典、最直觉的用途之一。

---

## 为什么这个漏掉最可惜
因为很多人对 Task Manager 的第一反应就是：
## **程序卡死了，去 Task Manager 里 End task**

所以：
### **Allows users to close a non-responsive application in Windows**
是非常标准、非常基础的 Task Manager 功能。

这题漏它，
就等于把 Task Manager 最招牌的功能忘掉了。

---

## Task Manager 最核心到底是哪四件事
你以后就把它固定背成四件事：

### 1. 看当前运行内容
- 程序
- 进程
- 服务

### 2. 看系统资源占用
- CPU
- RAM
- Disk
- Network
- GPU

### 3. 管启动项
- 开机自启程序启用/禁用

### 4. 杀掉卡死程序
- **End task**

---

## 为什么其他几个不对
### Provides access to administrative tools for managing network traffic
这更像：
- 专门网络管理工具
- 高级网络监控/管理工具

不是 Task Manager 的标准定义。

### Allows users to schedule the launch of programs or scripts at pre-defined times
这个是：
## **Task Scheduler（任务计划程序）**
不是 Task Manager。

### Allows system administrators to modify user account permissions
这个更像：
- 用户管理
- 本地安全策略
- 账户权限配置

不是 Task Manager 的功能。

---

## 最简单记忆法
### Task Manager = 四件事
## **看运行**
## **看资源**
## **管启动**
## **杀卡死**

不要混到：
- **Task Scheduler**（定时任务）
- **User permissions**（用户权限）
- **高级网络管理**

---

## 一句话口诀
## **Task Manager 看运行、看资源、管启动、杀卡死；定时任务去 Scheduler。**

### 再压缩一句
## **程序卡死先开 Task Manager，不是去改权限。**

**一句话：**
这题以后直接背 Task Manager 的四大功能：**看运行进程、看资源占用、管理启动项、结束无响应程序。**
---

## lusrmgr.msc = Local Users and Groups，能管本地用户和组；但 Home 版通常没有，这题是 True
![Local Users and Groups lusrmgr true not home question](images/2026-04-24-core2-local-users-and-groups-lusrmgr-true-not-home.jpg)

**题干：** In Microsoft Windows, Local Users and Groups (lusrmgr.msc) is an MMC snap-in for adding or removing users and managing group membership for users who have specific rights and permissions on a Windows system. The Local Users and Groups utility is not included in Home editions of Windows 10 and Windows 11.

|  |  |
| --- | --- |
| ❌ 我的答案 | False |
| ✅ 正确答案 | True |

### 这题最该直接记住的点
## **lusrmgr.msc = Local Users and Groups**
它就是 Windows 里的一个：
### **MMC snap-in**

主要用来：
- 管理本地用户
- 管理本地组
- 调整组成员关系

所以题目前半句本身就是对的。

---

## 为什么后半句也是对的
题目后半句说：
### **The Local Users and Groups utility is not included in Home editions of Windows 10 and Windows 11.**

这也是题库常考点：
## **Home 版通常没有这个本地用户和组管理器。**

也就是说：
- **Pro / Enterprise / 更高版本** 更常见这个工具
- **Home 版** 往往没有完整提供这个 MMC 工具

所以整句话判定就是：
## **True**

---

## 为什么你容易误判成 False
因为这题前半句很长，
后半句又补了一个版本差异，
很容易让人怀疑：
- “会不会有一句是错的？”
- “是不是 Home 版也有？”

但这题真正要你记的就是两件事：
1. **lusrmgr.msc 是管本地用户和组的 MMC snap-in**
2. **Home 版通常不带它**

这两个都成立，
所以答案就是：
## **True**

---

## 最简单记忆法
### lusrmgr.msc 先拆词
- **usr** → users
- **mgr** → manager

你就把它记成：
## **本地用户和组管理器**

### 再补一句版本差异
## **Home 没它，Pro 更常见。**

---

## 一句话口诀
## **lusrmgr 管本地用户组，Home 版通常没有。**

### 再压缩一句
## **看到 lusrmgr.msc，就想到 Local Users and Groups。**

**一句话：**
这题以后直接背：**lusrmgr.msc 就是本地用户和组管理器（MMC snap-in），而且 Windows 10/11 Home 版通常不包含它，所以这题是 True。**
---

## 启动故障排查先想 msconfig.exe，不是 sysdm.cpl；sysdm 偏系统属性，msconfig 偏启动配置
![msconfig startup troubleshooting question](images/2026-04-24-core2-msconfig-startup-troubleshooting.jpg)

**题干：** Which of the following refers to a Microsoft Windows tool designed for troubleshooting system startup problems?

|  |  |
| --- | --- |
| ❌ 我的答案 | sysdm.cpl |
| ✅ 正确答案 | msconfig.exe |

### 这题最关键的对比
你这题不是完全不会，
而是把两个 Windows 工具的用途混了：
- **sysdm.cpl**
- **msconfig.exe**

其中真正偏：
## **启动问题排查**
的是：
## **msconfig.exe**

---

## 为什么答案是 msconfig.exe
### **msconfig.exe = System Configuration**
它最经典的用途就是：
- 排查启动问题
- 调整启动配置
- 控制启动项/服务的加载方式
- 进行选择性启动 / diagnostic startup

所以题目问：
## **tool designed for troubleshooting system startup problems**

最标准答案就是：
## **msconfig.exe**

---

## 为什么 sysdm.cpl 不对
### **sysdm.cpl = System Properties**
它更偏：
- 计算机名
- 系统保护
- 高级系统设置
- 环境变量
- 性能设置入口
- 远程设置

也就是说：
## **它是系统属性配置工具**
不是专门拿来做“启动故障排查”的代表答案。

你会选它，
多半是因为它也长得很“系统底层”，
但它不是这题最贴的那个。

---

## 为什么另外两个不对
### eventvwr.msc
- 事件查看器
- 可以看日志
- 对排错有帮助
- 但题目问的是“designed for troubleshooting startup problems”的工具名
更标准还是 **msconfig**

### compmgmt.msc
- 计算机管理
- 是综合管理控制台
- 能进很多管理模块
- 也不是这题最直接的“启动故障排查工具”

---

## 最简单记忆法
### Windows 启动故障题先记：
## **msconfig = 启动配置/启动排错**

### 顺手对比
- **msconfig.exe** → 启动配置、启动排错
- **sysdm.cpl** → 系统属性
- **eventvwr.msc** → 事件查看器
- **compmgmt.msc** → 计算机管理

---

## 一句话口诀
## **启动排错找 msconfig，系统属性找 sysdm。**

### 再压缩一句
## **msconfig 管启动，sysdm 管系统属性。**

**一句话：**
这题以后直接这样背：**Windows 里排查启动问题最典型的工具是 msconfig.exe；sysdm.cpl 是系统属性，不是启动排错工具。**
---

## msconfig 的 Boot tab 不只管 Safe boot，还能管 boot logging、默认启动系统、以及资源限制；startup items 不在 Boot tab
![msconfig Boot tab settings question](images/2026-04-24-core2-msconfig-boot-tab-safe-boot-boot-logging-multiboot-memory.jpg)

**题干：** Which of the settings listed below can be managed through the Boot tab of the System Configuration utility in Windows? (Select all that apply)

**正确答案：**
- **Safe boot, including an option to load minimal drivers and services for troubleshooting during system startup**
- **Boot logging, which collects detailed information about the startup process for diagnostic purposes**
- **Selecting the default operating system to load in a multiboot environment**
- **Limits on hardware resources, such as maximum RAM, allocated to the selected OS in a multiboot environment**

**错误选项：**
- **Startup items, including programs and services set to launch automatically during system boot**

### 这题你其实已经抓对一半以上了
你答对了：
- **Safe boot** ✅
- **Selecting the default operating system in a multiboot environment** ✅

你漏掉了：
- **Boot logging** ✅
- **Limits on hardware resources (like max RAM)** ✅

你错选的是：
- **Startup items** ❌

---

## 这题最关键的思路
### **Boot tab = 跟“启动方式、启动日志、多系统启动、启动参数限制”有关**

不是：
### **普通程序自启动管理页**

也就是说，
Boot tab 关注的是：
- 怎么启动
- 启动时记录什么
- 启哪个系统
- 启动时给这个系统加什么限制/参数

---

## 为什么 boot logging 是对的
这个很容易漏。

在 msconfig 的 Boot 相关选项里，
**boot log / boot logging** 是很典型的排错功能，
用来：
## **记录启动过程细节，帮助诊断问题**

所以它属于 Boot tab 管的内容。

---

## 为什么 hardware resource limits 也是对的
这个更容易被忽略。

msconfig 的 Boot 相关高级选项里，
可以做一些启动资源限制类设置，
比如：
- 最大内存（maximum memory）
- 处理器数量（number of processors）

所以题目里说：
### **Limits on hardware resources, such as maximum RAM**
是成立的。

你可以把它记成：
## **Boot tab 不只是选系统，也能加启动参数和资源限制。**

---

## 为什么 startup items 不对
这个是最容易混的。

### **Startup items**
更像：
- 开机自启动程序
- 启动应用
- 一般应用层自启动项目

它不属于这题说的：
## **Boot tab**

也就是说：
- **Boot tab** → 启动方式/日志/系统选择/启动参数
- **Startup items** → 启动程序管理（不是这题这页的核心）

所以你这项不该选。

---

## 最简单记忆法
### Boot tab 先记四件事：
## **Safe boot**
## **Boot logging**
## **选默认系统**
## **资源限制（如 max RAM）**

不要记成：
## **启动程序管理页**

---

## 一句话口诀
## **Boot tab 管怎么启动、记不记日志、启哪个系统、限多少资源；不管普通 startup apps。**

### 再压缩一句
## **msconfig 的 Boot 是“启动参数页”，不是“程序自启动页”。**

**一句话：**
这题以后就这样背：**Boot tab 主要管 Safe boot、boot logging、默认启动系统、以及启动资源限制；startup items 不属于这里。**
---

## CMD 里列出当前目录文件和子目录直接用 dir；/all 不是标准参数，/? 是看帮助
![CMD dir command current directory question](images/2026-04-24-core2-cmd-dir-command-current-directory.jpg)

**题干：** Which of the following Windows command-line commands can be used to list all files and subdirectories in the current directory?

|  |  |
| --- | --- |
| ❌ 我的答案 | dir /all |
| ✅ 正确答案 | dir |

### 这题为什么会错
因为你是按直觉在想：
- “all files and subdirectories”
- 那是不是要加一个 **/all** 才像“全部显示”？

这个直觉很正常，
但 Windows CMD 的标准命令不是这么设计的。

---

## 为什么答案就是 dir
### **dir**
本身就是：
## **列出当前目录内容**

它默认就会显示：
- 文件
- 子目录

所以题目问：
### **list all files and subdirectories in the current directory**
直接答案就是：
## **dir**

不需要额外写 `/all`。

---

## 为什么 dir /all 不对
因为：
### **/all 不是 dir 的标准参数写法**

所以它看起来“语义很对”，
但命令本身不标准。

这类题的坑就在这里：
## **不是看你英文感觉像不像，而是看 Windows 命令本身认不认。**

---

## 为什么 dir /list 不对
它不是这题要的标准命令写法，
题库在这里就是要你记住：
### **最基础列目录命令就是 dir**

---

## 为什么 dir /? 也不对
### **/?**
在 Windows 命令里常表示：
## **查看帮助**

所以：
- `dir /?` = 看 dir 命令帮助说明
- 不是直接列目录内容的标准答案

---

## 最简单记忆法
### CMD 里：
- **dir** → 列当前目录
- **dir /?** → 看 dir 帮助

### 一句话口诀
## **列目录就用 dir；加 /? 是看帮助，不是看文件。**

### 再压缩一句
## **Windows CMD 先记：列目录 = dir。**

**一句话：**
这题以后直接秒选：**在 Windows CMD 里，列出当前目录的文件和子目录，标准命令就是 `dir`；`/?` 是帮助，`/all` 不是这题的标准参数。**
---

## Windows 里的命令行分区工具是 diskpart；sfdisk / gpart / diskutil 都是别的平台味道
![diskpart Windows CLI partitioning utility question](images/2026-04-24-core2-diskpart-windows-cli-partitioning-utility.jpg)

**题干：** Which of the commands in Windows launches a text-based, command-line partitioning utility?

|  |  |
| --- | --- |
| ❌ 我的答案 | gpart |
| ✅ 正确答案 | diskpart |

### 这题最该先抓的关键词
## **in Windows**

题目不是单纯问：
- 哪个命令像分区工具

而是在问：
## **Windows 里哪个命令能打开文本型命令行分区工具**

标准答案就是：
## **diskpart**

---

## 为什么答案是 diskpart
### **diskpart**
就是 Windows 里的：
## **命令行磁盘/分区管理工具**

它能做的事包括：
- 查看磁盘
- 选择磁盘/分区
- 创建分区
- 删除分区
- 格式化
- 指派盘符

所以题目说的：
### **text-based, command-line partitioning utility**
在 Windows 里最标准就是：
## **diskpart**

---

## 为什么你选的 gpart 不对
### **gpart**
看起来也像分区工具名字，
所以你会选它完全不奇怪。

但这题的关键不是“名字像不像”，
而是：
## **题目限定了 Windows**

Windows 里常考、标准、原生命令就是：
## **diskpart**

---

## 其他几个为什么不对
### sfdisk
- 更像 Linux/Unix 语境的命令
- 不是 Windows 里这一题的标准答案

### diskutil
- 更偏 macOS 语境
- 不是 Windows 命令

### gpart
- 也不是这题里 Windows 的标准原生命令

---

## 最简单记忆法
### 平台一对照就好记：
- **Windows** → **diskpart**
- **macOS** → **diskutil**
- **Linux** → 常见 fdisk / sfdisk / parted 这类

---

## 一句话口诀
## **Windows 分区命令记 diskpart，Mac 记 diskutil，Linux 再看 fdisk/sfdisk。**

### 再压缩一句
## **看到“in Windows”，先锁 diskpart。**

**一句话：**
这题以后直接秒选：**Windows 的文本型命令行分区工具就是 diskpart；别被其他平台的命令名字带偏。**
---

## Windows 命令行里复制功能最强、选项最多的是 robocopy；move 只是移动，xcopy 比较老，copy 更基础
![robocopy vs xcopy copy move question](images/2026-04-24-core2-robocopy-vs-xcopy-copy-move.jpg)

**题干：** Which copying utility accessible via Windows command line interface offers the widest range of options?

|  |  |
| --- | --- |
| ❌ 我的答案 | move |
| ✅ 正确答案 | robocopy |

### 这题最核心的词
## **copying utility**
和
## **widest range of options**

也就是说题目不是在问：
- 哪个命令能搬文件

而是在问：
### **哪个“复制工具”功能最全、选项最多**

所以标准答案就是：
## **robocopy**

---

## 为什么 robocopy 是对的
### **robocopy = Robust File Copy**
它是 Windows 里功能非常强的复制工具，
常见优势包括：
- 复制目录树
- 镜像同步
- 保留属性/权限
- 断点/重试
- 过滤文件
- 多种高级参数

所以如果题目问：
## **widest range of options**
Windows CLI 里最标准就该想到：
## **robocopy**

---

## 为什么你选的 move 不对
### **move**
只是：
## **移动文件/目录**

它不是“高级复制工具”，
更不是以“选项最多”著称。

所以这题不能选 move。

---

## 为什么 xcopy 没中
### **xcopy**
确实也是复制命令，
而且比最基础的 `copy` 强得多，
所以它很容易当干扰项。

但考试里如果问：
## **最强 / 选项最广 / widest range of options**

那通常是：
## **robocopy > xcopy > copy**

所以 xcopy 不如 robocopy。

---

## 为什么 copy 也不对
### **copy**
是更基础的复制命令，
功能最简单，
不是这题要的“选项最多”的那个。

---

## 最简单记忆法
### Windows CLI 复制命令这样排：
- **copy** → 最基础
- **xcopy** → 老一点、比 copy 强
- **robocopy** → 最强、最全、企业味最重
- **move** → 不是复制，是移动

---

## 一句话口诀
## **复制功能最强看 robocopy，移动文件才用 move。**

### 再压缩一句
## **copy < xcopy < robocopy。**

**一句话：**
这题以后直接背：**Windows 命令行里复制工具功能最强、选项最多的是 robocopy；move 不是复制工具，xcopy 也没有 robocopy 全。**
---

## Windows CMD 看某个命令的帮助语法：直接 `command /?`；`man` 是 Linux 味，不是 Windows 这题答案
![Windows help syntax command slash question](images/2026-04-24-core2-windows-help-syntax-command-slash-question.jpg)

**题干：** What is the standard syntax in Windows command line for displaying help or usage information related to a specific utility?

|  |  |
| --- | --- |
| ❌ 我的答案 | [command name] man |
| ✅ 正确答案 | [command name] /? |

### 这题最关键的点
你这次是把：
## **Windows CMD**
和
## **Linux / Unix 命令习惯**
混了。

在 Windows 里，
最标准的帮助写法通常是：
# **command /?**

比如：
- `dir /?`
- `ipconfig /?`
- `robocopy /?`

---

## 为什么 `/?” 是对的
在 Windows 命令提示符里，
很多命令都会支持：
## **`/?` = 查看该命令帮助/用法说明**

所以题目问：
### **displaying help or usage information related to a specific utility**
答案就是：
# **[command name] /?**

---

## 为什么 `man` 不对
### `man`
是 Linux / Unix 很经典的：
## **manual pages**

比如：
- `man ls`
- `man grep`
- `man ps`

但这题问的是：
## **Windows command line**

所以不能把 Linux 那套直接搬过来。

---

## 为什么 `help` 和 `info` 这题没中
它们看起来“像英语正确”，
但题目要的是：
## **standard syntax**

在 Windows 题库里，
最标准、最稳定、最常考的固定形式就是：
# **command /?**

所以不要靠英语感觉猜。

---

## 最简单记忆法
### 平台一对照就好记：
- **Windows CMD** → `command /?`
- **Linux/Unix** → `man command`

---

## 一句话口诀
# **Windows 看帮助用 `/?`，Linux 看帮助用 `man`。**

### 再压缩一句
# **CMD 见帮助先想斜杠问号，不想 man。**

**一句话：**
这题以后直接秒选：**Windows 命令行里查看某个命令的帮助/用法，标准写法是 `command /?`；`man` 是 Linux/Unix 那套。**
---

## 查看当前用户/计算机的 Group Policy 设置，用 gpresult；net view 是看网络共享，不是组策略
![gpresult group policy command question](images/2026-04-24-core2-gpresult-group-policy-command.jpg)

**题干：** Which of the answers listed below refers to a command-line tool in Windows that can be used to display current Group Policy settings for a user or computer?

|  |  |
| --- | --- |
| ❌ 我的答案 | net view |
| ✅ 正确答案 | gpresult |

### 这题最关键的词
## **Group Policy settings**

只要题目里出现：
- Group Policy
- 当前策略结果
- 用户/计算机应用了哪些策略

第一反应就该是：
# **gpresult**

---

## 为什么答案是 gpresult
### **gpresult = Group Policy Result**
它本来就是 Windows 里用来：
## **显示用户或计算机当前应用到的组策略结果**

所以题目问：
> display current Group Policy settings for a user or computer

标准答案就是：
# **gpresult**

它名字本身就能帮你记：
- **gp** = Group Policy
- **result** = 结果 / 生效结果

---

## 为什么你选的 net view 不对
### **net view**
更偏：
## **查看网络上的共享资源 / 共享计算机**

也就是它和：
- 共享
- 网络浏览
- 远程主机共享资源

更相关，
而不是组策略。

所以：
- **net view** ≠ Group Policy
- **gpresult** = Group Policy result

---

## 另外两个为什么不对
### verify
- 是文件/卷校验相关语境的命令
- 跟组策略无关

### gpupdate
- 这个很容易混！
- **gpupdate** 是：
## **刷新/重新应用 Group Policy**

而不是：
## **显示当前生效的 Group Policy 结果**

所以这题一定要分清：
- **gpupdate** → 更新/刷新策略
- **gpresult** → 查看策略结果

---

## 最简单记忆法
### Group Policy 两兄弟：
- **gpupdate** → 更新策略
- **gpresult** → 看结果

---

## 一句话口诀
# **要刷新用 gpupdate，要查看用 gpresult。**

### 再压缩一句
# **Group Policy 看结果就找 gpresult。**

**一句话：**
这题以后直接秒选：**查看当前用户/计算机应用了哪些组策略，用 `gpresult`；`gpupdate` 是刷新策略，`net view` 是看网络共享。**
---

## SFC = System File Checker，核心就是“扫系统文件 + 修系统文件”；不是加密，也不是查磁盘坏道
![SFC System File Checker scan and repair question](images/2026-04-24-core2-sfc-system-file-checker-scan-and-repair.jpg)

**题干：** The sfc command-line utility in Windows: (Select 2 answers)

**正确答案：**
- **Replaces incorrect system file versions with correct Microsoft versions**
- **Scans the integrity of all protected system files**

**错误选项：**
- Scans disk volumes for file system errors
- Identifies and recovers readable data from bad sectors on a drive
- Encrypts files to prevent unauthorized access to sensitive data

### 这题你卡住很正常
因为 **sfc** 如果没实际用过，
光看缩写很难第一反应知道它干嘛。

你现在只要把它强行绑定成一句话就行：
# **SFC = System File Checker = 查系统文件、修系统文件**

---

## sfc 到底是干嘛的
### **sfc = System File Checker**
它是 Windows 里专门用来：
- 检查受保护的系统文件是否损坏
- 发现系统文件版本不对/损坏时进行修复
- 用正确的 Microsoft 系统文件替换坏掉的版本

所以这题正确两项就是：

### 1. **Scans the integrity of all protected system files**
也就是：
## **检查受保护系统文件的完整性**

### 2. **Replaces incorrect system file versions with correct Microsoft versions**
也就是：
## **把错误/损坏的系统文件换成正确版本**

---

## 最常见命令长什么样
你以后看到最常见的就是：
# **sfc /scannow**

这个命令的味道就是：
## **现在立刻扫描并尝试修复系统文件**

所以你可以把 sfc 直接记成：
# **Windows 系统文件体检 + 修复工具**

---

## 为什么其他几个不对
### 1. Scans disk volumes for file system errors
这个更像：
# **chkdsk**

因为 **chkdsk** 才是检查磁盘/文件系统错误的。

### 2. Identifies and recovers readable data from bad sectors on a drive
这个也更像：
# **chkdsk /r**

因为坏道、恢复可读数据，这都是磁盘层面的事情，
不是 sfc。

### 3. Encrypts files to prevent unauthorized access to sensitive data
这个更像：
- **EFS**
- **BitLocker**

总之是加密工具，
不是 sfc。

---

## 最简单区分
### Windows 常见命令这样记：
- **sfc** → 查/修系统文件
- **chkdsk** → 查磁盘/文件系统/坏道
- **BitLocker / EFS** → 加密

---

## 一句话口诀
# **SFC 修系统文件，CHKDSK 修磁盘。**

### 再压缩一句
# **sfc /scannow = 扫系统文件，不扫坏道。**

**一句话：**
这题以后直接这样背：**SFC 就是 System File Checker，负责检查受保护系统文件的完整性，并用正确的 Microsoft 版本替换损坏或错误的系统文件。**
---

## rmdir 要删整个目录树，关键是“路径要对 + /s”；这题错在选项都没指向 Data，所以答案是 None of the above
![rmdir delete directory tree correct path and switches question](images/2026-04-24-core2-rmdir-delete-directory-tree-correct-path-and-switches.jpg)

**题干：** A user wants to delete the entire directory named Data located at `C:\Files\Data` along with all its subdirectories and files using the Windows command-line. Which variant of the `rmdir` command should they run?

|  |  |
| --- | --- |
| ❌ 我的答案 | `rmdir C:\Files /r` |
| ✅ 正确答案 | **None of the above** |

### 这题最坑的地方
你不是完全不会，
而是被：
## **“删整个目录树”**
这个概念带去想 `/r` 了。

但 Windows 这题真正要你同时看两件事：
1. **参数对不对**
2. **路径对不对**

只看参数很容易掉坑。

---

## 为什么正确答案是 None of the above
题目要删的是：
# **`C:\Files\Data`**

而选项写的是：
- `rmdir C:\Files /s`
- `rmdir C:\Files /q`
- `rmdir C:\Files /r`

它们都在删：
# **`C:\Files`**
不是：
# **`C:\Files\Data`**

所以这几项即使参数里有看起来“接近”的，
也都不是题目要求的正确命令。

因此标准答案才是：
# **None of the above**

---

## 真正正确的命令应该长什么样
如果真要删除：
- `C:\Files\Data`
- 连同其子目录和文件

标准写法应该是：
# **`rmdir C:\Files\Data /s`**

如果还想静默不提示确认，
常见会再加：
# **`rmdir C:\Files\Data /s /q`**

---

## 为什么你选的 `/r` 不对
因为在 Windows 这题语境里，
## **rmdir 常见考点是 `/s` 和 `/q`**

### `/s`
- 删除目录本身
- 连同所有子目录和文件

### `/q`
- quiet
- 静默模式
- 不再确认（通常和 `/s` 搭配）

而你选的：
### `/r`
不是这题要考的标准参数。

---

## 最简单记忆法
### Windows `rmdir` 两个最常考开关：
- **`/s`** → 连子目录和文件一起删
- **`/q`** → 静默删除，不确认

### 所以固定背法：
# **删整个目录树先想 `/s`**
# **安静删再加 `/q`**

---

## 一句话口诀
# **删目录树用 `rmdir /s`，静默再加 `/q`。**

### 再压一句
# **先看路径，再看参数；路径错了整题都错。**

**一句话：**
这题以后直接这样背：**Windows 里删除整个目录及其子目录/文件要靠 `rmdir <目录> /s`，但这题所有选项都写成了 `C:\Files` 而不是 `C:\Files\Data`，所以只能选 None of the above。**
---

## chkdsk 里 `/f` 是修文件系统错误，`/r` 是找坏扇区并尽量恢复数据；这题问 `/f`，不是 `/r`
![chkdsk f vs r filesystem errors vs bad sectors question](images/2026-04-24-core2-chkdsk-f-vs-r-filesystem-errors-vs-bad-sectors.jpg)

**题干：** The `/f` switch of the `chkdsk` command-line utility in MS Windows instructs the utility to:

|  |  |
| --- | --- |
| ❌ 我的答案 | Identify bad sectors on the disk and attempt to recover any readable data from them |
| ✅ 正确答案 | Automatically repair detected file system errors on the disk |

### 你这题错得非常典型
因为你其实记住的是：
# **`chkdsk /r`**

但题目问的是：
# **`chkdsk /f`**

这两个经常一起考，
也最容易混。

---

## `/f` 和 `/r` 到底差在哪
### **`/f`**
意思是：
# **修复磁盘上的文件系统错误**

也就是：
- 检测 file system errors
- 自动尝试修复这些错误

所以题目里正确答案：
### **Automatically repair detected file system errors on the disk**
就是 `/f`。

---

### **`/r`**
意思是：
# **查找坏扇区，并尽量恢复可读数据**

也就是：
- identify bad sectors
- recover readable data

这正是你这题选的那句。

所以：
## **你不是不会 chkdsk，你是把 `/r` 的作用答到了 `/f` 题上。**

---

## 最简单对照记忆
### **`/f` = fix**
直接记：
# **f = fix file system errors**

### **`/r` = recover**
直接记：
# **r = recover readable data from bad sectors**

虽然严格说 `/r` 还包含定位坏扇区，
但考试里这样记最好用。

---

## 你可以这样一口气背下来
- **chkdsk /f** → 修文件系统错误
- **chkdsk /r** → 找坏扇区 + 尽量恢复可读数据

而且常见理解里：
## **`/r` 比 `/f` 更重、更慢**
因为它做的事情更多。

---

## 为什么其他两个也不对
### Scan the system for corrupted or missing system files
这个更像：
# **sfc /scannow**

### Optimize disk usage by consolidating fragmented file data
这个更像：
# **磁盘碎片整理 / defrag**

都不是 chkdsk `/f`。

---

## 一句话口诀
# **`/f` = fix 错误，`/r` = recover 坏道数据。**

### 再压一句
# **CHKDSK：修错看 `/f`，查坏道看 `/r`。**

**一句话：**
这题以后直接这样背：**`chkdsk /f` 用来自动修复文件系统错误；`chkdsk /r` 才是查找坏扇区并尽量恢复可读数据。**
---

## pathping：既看路径，也看延迟/丢包；不是测指定端口
![pathping traces route and measures latency packet loss](images/2026-04-25-core2-pathping-trace-route-latency-packet-loss.jpg)

**题干：** What are the most important functionalities provided by the pathping utility? (Select 2 answers)

|  |  |
| --- | --- |
| ❌ 我的答案 | Tests connectivity to a specific port |
| ✅ 正确答案 | Traces the path to the destination / Measures latency and packet loss |

### 这题最该抓的关键词
题目问的是：
## **pathping utility**

这个命令本质上可以把它记成：
## **ping + tracert 的结合版**

所以它最重要的两个功能就是：
- **Traces the path to the destination**
- **Measures latency and packet loss**

---

## 为什么 trace the path 对
`pathping` 会先像 `tracert/traceroute` 一样：
### **把数据到目标主机经过的路径跳点列出来**

也就是看：
- 经过哪些路由器
- 路径走到哪里
- 哪一跳可能有问题

所以：
## **Traces the path to the destination** 一定是对的。

---

## 为什么 latency and packet loss 对
`pathping` 比 `tracert` 更进一步的地方就在于：
### **它还会统计每一跳的延迟和丢包情况**

所以它常被用来判断：
- 哪一段链路慢
- 哪一跳丢包严重

因此：
## **Measures latency and packet loss** 也是对的。

---

## 为什么不是 specific port
### **测指定端口** 更像是：
- `telnet <host> <port>`
- `Test-NetConnection -Port`
- `nc` / `nmap`

`pathping` 不是拿来测某个 TCP/UDP 端口通不通的。

所以：
## **Tests connectivity to a specific port** 是错的。

---

## 其他选项为什么不对
### Displays network statistics
这说法太泛，不是 `pathping` 的核心考试点。

### Sends broadcast messages over the network
这根本不是 `pathping` 的用途。

---

## 最短记忆法
## **pathping = 路径 + 延迟/丢包**

再压缩成一句：
## **先 trace route，再看 loss/latency。**

---

## 一句话口诀
## **pathping 不是查端口，是查路径和丢包。**

### 再给你一个考场版
## **端口找 telnet / Test-NetConnection；路径丢包找 pathping。**

**一句话：**
这题以后直接这样背：**pathping = traceroute 功能 + latency/packet loss 分析，所以答案是“追踪路径”加“测延迟和丢包”，不是“测试指定端口”。**
---

## robocopy：大批量拷贝、网络中断可续传，优先于 xcopy
![robocopy resume large volume file transfer](images/2026-04-25-core2-robocopy-resume-large-file-transfer.jpg)

**题干：** A user needs to copy a very large volume of files from one Windows host to another. The task must resume automatically if interrupted due to network issues. Which command-line tool is best suited for this task?

|  |  |
| --- | --- |
| ❌ 我的答案 | xcopy |
| ✅ 正确答案 | robocopy |

### 这题最该抓的关键词
题目里最关键的是：
- **very large volume of files**
- **resume automatically if interrupted**

只要看到这种描述，就优先想到：
## **robocopy**

---

## 为什么 robocopy 对
`robocopy` = **Robust File Copy**，名字就已经在提示它的用途：
### **适合大量文件、网络复制、可重试、可恢复**

它特别适合：
- 大批量文件迁移
- 网络共享之间复制
- 中断后继续
- 更稳定的复制任务

所以这题说“网络问题中断后还能自动继续”，正确答案就是：
## **robocopy**

---

## 为什么不是 xcopy
`xcopy` 比 `copy` 强，能复制目录树，历史上也常用。

但考试里要分清：
- **xcopy** → 老一点、基础一点
- **robocopy** → 更强壮、更适合大规模和不稳定网络环境

题目已经明确强调：
## **大批量 + 中断恢复**

这正是 `robocopy` 的典型场景，不是 `xcopy` 的最佳答案。

---

## 为什么其他两个更不对
### copy
- 适合简单文件复制
- 不适合大规模目录/复杂迁移

### move
- 是移动，不是强调可靠的大批量复制工具
- 也不是这题考点

---

## 最短记忆法
## **大批量传输看 robocopy，简单复制才想 copy/xcopy。**

再压缩成一句：
## **网络会断、文件很多，就选 robocopy。**

---

## 一句话口诀
## **robocopy = robust copy，越大越乱越该用它。**

### 考场速记版
## **copy 复制单个，xcopy 复制目录，robocopy 打大仗。**

**一句话：**
这题以后直接这样背：**看到“大量文件 + Windows 主机间传输 + 网络中断后自动恢复”，就选 robocopy；xcopy 不如它适合这种企业级/大批量复制场景。**


---

## Control Panel 的 Category 视图是分类入口，不是全部 applet 平铺列表
![Control Panel category vs icons view](images/2026-04-26-core2-control-panel-category-vs-icons-view.jpg)

**题干：** The “View by: Category” option in the Microsoft Windows Control Panel displays the entire contents of the Control Panel in a single window, enabling quick access to each Control Panel applet.

|  |  |
| --- | --- |
| ❌ 我的答案 | True |
| ✅ 正确答案 | False |

### 为什么这题是错的
题干把 **Category view** 和 **Large icons / Small icons** 搞混了。

- **Category**：按功能分类显示
  - System and Security
  - Network and Internet
  - Hardware and Sound
- **Large icons / Small icons**：才是把各个 **Control Panel applet** 直接列出来

所以：
## **Category 不是“全部项目一页展开”**
它只是**分类入口页**。

---

## 为什么 False 才对
题干说：
> displays the entire contents of the Control Panel in a single window, enabling quick access to each Control Panel applet

这句话描述的其实更像：
## **Large icons / Small icons 视图**
因为这两种视图才会把控制面板里的项目直接列出来，方便你直接点到某个 applet。

而 **Category** 视图是先按类别分组，
你通常还要再点进去下一层，
所以不算“把整个内容完整平铺出来”。

---

## 考点本质
这题考的是：
## **Windows Control Panel 不同查看方式的区别**

### 快速对应
- **Category** → 分类看
- **Large icons / Small icons** → 全项目直接看

---

## 最简单记忆法
## **Category 看大类，Icons 看全表。**

再压缩一句：
## **想一眼看到全部 applet，不选 Category，选 Icons。**

---

## 一句话口诀
## **Category 先分组，Icons 才全出。**

**一句话：**
以后看到 Control Panel 题目里写 **Category 会显示全部 applet**，基本就要警觉：**错，真正接近“全部列出”的是 Large icons / Small icons。**

---

## Internet Properties 里删除浏览痕迹先想 General，不是 Privacy
![Internet Properties General tab delete browsing history](images/2026-04-26-core2-internet-properties-general-delete-browsing-history.jpg)

**题干：** Which tab of the Windows Internet Properties applet provides an option for deleting temporary Internet files, cookies, web browsing and download history, saved passwords, and data typed into web forms?

|  |  |
| --- | --- |
| ❌ 我的答案 | Privacy |
| ✅ 正确答案 | General |

### 为什么正确答案是 General
在 **Internet Properties** 里面，
和下面这些“浏览数据清理”最直接对应的是：

- temporary Internet files
- cookies
- browsing history
- download history
- saved passwords
- form data

这些都属于：
## **Browsing history / Delete browsing history**
而这个按钮位置就在：
## **General 选项卡**

---

## 为什么 Privacy 容易让人选错
因为看到 **cookies**，很多人会马上联想到 **Privacy**。
这就是这题最容易掉坑的地方。

但 **Privacy** 选项卡更偏向：
- cookie 处理策略
- 弹窗阻止
- 隐私级别设置

它不是那个“把浏览记录、缓存、密码、表单记录一起清掉”的主要入口。

所以这题问的是：
## **删除一整组浏览数据的入口在哪个 tab**
答案就该想到：
## **General**

---

## 考点本质
这题考的是：
## **Internet Properties 各标签页的职责区分**

### 快速对应
- **General** → 主页、标签页、浏览历史删除
- **Security** → 安全区域级别
- **Privacy** → Cookie / 隐私设置 / 弹窗
- **Content** → 证书、自动完成
- **Connections** → 拨号/VPN/代理连接
- **Programs** → 默认程序
- **Advanced** → 高级 IE/网络选项

---

## 最简单记忆法
## **删历史去 General；调隐私才去 Privacy。**

再压缩一句：
## **“Delete browsing history” 看到 delete 就先想 General。**

---

## 一句话口诀
## **清缓存删记录找 General，控 Cookie 隐私看 Privacy。**

**一句话：**
以后遇到这类题，别被 **cookies** 这个词带跑：**如果题目是在问“删除整套浏览痕迹”的入口，优先选 General。**

---

## Internet Properties 的内建弹窗拦截器在 Privacy，不在 Content
![Internet Properties pop-up blocker Privacy tab](images/2026-04-26-core2-internet-properties-pop-up-blocker-privacy-tab.jpg)

**题干：** Which of the answers listed below refers to a Windows Internet Properties applet tab that provides settings for a built-in pop-up blocker?

|  |  |
| --- | --- |
| ❌ 我的答案 | Content |
| ✅ 正确答案 | Privacy |

### 为什么正确答案是 Privacy
在 **Internet Properties** 里面，
**Pop-up Blocker（弹窗阻止程序）** 的设置放在：
## **Privacy**

这是经典考点：
- Privacy 里不只是隐私级别
- 还包含 **Pop-up Blocker** 相关设置

所以题目问：
## **built-in pop-up blocker 在哪个 tab**
就应该选：
## **Privacy**

---

## 为什么 Content 容易选错
因为很多人会把下面这些混在一起：
- certificates
- AutoComplete
- feeds/web slices
- content advisor
- 浏览器内容相关设置

这些更像是 **Content** 在管的范围。

但 **弹窗拦截器** 不是 Content 的主考点，
它属于：
## **Privacy**

---

## 考点本质
这题考的是：
## **Internet Properties 各 tab 的功能定位**

### 快速对应
- **General** → 浏览历史 / 主页 / 标签页
- **Security** → 安全区域
- **Privacy** → Cookie、隐私级别、Pop-up Blocker
- **Content** → 证书、AutoComplete、内容相关
- **Connections** → 拨号 / VPN / 代理
- **Programs** → 默认程序
- **Advanced** → 高级设置

---

## 最简单记忆法
## **弹窗拦截属于隐私控制，所以看 Privacy。**

再压缩一句：
## **Pop-up → Privacy。**

---

## 一句话口诀
## **删记录找 General，拦弹窗找 Privacy。**

**一句话：**
以后看到 **pop-up blocker**，直接先想 **Privacy**；看到 **certificates / AutoComplete** 才更容易联想到 **Content**。

---

## Internet Properties 里的高级 Cookie 管理选项在 Privacy，不在 Security
![Internet Properties advanced cookie management Privacy tab](images/2026-04-26-core2-internet-properties-advanced-cookie-management-privacy-tab.jpg)

**题干：** Which tab of the Internet Properties applet in Windows provides access to advanced cookie management options?

|  |  |
| --- | --- |
| ❌ 我的答案 | Security |
| ✅ 正确答案 | Privacy |

### 为什么这题是 Privacy
题目问的是：
## **advanced cookie management options**

只要看到：
- cookie
- privacy level
- site handling / cookie handling
- pop-up blocker

大概率就要先想到：
## **Privacy 选项卡**

因为 **Internet Properties → Privacy** 里面本来就负责：
- Cookie 处理策略
- 隐私级别
- 站点例外设置
- 高级 Cookie 选项
- Pop-up Blocker

所以这题答案是：
## **Privacy**

---

## 为什么不是 Security
**Security** 选项卡主要在管：
- Internet / Local intranet / Trusted sites / Restricted sites 区域
- 安全级别
- 站点信任区域分配

它重点是：
## **安全区域和安全级别**
不是 Cookie 的高级管理。

所以这题如果选 Security，
说明把“安全”这个大词和“隐私/Cookie管理”混在一起了。

---

## 考点本质
这题其实和前两题是同一组：
## **Internet Properties 各 tab 的职责区分**

### 快速对应
- **General** → 浏览历史、主页
- **Security** → 安全区域
- **Privacy** → Cookie、隐私级别、弹窗拦截
- **Content** → 证书、AutoComplete
- **Connections** → 拨号/VPN/代理
- **Programs** → 默认程序
- **Advanced** → 高级系统/浏览器设置

---

## 最简单记忆法
## **Cookie 管理看 Privacy；站点信任区看 Security。**

再压缩一句：
## **cookie → Privacy，zone → Security。**

---

## 一句话口诀
## **隐私管 Cookie，安全管区域。**

**一句话：**
以后看到题干里有 **advanced cookie management**，就直接往 **Privacy** 想；如果看到 **trusted sites / security zones**，才是 **Security**。

---

## Internet Properties 里证书、AutoComplete、RSS/Feeds 看 Content，不是 Connections
![Internet Properties Content tab certificates autocomplete RSS](images/2026-04-26-core2-internet-properties-content-certificates-autocomplete-rss.jpg)

**题干：** Which of the Windows Internet Properties applet tabs enables the management of digital certificates, the AutoComplete functionality, and RSS feeds?

|  |  |
| --- | --- |
| ❌ 我的答案 | Connections |
| ✅ 正确答案 | Content |

### 为什么正确答案是 Content
这题其实是在考 **Internet Properties 各标签页的“招牌功能”**。

看到下面这些关键词时：
- digital certificates
- AutoComplete
- RSS feeds / Feeds and Web Slices

就应该先想到：
## **Content**

因为 **Content** 选项卡典型包含：
- **Certificates**
- **AutoComplete**
- **Feeds and Web Slices**
- （老版本里还常见 Content Advisor）

所以这题答案很标准：
## **Content**

---

## 为什么不是 Connections
**Connections** 选项卡主要负责的是：
- 拨号设置
- VPN / 网络连接相关
- LAN settings
- Proxy server

它重点是：
## **连接方式与网络接入配置**

不是证书、自动完成、RSS 这些“浏览器内容/身份/表单体验”相关内容。

所以如果题干出现：
- certificate
- AutoComplete
- feed

那就别往 Connections 想。

---

## 考点本质
这题和前面几题一样，都是：
## **Internet Properties tab 对应关系题**

### 快速对应
- **General** → 主页、浏览历史删除
- **Security** → 安全区域
- **Privacy** → Cookie、弹窗拦截
- **Content** → 证书、AutoComplete、Feeds
- **Connections** → 拨号 / VPN / 代理
- **Programs** → 默认程序
- **Advanced** → 高级设置

---

## 最简单记忆法
## **证书和自动完成，先看 Content。**

再压缩一句：
## **certificate / autocomplete / feed → Content**

---

## 一句话口诀
## **证书自动填，RSS 也归 Content。**

**一句话：**
以后看到题干里同时出现 **Certificates + AutoComplete + RSS/Feeds**，基本就是在明示你选 **Content**。

---

## Connections 选项卡要记住：VPN、Proxy、LAN；Security zones 不在这里
![Internet Properties Connections tab LAN VPN Proxy not Security zones](images/2026-04-26-core2-connections-tab-lan-vpn-proxy-not-security-zones.jpg)

**题干：** Which of the following answers refer to network settings accessible through the Connections tab of the Internet Properties applet in Windows? (Select 3 answers)

|  |  |
| --- | --- |
| ❌ 我的答案 | Internet security zone settings / Dial-up and VPN settings / Proxy server settings |
| ✅ 正确答案 | LAN settings / Dial-up and VPN settings / Proxy server settings |

### 为什么你这题会错
你已经抓对了两项：
- **Dial-up and VPN settings**
- **Proxy server settings**

漏掉的是：
- **LAN settings**

错选的是：
- **Internet security zone settings**

---

## 为什么 LAN settings 对
在 **Internet Properties → Connections** 里，经典会出现这些东西：
- 拨号连接
- VPN 连接
- **LAN settings**
- 代理（Proxy）相关设置

所以题目问 **Connections tab 可访问的网络设置**，
**LAN settings** 一定要想到。

---

## 为什么 Internet security zone settings 不对
**Internet security zone settings** 属于：
## **Security 选项卡**

那边管的是：
- Internet
- Local intranet
- Trusted sites
- Restricted sites
- 安全级别 / 区域策略

它不是 **Connections** 的内容。

所以这题的核心混淆点是：
## **Connections = 连接方式 / 代理 / LAN**
## **Security = 区域 / 站点信任 / 安全级别**

---

## 考点本质
这题本质还是在考：
## **Internet Properties 各选项卡的职责边界**

### Connections 速记
- **Dial-up / VPN**
- **LAN settings**
- **Proxy**

### Security 速记
- **Security zones**
- Trusted / Restricted sites
- 安全级别

---

## 最简单记忆法
## **Connections 管“怎么连”，Security 管“连哪些站更信任”。**

再压缩一句：
## **VPN / Proxy / LAN → Connections；Zones → Security**

---

## 一句话口诀
## **连线走 Connections，分区看 Security。**

**一句话：**
以后只要题目里出现 **LAN / VPN / Proxy**，优先想 **Connections**；出现 **security zones / trusted sites**，就转去 **Security**。

---

## Devices and Printers 是简化设备视图，可增删设备也可做故障排除，不是详细驱动管理页
![Devices and Printers simplified view and troubleshooting](images/2026-04-26-core2-devices-and-printers-simplified-view-troubleshooting.jpg)

**题干：** Which of the answers listed below refer to features of the Windows Devices and Printers Control Panel applet? (Select 3 answers)

|  |  |
| --- | --- |
| ❌ 我的答案 | Allows users to add/remove wired and wireless devices / Provides a detailed view of all connected devices / Allows users to troubleshoot a device that is not working properly |
| ✅ 正确答案 | Allows users to add/remove wired and wireless devices / Provides a simplified view of all connected devices / Allows users to troubleshoot a device that is not working properly |

### 这题错在哪里
你选对了两项：
- **Allows users to add/remove wired and wireless devices**
- **Allows users to troubleshoot a device that is not working properly**

错的是把：
- **Provides a detailed view of all connected devices**

选进去了。

真正正确的是：
- **Provides a simplified view of all connected devices**

---

## 为什么是 simplified view
**Devices and Printers** 的定位更像：
## **给用户一个比较直观、简化的设备总览界面**

它会把：
- 打印机
- 蓝牙设备
- 外接设备
- 部分已连接硬件

用比较容易理解的方式展示出来，
方便普通用户做：
- 添加设备
- 删除设备
- 查看基本状态
- 运行故障排除

所以它不是那种“详细技术参数/驱动层级/硬件树状结构”的页面。

那种更细、更底层、更技术性的查看，通常更像：
## **Device Manager 的风格**

---

## 为什么 detailed view 不对
题目里的 **detailed view of all connected devices** 听起来更像：
- 设备管理器（Device Manager）
- 更底层的硬件详情
- 驱动与资源级别的查看

而不是 **Devices and Printers** 这种偏用户友好的入口。

所以这题的关键就是区分：
## **Devices and Printers = 简化设备视图**
## **Device Manager = 详细硬件/驱动视图**

---

## 其他选项为什么不对
### Does not include troubleshooting features
错，因为它**确实带 troubleshooting**。

### Allows users to restore a device driver to the previously installed version
这更像 **Device Manager 里的 driver rollback**，不是 Devices and Printers 的核心功能。

---

## 最简单记忆法
## **Devices and Printers 给用户看“设备概览”，Device Manager 给技术员看“设备细节”。**

再压缩一句：
## **Printers 看简图，Manager 看细节。**

---

## 一句话口诀
## **增删排障去 Devices and Printers，驱动细节去 Device Manager。**

**一句话：**
以后看到 **Devices and Printers**，先想 **简化视图 + 添加/删除设备 + 故障排除**；看到 **详细硬件/驱动信息**，就别选它，去想 **Device Manager**。

---

## Network and Sharing Center 记三样：Adapter、Advanced sharing、Media streaming；不是 security zones
![Network and Sharing Center media streaming options](images/2026-04-26-core2-network-and-sharing-center-media-streaming.jpg)

**题干：** The Network and Sharing Center Control Panel applet in Windows provides access to: (Select 3 answers)

|  |  |
| --- | --- |
| ❌ 我的答案 | Network adapter settings / Advanced sharing settings / Internet security zone settings |
| ✅ 正确答案 | Network adapter settings / Advanced sharing settings / Media streaming options |

### 这题错在哪里
你前两项选对了：
- **Network adapter settings**
- **Advanced sharing settings**

漏掉的是：
- **Media streaming options**

错选的是：
- **Internet security zone settings**

---

## 为什么 Media streaming options 对
在 **Network and Sharing Center** 里，常见入口包括：
- **Change adapter settings**
- **Change advanced sharing settings**
- **Media streaming options**

这些都和：
## **网络发现、共享、连接方式、局域网媒体共享**
有关，所以属于这个 applet 的范围。

---

## 为什么 Internet security zone settings 不对
**Internet security zone settings** 属于：
## **Internet Properties / Internet Options → Security**

它管的是：
- Internet
- Local intranet
- Trusted sites
- Restricted sites
- 安全级别和站点区域

这不是 **Network and Sharing Center** 的内容。

所以这题的坑点就是：
## **Network and Sharing Center = 网络/共享/媒体流**
## **Security zones = Internet Options 的 Security**

---

## Physical location settings 为什么不对
这个说法不是 Network and Sharing Center 的标准核心入口。
考题里真正常考的是：
- adapter settings
- advanced sharing settings
- media streaming options

所以别被“location”这种听起来像网络环境的词带偏。

---

## 最简单记忆法
## **共享中心先想：网卡、共享、媒体流。**

再压缩一句：
## **Adapter + Sharing + Streaming**

---

## 一句话口诀
## **共享中心三件套：网卡、共享、媒体流。**

**一句话：**
以后看到 **Network and Sharing Center**，优先往 **adapter / advanced sharing / media streaming** 想；看到 **security zones**，马上切换到 **Internet Options → Security**。

---

## Windows 10/11 里防火墙设置对应的是 Windows Defender Firewall
![Windows Defender Firewall applet question](images/2026-04-26-core2-windows-defender-firewall-applet.jpg)

**题干：** Which of the following Control Panel applets in Windows 10 and Windows 11 provides access to firewall settings?

|  |  |
| --- | --- |
| ❌ 我的答案 | Security and Maintenance |
| ✅ 正确答案 | Windows Defender Firewall |

### 为什么正确答案是 Windows Defender Firewall
题目问的是：
## **哪个 Control Panel applet 提供 firewall settings**

在 **Windows 10 / Windows 11** 里，对应名称是：
## **Windows Defender Firewall**

这就是控制：
- 防火墙开关
- 允许应用通过防火墙
- 入站/出站规则（进一步高级配置）
- 公用/专用网络防火墙状态

所以这题是很直接的“名称识别题”。

---

## 为什么不是 Security and Maintenance
**Security and Maintenance** 更像是：
- 查看系统安全状态
- 查看维护提醒
- 汇总安全/维护通知

它不是专门进入防火墙详细配置的 applet。

也就是说：
## **Security and Maintenance 偏状态总览**
## **Windows Defender Firewall 才是防火墙入口**

---

## 为什么不是 Windows Firewall
这题有个容易混淆点：
旧资料或旧版本里你可能见过：
- **Windows Firewall**

但题目特别说的是：
## **Windows 10 and Windows 11**

所以新版正式名称更应该对应：
## **Windows Defender Firewall**

考试遇到这种题，
如果选项里同时有旧叫法和新叫法，
优先选**符合当前系统版本命名**的那个。

---

## 最简单记忆法
## **Win10/11 的防火墙看 Defender Firewall。**

再压缩一句：
## **防火墙设置 ≠ Security and Maintenance**

---

## 一句话口诀
## **安全总览看 Maintenance，防火墙本体找 Defender Firewall。**

**一句话：**
以后题目一旦明确写 **Windows 10/11**，再问防火墙 applet，优先想 **Windows Defender Firewall**。

---

## Outlook 的控制面板配置入口叫 Mail，不是 User Accounts
![Mail applet for Outlook configuration](images/2026-04-26-core2-mail-applet-outlook-configuration.jpg)

**题干：** In Windows 10 and Windows 11, the Control Panel applet providing access to Microsoft Outlook configuration options is called:

|  |  |
| --- | --- |
| ❌ 我的答案 | User Accounts |
| ✅ 正确答案 | Mail |

### 为什么正确答案是 Mail
这题考的是一个很具体的 Control Panel 名称。

如果要配置 **Microsoft Outlook** 相关内容，比如：
- Outlook profiles
- data files
- email accounts
- account setup / profile management

常见入口就是：
## **Mail**

在控制面板里它通常会显示成类似：
- **Mail**
- 或 **Mail (Microsoft Outlook)**

所以题目问 Outlook configuration options 对应哪个 applet，
答案就是：
## **Mail**

---

## 为什么不是 User Accounts
**User Accounts** 主要处理的是：
- Windows 本地账户/微软账户相关设置
- 用户类型
- 密码/凭据的部分管理
- UAC 等账户层面的东西

它不负责 Outlook 配置。

所以这题的混淆点在于：
## **邮箱账户 ≠ Windows 用户账户**

Outlook 的邮件配置入口是 **Mail**，
不是 **User Accounts**。

---

## 其他选项为什么不对
### Programs and Features
是程序安装/卸载与功能管理，
不是 Outlook 配置入口。

### Administrative Tools
是系统管理工具集合，
也不是 Outlook profile 配置入口。

---

## 最简单记忆法
## **配 Outlook 看 Mail，配 Windows 账户看 User Accounts。**

再压缩一句：
## **Outlook → Mail**

---

## 一句话口诀
## **邮箱配置找 Mail，系统账户找 User Accounts。**

**一句话：**
以后只要题目问 **Outlook configuration options**，就直接先想 **Mail applet**。

---

## Windows 10/11 的音频配置控制面板叫 Sound，不是老名字 Sounds and Audio Devices
![Sound applet Windows 10 and 11](images/2026-04-26-core2-sound-applet-windows10-11.jpg)

**题干：** Which of the answers listed below refers to an audio configuration Control Panel applet in Windows 10 and Windows 11?

|  |  |
| --- | --- |
| ❌ 我的答案 | Sounds and Audio Devices |
| ✅ 正确答案 | Sound |

### 为什么正确答案是 Sound
题目特别限定了：
## **Windows 10 and Windows 11**

在这两个版本里，音频相关的控制面板 applet 名称是：
## **Sound**

它对应的就是：
- 播放设备
- 录音设备
- 声音方案
- 默认音频设备
- 通信设备等设置

所以如果题目问的是：
## **现在这代 Windows 里的音频配置 applet 叫什么**
答案就是：
## **Sound**

---

## 为什么不是 Sounds and Audio Devices
**Sounds and Audio Devices** 是更老版本 Windows 的常见叫法，
比如早期 Windows XP 时代你更容易看到这个名称。

但题目已经明确缩小到：
## **Windows 10 / Windows 11**

所以这题考的核心就是：
## **旧名称 vs 新名称**

新版里你要认：
## **Sound**
而不是老名称。

---

## 为什么其他选项不对
### Device Manager
它可以看/管理声卡设备驱动，
但它不是“音频配置 Control Panel applet”的名称。

### Computer Management
更不是音频控制面板入口。

---

## 最简单记忆法
## **新系统看短名字：Sound。**

再压缩一句：
## **Win10/11 音频配置 = Sound**

---

## 一句话口诀
## **老系统名字长，新系统直接 Sound。**

**一句话：**
以后题目只要写 **Windows 10/11**，再看到音频控制面板名字，优先想 **Sound**，别被老名字 **Sounds and Audio Devices** 带偏。

---

# 2026-04-27 Control Panel 本地账户设置入口

![Control Panel 本地账户设置入口](images/2026-04-27-core2-control-panel-user-accounts.jpg)

**题目简述：**
Which applet in the Windows Control Panel enables the modification of local user account settings?

- 你的答案：Local Users and Groups
- 正确答案：User Accounts

### 为什么正确答案是 User Accounts
这题考的是 **Control Panel 里的 applet 名称**。

如果题目问：
- 修改本地用户账户设置
- 在 **Control Panel** 里找入口

那对应的是：
## **User Accounts**

这里可以做的通常包括：
- 更改账户类型
- 管理密码/凭据相关设置
- 修改本地账户的一些基础配置

### 为什么不是 Local Users and Groups
**Local Users and Groups** 确实也能管理本地用户，
但它属于：
## **Computer Management / MMC 管理控制台**

它不是标准的 **Control Panel applet**。

所以这题不是在问：
- “哪个工具功能更强？”
而是在问：
- “Control Panel 里这个入口叫啥？”

### 为什么这种题会考
说实话，这类题确实有点无聊 😅
但它在 CompTIA 里的意义通常不是让你死记菜单，而是考你：

- 能不能区分 **Control Panel / Settings / MMC / 管理工具** 这几类入口
- 用户描述一个问题时，你知不知道大概要去哪个管理界面
- 看到老题或旧文档时，能不能认出这些 Windows 传统入口

也就是说，它本质考的是：
## **“你认不认识 Windows 管理入口的分类”**
而不只是背单词。

### 应试角度怎么记
你不用把所有入口都当百科全书背。
重点记这一层：

- **User Accounts** → Control Panel 里的“账户入口”
- **Local Users and Groups** → MMC 里的“高级本地用户管理”

### 最短记忆法
## **题目写 Control Panel，就先选面板名字；别选 MMC 工具名。**

### 一句话口诀
## **面板改账户找 User Accounts；高级管用户才是 Local Users and Groups。**

---

# 2026-04-27 Hidden items 与 File Explorer Options

![Hidden items 与 File Explorer Options](images/2026-04-27-core2-hidden-items-file-extensions.jpg)

## 题 1：显示隐藏文件/文件夹的入口

**题目简述：**
Which of the following actions provides access to the Windows 10 and Windows 11 File Explorer setting that toggles the visibility of files and folders marked by default as hidden?

- 你的答案：Windows logo key + F > File > Show hidden files and folders
- 正确答案：Windows logo key + E > View > Hidden items

### 为什么正确答案是 View > Hidden items
在 **Windows 10 / 11** 里，要快速切换隐藏文件显示，最直接的是：

## **File Explorer > View > Hidden items**

这就是资源管理器里的可见性开关。

### 为什么你的答案不对
你的选项写的是：
- **Windows logo key + F**
- **File > Show hidden files and folders**

问题有两个：
1. **Win + F** 不是这里标准的资源管理器入口记法；题目通常会用 **Win + E** 打开 File Explorer
2. **File > Show hidden files and folders** 这个菜单路径本身也不像 Win10/11 的标准现成选项名称

也就是说，这题考的是：
## **Win10/11 里“直接显示隐藏项”的新路径**

### 最短记忆法
## **看隐藏文件：资源管理器打开后，去 View 找 Hidden items。**

---

## 题 2：隐藏/显示已知文件扩展名的入口

**题目简述：**
Which sequence of steps in Windows 10 and Windows 11 Control Panel provides access to a configuration setting that enables showing or hiding extensions for known file types?

- 你的答案：Folder Options applet > View tab > Hide extensions for known file types
- 正确答案：File Explorer Options applet > View tab > Advanced settings: > Hide extensions for known file types

### 为什么正确答案是 File Explorer Options
这题故意卡的是 **名称**。

在 Win10/11 / 新版题库表述里，Control Panel 这里更标准的名字是：
## **File Explorer Options**

然后路径是：
- **View tab**
- **Advanced settings**
- **Hide extensions for known file types**

### 为什么你的答案会错
**Folder Options** 其实更像旧名称/旧叫法。
功能方向没错，但题库要你选的是：
## **Win10/11 当前标准名称：File Explorer Options**

所以这题和前面那题本质一样，都是：
## **旧叫法 vs 新叫法 / 精确入口名**

### 应试角度怎么记
你不用纠结所有按钮位置，记住两层就够：

- **直接显示隐藏文件** → **View > Hidden items**
- **扩展名等高级显示设置** → **File Explorer Options > View > Advanced settings**

### 最短口诀
## **隐藏项走 View；扩展名走 File Explorer Options。**

---

# 2026-04-27 File name extensions 与 General tab 范围

![File name extensions 与 General tab 范围](images/2026-04-27-core2-file-explorer-extensions-general-tab.jpg)

## 题 1：显示文件扩展名的更直接入口

**题目简述：**
The File Explorer setting that enables showing or hiding extensions for known file types in Windows 10 and 11 can be accessed via:

- 你的答案：Windows logo key + E > View > Options > Advanced settings > File name extensions
- 正确答案：Windows logo key + E > View > File name extensions

### 为什么正确答案更直接
这题和上一组有点像，但它考的是：
## **File Explorer 里有没有一个更直接的开关**

答案是有：
## **View > File name extensions**

也就是说，在 Win10/11 里，显示扩展名不一定要绕进 **Options > Advanced settings**，可以直接在 View 菜单里切换。

### 为什么你的答案会错
你的路径不是完全没道理，
但题目问的是：
## **can be accessed via**

它要的是现成、直接的入口，
不是更绕的高级设置路径。

所以这题本质是：
- **直接开关** 优先
- 不要一上来就钻 Advanced settings

### 最短记忆法
## **扩展名现在也能直接在 View 里切。**

---

## 题 2：General tab 不包含什么

**题目简述：**
Which of the settings listed below is not part of the General tab of the File Explorer Options Control Panel applet in Windows 10 and Windows 11?

- 你的答案：File Explorer browsing history options (Privacy section)
- 正确答案：Visibility of hidden files, folders, and drives

### 为什么正确答案是 hidden files visibility
这题考的是 **General tab** 和 **View tab** 的范围区分。

在 **General tab** 里常见的是：
- 打开 File Explorer 默认进入哪里
- 单击/双击打开项目
- 浏览文件夹是在同一窗口还是新窗口
- Privacy / history 相关选项

但：
## **hidden files, folders, and drives 的可见性**
属于 **View tab > Advanced settings**

所以它**不属于 General tab**。

### 为什么你的答案不对
因为 **Privacy / browsing history** 恰恰就是 **General tab** 里很典型的一块。

所以这题不是考功能，而是在考：
## **General 管“基础行为”，View 管“显示规则”**

### 最短口诀
## **General 管打开方式和历史；View 管隐藏项和扩展名。**

---

# 2026-04-27 Hibernation mode 三个特征

![Hibernation mode 三个特征](images/2026-04-27-core2-hibernation-mode.jpg)

**题目简述：**
Which of the following answers refer to hibernation mode in Windows? (Select 3 answers)

- 你的答案：
  - Requires a small amount of power to maintain system memory
  - Keeps system state in RAM
  - Resumes full system operation faster than when waking from sleep mode
- 正确答案：
  - Saves the system state to a storage drive
  - Resumes full system operation more slowly than it does when waking from sleep mode
  - Turns the computer off after saving the system state to disk

### 为什么你会错
因为你选到的那三项，基本都在描述：
## **Sleep（睡眠）**

Sleep 的特点是：
- 状态保存在 **RAM**
- 需要一点点电维持内存
- 唤醒通常比较快

而这题问的是：
## **Hibernation（休眠）**

### Hibernation 的核心特征
休眠的关键就是：
## **把当前系统状态写到磁盘，然后彻底断电**

所以它对应这三条：

1. **Saves the system state to a storage drive**
   - 状态写到硬盘/SSD，不是只留在 RAM

2. **Turns the computer off after saving the system state to disk**
   - 写完以后机器相当于关机

3. **Resumes full system operation more slowly than it does when waking from sleep mode**
   - 因为要从磁盘恢复，所以通常比 Sleep 慢

### 一句话区分 Sleep vs Hibernation
- **Sleep** = 存 RAM、耗一点电、恢复快
- **Hibernation** = 存磁盘、几乎不耗电、恢复较慢

### 最短口诀
## **睡眠留内存，休眠落硬盘；睡眠醒得快，休眠更省电。**

---

# 2026-04-27 Sleep mode 三个特征

![Sleep mode 三个特征](images/2026-04-27-core2-sleep-mode.jpg)

**题目简述：**
Which of the statements listed below describe the behavior of sleep mode in Windows? (Select 3 answers)

- 你的答案：
  - Requires a small amount of power to maintain system memory
  - Saves the system state to a storage drive
  - Resumes full system operation more slowly than when recovering from hibernation mode
- 正确答案：
  - Requires a small amount of power to maintain system memory
  - Resumes full system operation faster than it does when recovering from hibernation mode
  - Keeps the system state (e.g., all open/unsaved files and running applications) in RAM

### 为什么这题会错
因为你把 **Sleep** 和 **Hibernation** 的特征又混了一下。

你选错的两项：
- **Saves the system state to a storage drive**
- **Resumes more slowly than hibernation**

这两条其实都更像：
## **Hibernation（休眠）**

### Sleep 的核心特征
Sleep 本质上是：
## **状态留在 RAM，系统保持低功耗待机**

所以它的三个关键点是：

1. **Requires a small amount of power to maintain system memory**
   - 需要一点点电维持内存内容

2. **Keeps the system state in RAM**
   - 当前打开的文件、程序状态还留在内存里

3. **Resumes full system operation faster than recovering from hibernation**
   - 因为不用从磁盘整包恢复，所以比休眠更快

### 和 Hibernation 再对照一次
- **Sleep** → RAM / 少量供电 / 恢复快
- **Hibernation** → 磁盘 / 近乎断电 / 恢复慢

### 最短口诀
## **睡眠在内存，休眠在硬盘；睡眠醒得快，休眠更省电。**
