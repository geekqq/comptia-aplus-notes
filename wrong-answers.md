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

