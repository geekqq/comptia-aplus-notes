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
