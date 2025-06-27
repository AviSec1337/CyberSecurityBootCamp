---

# 🛡️ CyberSecurity BootCamp - Day 3

Welcome to Day 3 of the Wazuh training program. This session focuses on hands-on tasks for deploying and utilizing Wazuh in a security monitoring environment. Below are the questions, tasks, and configuration snippets needed for today's exercises.

---

## 📌 Questions

Please answer the following before starting today's tasks:

1. **Who installed Wazuh on their environment?**
2. **Who enrolled at least one agent on the Wazuh server?**

---

## ✅ Tasks

### 🔐 Task 1: Agent Enrollment (Linux and Windows)

Enroll at least one Wazuh agent to your Wazuh server.

* **Linux Agent:** Follow [Wazuh Linux agent installation guide](https://documentation.wazuh.com/current/installation-guide/installing-wazuh-agent/index.html#linux)
* **Windows Agent:** Follow [Wazuh Windows agent installation guide](https://documentation.wazuh.com/current/installation-guide/installing-wazuh-agent/index.html#windows)

Once installed, verify that the agent is connected and reporting to the Wazuh server.

---

### 🗂️ Task 2: File Integrity Monitoring (FIM)

Set up File Integrity Monitoring on both Windows and Ubuntu endpoints.

#### 🔧 Windows Endpoint

Edit the agent's `ossec.conf` to include:

```xml
<directories check_all="yes" report_changes="yes" realtime="yes">C:\Users\<USER_NAME>\Desktop</directories>
```

Replace `<USER_NAME>` with the actual user account name.

#### 🐧 Ubuntu Endpoint

Edit the agent's `ossec.conf` to include:

```xml
<directories check_all="yes" report_changes="yes" realtime="yes">/root</directories>
```

Restart the agent after configuration changes for them to take effect.

---

### 🧨 Task 3: Attack a Vulnerable Web Application and Monitor Logs

Simulate an attack on a vulnerable web application such as [DVWA](http://www.dvwa.co.uk/) or [Mutillidae](https://sourceforge.net/projects/mutillidae/). Observe how Wazuh logs and detects the malicious behavior.

Steps:

1. Launch the vulnerable web app.
2. Use tools like OWASP ZAP, SQLMap, or Burp Suite to simulate attacks.
3. Monitor the alerts generated in Wazuh under **Security Events**.
4. Take screenshots or export logs as evidence of detection.

---

## 📁 Useful Links

* [Wazuh Documentation](https://documentation.wazuh.com/)
* [Wazuh GitHub Repository](https://github.com/wazuh/wazuh)
* [Community Slack](https://wazuh.com/community/)

---

## 📝 Notes

* Ensure Wazuh Manager and Agent clocks are synced to avoid log timestamp issues.
* Backup configurations before making changes.
* Always run tests in a controlled lab environment.

---

Let your instructor or mentor know once you've completed all the tasks for review and feedback.

Happy monitoring!

---
