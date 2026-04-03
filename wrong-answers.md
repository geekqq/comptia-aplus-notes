# CompTIA A+ 错题笔记

## Telnet 核心特性
**题干：** “Which of the following statements describe an important feature or service provided by Telnet? (Select three.)”

![Telnet question screenshot](images/20260330-telnet.jpg)

**正确选项：**
- Provides username and password authentication（提供用户名/密码认证）
- Transmits data in an unencrypted form（明文传输）
- Enables remote login and command execution（远程登录执行命令）

**说明：** Telnet 虽然要输入账号密码，但整条链路都是明文，任何人抓包都能看到凭证和命令。因此只适合实验或内网环境；需要安全远程必用 SSH。题目里“Telnet 不提供认证”是常见陷阱。

---

## 服务器角色：文件存储 vs 文档输出
![Server role question](images/2026-03-31-print-server.jpg)

**题干：** 哪种服务器主要负责文档输出而不是存储文件？

|  |  |
| --- | --- |
| ❌ 我的答案 | database server |
| ✅ 正确答案 | print server |

**说明：** Print server 的职责是接收打印作业、排队、发送到指定打印机；本身不负责长期存储文件。数据库/应用服务器或文件服务器才负责数据存储。

---

## 无线基础：信道宽度 / 蓝牙 / 802.11
![Wireless question set](images/2026-03-31-wireless.jpg)

### 1. 信道宽度
- ❌ 我的答案：增大信道宽度会减少干扰
- ✅ 正解：增大信道宽度可提升吞吐，但更容易与邻近信道重叠、引入干扰

### 2. 蓝牙特性（多选）
- ✅ 正确：工作在 2.4 GHz ISM 频段、短距离通信、构建 PAN、连接外设/穿戴/IoT
- ❌ 错误：认为需要视距（LOS）。蓝牙是跳频射频，不需要 LOS，视距是红外的特性

### 3. 802.11 WLAN 特性（多选）
- ✅ 正确：支持 Infrastructure 与 Ad-hoc 拓扑、由 IEEE 制定、用于高速无线局域网
- ❌ 错误：说它运行在“许可频段”。实际上 802.11 使用 ISM/UNII 等免许可频段

**记忆：**
- 信道宽度 ↑ ⇒ 带宽 ↑ 但干扰 ↑
- 蓝牙 = 2.4 GHz PAN + 外设，不需要视距
- 802.11 = IEEE WLAN，免许可频段，可基础设施或临时网络

---

## 2.4 GHz 与高频段对比
![2.4 GHz comparison question](images/2026-03-31-24ghz.jpg)

| 特性 | 2.4 GHz | 5/6 GHz |
| --- | --- | --- |
| 覆盖 | ✅ 最远，穿墙最好 | 较近 |
| 干扰 | ❌ 设备多、最容易受干扰 | 更干净 |
| 非重叠信道数量 | ❌ 只有 3 个（1/6/11） | 更多信道 |

**记忆：** “2.4 = far but few”——覆盖远，但干净信道少。

---

## TCP 445 = SMB/CIFS
![TCP 445 question](images/2026-03-31-tcp445.jpg)

|  |  |
| --- | --- |
| ❌ 我的答案 | IMAP |
| ✅ 正确答案 | SMB / CIFS |

**说明：** 445/TCP 是 Windows SMB (文件/打印共享)。IMAP 是 143/993，HTTPS 是 443，LDAPS 是 636。记住 “143/443/445/636” 这组即可。

---

## LDAP 389 & NetBIOS 137/138/139
![LDAP port question](images/2026-03-31-ldap389.jpg)

- LDAP 明文端口 = 389（TCP/UDP）
- LDAPS 加密端口 = 636
- HTTPS = 443

![NetBIOS question](images/2026-03-31-netbios.jpg)

| 端口 | 服务 |
| --- | --- |
| 137 | NetBIOS Name Service |
| 138 | NetBIOS Datagram Service |
| 139 | NetBIOS Session Service |

**记忆：** NetBIOS = 137-139 连续区间；135 是 RPC，445 是 SMB。

---

## POP3 vs SMTP；DHCP 客户端端口
![POP3 vs SMTP question](images/2026-03-31-pop3.jpg)

- SMTP（25/587）负责“发”邮件
- POP3（110/995）或 IMAP（143/993）负责“收”邮件
- 题目问“客户端下载邮件” ⇒ 应选 POP3

![DHCP client port question](images/2026-03-31-dhcp68.jpg)

- DHCP Server 监听 UDP 67
- DHCP Client 监听 UDP 68 接收 OFFER/ACK
- 记法：Server=67、Client=68，数字递增

---

## LDAP 389 再确认
![LDAP port question](images/2026-03-31-ldap389.jpg)

同上，LDAP 明文端口始终是 389；HTTPS/POP/SMTP 等各有固定端口，勿混淆。

---

## POP3 下载邮件
![POP3 question](images/2026-03-31-pop3.jpg)

客户端从服务器下载邮件 → POP3（或 IMAP）。SMTP 仅用于发信。

---

## DHCP 客户端端口 68
![DHCP question](images/2026-03-31-dhcp68.jpg)

DHCP 客户端接收响应使用 UDP 68；服务器监听 67。记成 “67→Server，68→Client”。
---

## 卫星网络特性
![Satellite Internet question](images/2026-04-01-satellite.jpg)

**正确特性（选 3）：**
- 高延迟（High signal latency）
- 易受天气影响（Interference / weather dependent）
- 成本高于地面链路（Relatively high cost vs terrestrial）

**错误选项：**
- Lack of signal interference（卫星恰好容易被雨雪衰减）
- Low signal latency（绕地轨道距离 3.6 万 km，往返延迟 500 ms 级别）
- Cheaper…（建造/发射卫星成本极高）

**记忆：** “卫星：贵、慢、怕天气”。
---

## MAN / WAN / SAN / CAN 对比（巩固题）
![MAN question](images/2026-04-01-man.jpg)

**题干：** “连接一座城市范围内多条 LAN 的网络称为什么？”
- ✅ MAN（Metropolitan Area Network）：覆盖城市/区域
- WAN（Wide Area Network）：跨城市/国家甚至全球（例如互联网、企业广域网）
- SAN（Storage Area Network）：专用存储网络（光纤通道/iSCSI）
- CAN（Campus/Controller Area Network）：校园/企业园区或车载总线

**记忆：**
- LAN → 单一建筑/楼层
- MAN → 城市级（地铁、城域光环）
- WAN → 跨城/跨国
- SAN → 和“存储”相关，不是地理范围
- CAN → “校园/车载”专用

虽然本题答对，但放进笔记方便以后回顾命名区别。
---

## SAN / NAS / iSCSI / SDN 区分
![SAN question](images/2026-04-01-san.jpg)

**题干：** 哪个缩写表示“专用的本地网络，由多个设备组成，提供集中式数据访问”？

| 选项 | 说明 |
| --- | --- |
| SDN | Software-Defined Networking，指控制面/数据面解耦的网络架构，不是“存储网络” |
| NAS | Network Attached Storage，通常是一台设备，通过 NFS/SMB 提供文件级共享 |
| iSCSI | 一种基于 IP 的块级传输协议，可用来构建 SAN，但本身不是网络类型 |
| **SAN** ✅ | Storage Area Network，独立的高速网络，用于在服务器和存储设备之间提供块级数据访问 |

**记忆：**
- NAS = “设备”→ 文件级共享
- SAN = “网络”→ 块级访问（常用 FC/iSCSI）
- iSCSI = 协议，SDN = 架构
---

## 线缆追踪工具：Toner & Probe
![Toner question](images/2026-04-02-toner.jpg)

**题干：** 哪种工具专门用来在一束电缆中追踪、识别单根线？

|  |  |
| --- | --- |
| ❌ 我的答案 | Wire mapper |
| ✅ 正确答案 | Toner & probe kit |

**说明：**
- Toner（发生器）给目标线缆注入音频信号，Probe（探头）沿束线寻找并通过蜂鸣声定位那根线，非常适合“从机柜追到墙面”的场景。
- Wire mapper 侧重检测双绞线的线序是否正确（T568A/B），无法追踪线缆走向。
- Cable certifier/line tester 则是用于带宽认证、阻抗/衰减测试，功能不同。

**记忆：** 追线 = Toner+Probe，“听声音找线”；查线序 = Wire mapper。
---

## Network tap 用途
![Network tap question](images/2026-04-02-network-tap.jpg)

**题干：** 哪种设备可以在不中断数据流的情况下监听网络流量？

|  |  |
| --- | --- |
| ❌ 我的答案 | Ethernet adapter |
| ✅ 正确答案 | Network tap |

**说明：**
- Network tap（TAP）是一个被动分流设备，把线上通讯复制一份给监控/IDS，原有链路不受影响。
- 普通网卡需要把设备串入链路，会中断/改变流量；Repeater/Transceiver 也不是为监控设计。
- 在交换机时代，SPAN/Port Mirroring 也能做到类似效果，但 TAP 的优点是“物理被动、不会掉包”。

**记忆：** 想监听又不影响业务，首选 **Network TAP**。
---

## 显示面板三兄弟：IPS / TN / VA
![Display technology question](images/2026-04-02-display.jpg)

### IPS（In-Plane Switching）
- ✅ 高色彩精度（High color quality）
- ✅ 宽广视角（Wide viewing angles ≈ 178°）
- ❗ 缺点：响应时间偏慢（Slow response time） ⇒ 不是游戏最佳，但细腻、色准好

### TN（Twisted Nematic）
- ✅ 响应时间最快（Fast response times）
- ✅ 成本低，但色彩一般（Low color quality）
- ✅ 视角最差（Low viewing angles，上下偏色明显）
- ❗ 常用于电竞/办公显示器

### VA（Vertical Alignment）
- ✅ 对比度极高（High contrast ratios，黑位深）
- ✅ 色彩比 TN 好（Good color quality），但不如 IPS
- ✅ 视角比 TN 好、比 IPS 略差（Good viewing angles）
- ❗ 响应时间介于 TN 与 IPS 之间

**速记：**
- *IPS* = Image Perfect & Stable → 色准/视角最好，响应慢
- *TN* = Turbo & Narrow → 响应快，视角窄，色彩弱
- *VA* = Very Amazing Blacks → 对比度王者，综合型选手
---

## 显示面板类型：IPS / TN / VA
![IPS/TN/VA question](images/2026-04-02-display.jpg)

### IPS（In-Plane Switching）
- ✅ 高色彩准确度（High color quality）
- ✅ 宽视角（Wide viewing angles）
- ⚠︎ 响应时间相对慢（Slow response times）

### TN（Twisted Nematic）
- ✅ 响应时间快（Fast response times）
- ✅ 成本低、常见于电竞显示器
- ❌ 视角窄、色彩偏灰（Low color quality）

### VA（Vertical Alignment）
- ✅ 高对比度（High contrast ratios）
- ✅ 色彩与视角介于 IPS 与 TN 之间（Good color quality + Good viewing angles）
- ⚠︎ 响应时间中等，黑场表现优秀

**记忆口诀：**
- IPS = 色准 + 视角；缺点是慢
- TN = 速度快；缺点是色彩/视角差
- VA = 对比度王；折中
---

## 显示参数术语巩固
![Display attributes question](images/2026-04-02-attributes.jpg)

| 概念 | 正确认知 | 记忆重点 |
| --- | --- | --- |
| Pixel density（像素密度） | 同尺寸下像素越多 ⇒ 图像越清晰 | 以 PPI 表示，与“锐利度”直接相关 |
| Refresh rate（刷新率） | 每秒刷新多少次（Hz）⇒ 越高越流畅 | 与动画/游戏流畅度有关 |
| Color depth（色深） | 每像素可显示的色彩数量（bit/pixel） | 8-bit = 16.7M 色，10-bit = 10.7 亿色 |
| **Color gamut（色域）** | 屏幕能覆盖的颜色空间范围（sRGB、DCI-P3 等） | 色域越大，可显示的颜色范围越广、色彩越饱满 |

**Color gamut 补充：**
- 常见色域：sRGB（网页标准）、Adobe RGB（摄影）、DCI-P3（影视）。
- 广色域面板（如 95% DCI-P3）在看 HDR 内容或做设计时更准确。
- 色域 ≠ 色深：一个是“覆盖范围”，一个是“每个颜色点的细腻程度”。
---

## 显示参数匹配：像素密度 / 颜色位深 / 刷新率 / 色域
![Display attributes question](images/2026-04-02-attributes.jpg)

| 概念 | 解释 | 题目正确匹配 |
| --- | --- | --- |
| Color Gamut（色域） | 显示器能覆盖的颜色范围，通常用 sRGB / Adobe RGB / DCI-P3 等标准衡量 | 显示器可呈现的颜色范围 |
| Color Bit Depth（颜色位深） | 每个颜色通道的比特数，决定颜色阶梯数（8-bit=16.7M 色，10-bit=10.7 亿色） | 每像素颜色信息位数 |
| Refresh Rate（刷新率） | 每秒刷新画面的次数（Hz），决定运动画面的流畅度 | 显示器刷新画面的速度 |
| Pixel Density（像素密度） | PPI，单位面积内的像素数量，分辨率 ÷ 尺寸决定清晰度 | 给定显示尺寸和分辨率时的像素数 |

**色域 Color Gamut 补充：**
- 色域越大，可显示的颜色越多，颜色更饱满。
- 常见标准：sRGB（网页）、Adobe RGB（摄影）、DCI-P3（影视）。
- 题目要你匹配“能显示的颜色范围” ⇒ 选 Color Gamut。
---

## 多模光纤特性
![Multimode fiber question](images/2026-04-02-multimode.jpg)

**正确特征（选 3）：**
- 典型传输距离 ≤ 2 km（取决于 OM 级别）
- 成本通常低于单模光纤（接收器/发射器更便宜）
- 使用 **LED**（或 VCSEL）作为光源

**错误认知：**
- “Utilizes laser light” → 这是单模常用（激光/LC laser），多模更多使用 LED/VCSEL。
- “Supports 100 km” → 只有单模才能跑这么远。
- “More expensive” → 实际上多模核心大、器件便宜，成本低。

**记忆：** 多模 = “短距 + LED + 便宜”；单模 = “长距 + 激光 + 贵”。
---

## Direct Burial STP 电缆特性
![Direct burial STP question](images/2026-04-02-direct-burial.jpg)

**正确特征：**
- Enhanced shielding（加强屏蔽）
- Water & chemical resistance（防水/防化学腐蚀）
- Durable outer jacket（抗撕裂、抗压）
- Outdoor / Underground network use（户外/直埋场景）

**为什么不是 Plenum-rated？**
- Plenum 等级是针对建筑内部空气回风层（防火低烟），而直埋电缆关注的是 **防潮 / 防腐 / 防压**；两者应用场景不同。
- 真正要过风管、吊顶才选 Plenum (CMP) 或 Riser (CMR)。

**记忆：** 直埋 = “走地下 / 户外”，关键词是防水、防腐、厚外被；若题目提“火灾、吊顶”，那才是 Plenum。
---

## USB 版本与速率
![USB 2.0 question](images/2026-04-02-usb2.jpg)

| 标称 | 别名 | 理论速率 |
| --- | --- | --- |
| USB 1.1 | Full Speed | 12 Mbps |
| **USB 2.0** | **Hi-Speed** | **480 Mbps** |
| USB 3.2 Gen 1 | SuperSpeed USB | 5 Gbps |
| USB 3.2 Gen 2 | SuperSpeed+ | 10 Gbps |
| USB 3.2 Gen 2x2 | SuperSpeed++ | 20 Gbps |

**记忆：** “2 = 480 Mbps” → 把 2 和 480 组成“2480”方便记忆。越往后代号越乱，建议记住“2=480、3=5G、3.1=10G”。

