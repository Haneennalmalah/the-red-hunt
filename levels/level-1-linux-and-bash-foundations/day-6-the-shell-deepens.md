# Day 6 — The Shell Deepens

> “They say the shell is just a tool. But in this place… it’s a weapon, a compass, and a way out.”

---

##  What Aroha Learned

Today was a deep dive. As the virtual environment shifted around her, cold terminals flickered open, whispering secrets in green. Here's what she uncovered:

### Network & Process Utilities

- `ifconfig` – Inspected her network interfaces like a true digital cartographer.
- `free` – Took a glance at the system’s memory.
- `df -H` – Measured the disk usage in a more human-friendly format.
- `ps aux` – Explored all running processes.
- `kill <pid>` – Learned how to terminate rogue processes like a silent assassin.

### Installing & Managing Packages

- `apt install <app>` – Installed essential tools (like `snap`) via the package manager.
- `snap install <app>` – Used Snap to install Spotify.
- `dpkg -i <file>.deb` – Manually installed Chrome using `.deb` packages.

 Discovered the life-saving `sudo !!` trick to rerun previous commands with root privileges.

### File Permissions & Ownership

- Learned the meaning behind permission bits:
  - `r` (4) – read
  - `w` (2) – write
  - `x` (1) – execute
- Added them up (e.g. `5 = r+x`, `7 = full access`) to understand how files are accessed.
- Observed:
  - The three permission sections represent: **owner**, **group**, and **others**.
- Ran:
  - `ls -lah` – Viewed file permissions and metadata clearly.
  - `chmod` – Modified permissions:
    - `chmod 777 gumball.jpg` – Gave full access to all.
    - `chmod +x GIFutil.dll` – Made a file executable.
    - `chmod -r GIFutil.dll` – Removed read permissions.
- Understood ownership:
  - `root root`, `kali kali` – The first is the owner, the second is the group.

### Other Powerful Tools

- `cat` – Viewed the content of files.
- `grep` – Searched within files like a forensic investigator.
- `wc` – Counted words/lines for summaries.
  
### 💻 VPS & Segfault Exploration

- Learned how to connect to a **Virtual Private Server (VPS)**.
- Connected to the **Segfault CTF environment** using:

```bash
ssh -o "SetEnv SECRET=HzrKAQJYrRayXHYxdYulyfNp" root@lsd.segfault.net
