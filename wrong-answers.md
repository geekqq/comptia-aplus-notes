# CompTIA A+ Wrong-Answer Notebook

## Telnet core features
**Original prompt:** “Which of the following statements describe an important feature or service provided by Telnet? (Select three.)”

![Telnet question screenshot](images/20260330-telnet.jpg)


**Correct choices:**
- Provides username and password authentication
- Transmits data in an unencrypted form
- Enables remote login and command execution

**Key takeaways:**
- Telnet does have basic login prompts, but it sends *everything* in clear text, so credentials can be sniffed easily.
- Because there is no encryption or integrity protection, Telnet should only be used on trusted internal labs. SSH has replaced it for real-world remote administration.
- Any answer claiming Telnet “does not provide authentication” is a trap—it *does*, it’s just insecure.
---

## Server roles – document output vs storage
![Server role question](images/2026-03-31-print-server.jpg)

**Question:** "Which type of server does not primarily store files but facilitates document output?"

|  |  |
| --- | --- |
| ❌ My answer | database server |
| ✅ Correct | print server |

**Key takeaways**
- Print servers sit between users and printers: they accept print jobs, spool them, manage queues, and forward jobs to the right device. Their role is document *output*, not long-term file storage.
- Database, web, and application servers focus on storing/processing data or hosting apps, but none are tailored to printer spooling.
- File servers (NAS/SAN) are the ones optimized for storing files.

**Memory hook:** Print server = "document traffic controller"—think of it as the dispatcher for printers, not a storage bin.
---

## Wireless basics – channel width, Bluetooth traits, 802.11 features
![Wireless question set](images/2026-03-31-wireless.jpg)

### 1. Increasing channel width
- ❌ My answer: "Reduces interference from neighboring channels"
- ✅ Correct: "Increases data throughput but may cause more interference"

**Why:** Wider channels (40/80/160 MHz) give more bandwidth, but their larger footprint overlaps more adjacent channels, so interference risk rises instead of shrinking. Use narrow 20 MHz in noisy environments.

### 2. Bluetooth characteristics (select all that apply)
- ❌ Missed: Operates in the 2.4 GHz ISM band
- ❌ Incorrectly chose: Requires line-of-sight (其实 BT 是短距射频，不需要 LOS)
- ✅ Correct traits:
  - 2.4 GHz ISM band
  - Short-range wireless communication
  - Optimized for creating PANs
  - Used for peripherals / wearables / IoT

**Why:** Bluetooth is a frequency-hopping spread spectrum tech in the 2.4 GHz band. It’s meant for PANs and peripherals. Line-of-sight是红外的特性，不是 BT。

### 3. 802.11 network characteristics (select 3)
- ❌ Missed: Built to support both infrastructure and ad-hoc topologies
- ❌ Incorrectly chose: Designed to operate in licensed bands (802.11 uses unlicensed ISM/UNII bands)
- ✅ Correct picks:
  - Supports infrastructure + ad-hoc
  - Engineered for high-speed wireless data transmission
  - Standardized by IEEE as a wireless alternative to wired LANs

**Memory hooks:**
- Channel width ↑ ⇒ throughput ↑ but interference ↑
- Bluetooth = 2.4 GHz PAN, no line-of-sight requirement.
- 802.11 = IEEE WLANs in unlicensed bands, works in infrastructure or ad-hoc.
---

## 2.4 GHz vs higher bands
![2.4 GHz comparison question](images/2026-03-31-24ghz.jpg)

**Question:** Characteristics of the 2.4 GHz band compared to 5/6 GHz (select 3).

|  |  |
| --- | --- |
| ❌ My wrong pick | "A wider number of available channels with less overlap" |
| ❌ Missed | "The lowest number of non-overlapping channels" |
| ✅ Already got | Longest range; higher susceptibility to interference |

**Why:**
- 2.4 GHz travels farther / penetrates walls better, but the band is crowded (Bluetooth, microwaves, etc.), so interference risk is high.
- It only has **3** non-overlapping channels (1/6/11 in many regions). That’s the *fewest*, not the widest.
- 5 GHz/6 GHz bands provide more spectrum and more non-overlapping channels, so they suffer less overlap.

**Memory hook:** 2.4 GHz = "far but few" — further reach, but only a few clean channels.
---

## TCP port 445 – SMB/CIFS, not IMAP
![TCP 445 question](images/2026-03-31-tcp445.jpg)

**Question:** Which service runs on TCP port 445?

|  |  |
| --- | --- |
| ❌ My answer | IMAP |
| ✅ Correct | SMB (a.k.a. CIFS) |

**Why:**
- Port 445/TCP is used by Microsoft SMB over TCP (file & printer sharing). Windows uses it for network shares.
- IMAP uses 143 (unencrypted) / 993 (IMAPS).
- HTTPS = 443, LDAPS = 636. 445 is the odd one out dedicated to SMB.

**Memory hook:** Think "4-4-5" → 44 = Windows (WinNT), **5** = SMB. Or remember the trio 143/443/445/636 (mail/web/file/LDAP).

