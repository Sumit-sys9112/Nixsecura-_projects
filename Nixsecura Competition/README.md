# 🛡️ CTF Walkthrough

Welcome to the **Capture The Flag (CTF) Walkthrough**! This guide takes you step by step through the process of identifying vulnerabilities and exploiting them in a controlled environment.

## ⚙️ Tools Used

- **🔍 Netdiscover**: For network discovery using ARP requests.
- **🌐 Nmap**: For network scanning and discovering open ports and services.
- **📁 Dirsearch**: For brute-forcing web directories and hidden files.
- **🔐 Hydra**: For brute-forcing login credentials.
- **🐙 Wireshark**: For analyzing network traffic.

## 🚀 Steps Overview

### 1. **Network Discovery**
- Utilized `Netdiscover` to identify live hosts within the subnet.

### 2. **Port Scanning**
- Conducted scanning with `Nmap` to discover open ports and services running.

### 3. **Web Page Analysis**
- Accessed the target's web page but found no immediate clues.

### 4. **Directory Bruteforce**
- Employed `dirsearch` to identify hidden directories, discovering a `robots.txt` file.

### 5. **Decoding Hidden Data**
- Found encoded data and decoded it using Base64 to uncover sensitive paths.

### 6. **File Analysis**
- Accessed a hidden path to download a `.pcapng` file and analyzed it using `Wireshark`.

### 7. **Credential Discovery**
- Identified FTP credentials by filtering for FTP traffic in the packet capture.

### 8. **FTP Access**
- Logged into the FTP server using discovered credentials and downloaded `users.txt` and `pass.txt`.

### 9. **Brute-Forcing SSH**
- Used `Hydra` with the downloaded username and password lists to brute-force SSH access.

### 10. **SSH Login**
- Successfully logged into SSH, discovering user and root flags.

### 11. **Investigative Analysis**
- Found a `TNIH.txt` file with hints suggesting checking multiple user accounts.

### 12. **User Enumeration**
- Identified three users (Marco, Murfy, Nixsecura) and attempted to access their accounts.

### 13. **Brute-Forcing User Password**
- Brute-forced the password for the `Nixsecura` user account.

### 14. **Root Access**
- Achieved root access by creating an executable in the `/tmp` directory, finalizing the challenge.

## ✅ Conclusion

Successfully captured both the user and root flags! This walkthrough demonstrates effective use of network discovery, enumeration, brute-forcing, and privilege escalation techniques.

---

**Happy Hacking! ⚔️**

