
---

## 🛡️ **Use Cases for Threat Detection**

### 1. **Malware Detection**

* Identify abnormal file behavior (e.g., unexpected file encryption).
* Alert when known malicious hashes appear in endpoints or network traffic.

### 2. **Phishing Detection**

* Monitor for suspicious email patterns (e.g., spoofed domains, malicious attachments).
* Alert on users clicking on known malicious URLs.

### 3. **Insider Threats**

* Detect data exfiltration (e.g., large file transfers to external storage).
* Monitor for privilege abuse or unusual login times.

### 4. **Brute Force Attacks**

* Multiple failed login attempts in a short period.
* Lockout or alert on repeated access failures from the same IP/user.

### 5. **Command & Control (C2) Communications**

* Alert on outbound traffic to known C2 servers.
* Look for unusual DNS queries or beaconing behavior.

### 6. **Ransomware Activity**

* Detect mass file renaming/encryption.
* Monitor for unusual process execution (e.g., PowerShell + obfuscation).

### 7. **Privilege Escalation**

* Detect sudden privilege changes or use of privilege escalation tools (e.g., Mimikatz).
* Monitor for suspicious access to `Admin`, `Domain Controller`, etc.

### 8. **Unusual Network Traffic**

* Traffic spikes or patterns outside business hours.
* Unexpected geographic IP access (e.g., login from China while user is in the US).

### 9. **Data Exfiltration**

* Abnormal outbound data volume or uploads to external services (Dropbox, WeTransfer).
* Steganography or encrypted traffic with no clear business need.

### 10. **Anomalous User Behavior**

* User logging in from two countries within minutes (impossible travel).
* Accessing systems or files they normally don’t interact with.

### 11. **Lateral Movement Detection**

* Alert on internal IP-to-IP communication that breaks network segmentation.
* Detection of tools like PsExec, RDP, SMB enumeration.

### 12. **Software Exploits**

* Detection of exploitation attempts (e.g., log4j, buffer overflow patterns).
* IDS/IPS logs showing known exploit signatures.

---

