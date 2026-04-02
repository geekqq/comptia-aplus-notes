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

