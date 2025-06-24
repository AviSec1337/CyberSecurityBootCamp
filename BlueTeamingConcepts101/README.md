
---

## 🔵 **Blue Teaming: Basics**

**Blue Teaming** refers to the **defensive side of cybersecurity**, where the main goal is to **detect, respond to, and prevent cyber threats**.

---

## 🧠 **Core Concepts**

### 1. **Defense-in-Depth**

* A layered security approach.
* If one control fails, others still provide protection.
* Examples: firewall + antivirus + endpoint detection + logging.

### 2. **Security Monitoring**

* Watching systems for signs of malicious activity.
* Use of tools like **SIEM** (e.g., Splunk, ELK Stack).

### 3. **Incident Response (IR)**

* The process of identifying, managing, and recovering from cyber incidents.
* Phases: **Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned**.

### 4. **Threat Hunting**

* Proactively looking for threats that evaded detection.
* Uses threat intelligence and behavioral analysis.

### 5. **Vulnerability Management**

* Identifying, evaluating, and fixing vulnerabilities.
* Tools: Nessus, OpenVAS, Qualys.

### 6. **Log Analysis**

* Reviewing logs (from firewalls, servers, etc.) to detect unusual activity.

### 7. **Patch Management**

* Keeping software updated to prevent exploitation of known vulnerabilities.

### 8. **Network Security**

* Securing the network through:

  * Firewalls
  * IDS/IPS (Intrusion Detection/Prevention Systems)
  * VLANs
  * Segmentation

### 9. **Endpoint Protection**

* Protecting individual devices (laptops, servers, etc.).
* Tools: EDR (Endpoint Detection and Response), Antivirus.

### 10. **Security Policies and Procedures**

* Written guidelines to manage how systems and data are protected.
* Includes Acceptable Use Policies (AUPs), Incident Response Plans, etc.

---

## 🧰 **Common Tools**

| Category              | Examples                           |
| --------------------- | ---------------------------------- |
| SIEM                  | Splunk, ELK Stack, IBM QRadar      |
| EDR                   | CrowdStrike, SentinelOne, Defender |
| IDS/IPS               | Snort, Suricata, Zeek              |
| Vulnerability Scanner | Nessus, OpenVAS, Qualys            |
| Log Management        | Graylog, Logstash                  |
| Forensics             | Autopsy, Volatility, FTK           |
| Packet Analysis       | Wireshark, tcpdump                 |
| Threat Intelligence   | MISP, AlienVault OTX, VirusTotal   |

---

## 🧩 **Key Terms & Definitions**

| Term                                  | Meaning                                                                       |
| ------------------------------------- | ----------------------------------------------------------------------------- |
| IOC (Indicator of Compromise)         | Evidence that a breach has occurred (e.g., IP, domain, file hash)             |
| TTP (Tactics, Techniques, Procedures) | How attackers operate, based on MITRE ATT\&CK                                 |
| MITRE ATT\&CK                         | A framework that describes attacker behavior in stages                        |
| SOC (Security Operations Center)      | A team that monitors and defends an organization's network                    |
| Zero Trust                            | Security model assuming no one is trusted by default, even inside the network |
| Least Privilege                       | Giving users the minimum access needed to perform their jobs                  |
| Honeypot                              | A decoy system used to lure attackers and study their behavior                |
| Whitelisting                          | Only allowing known-safe apps or processes to run                             |
| Blacklisting                          | Blocking known-bad apps or IPs                                                |

---

## 📚 **Learning Resources**

* **TryHackMe – Blue Team Path**
* **CyberDefenders.org – Blue Team Labs**
* **MITRE ATT\&CK**: [https://attack.mitre.org](https://attack.mitre.org)
* **NIST Cybersecurity Framework**: [https://www.nist.gov/cyberframework](https://www.nist.gov/cyberframework)

---

