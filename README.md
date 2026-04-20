# CTF Attack Chain Analysis (Full System Compromise)

## 📄 Full Technical Report
👉 [View Report](./report/ctf-attack-chain.pdf)

## Overview
This project demonstrates a multi-stage attack chain in a Capture The Flag (CTF) environment, showing how multiple small vulnerabilities can be combined to achieve full system compromise.

## 🔗 Attack Chain Overview
- Initial access via exposed services (rsync)
- Discovery of hidden internal web application
- Exploitation of insecure configurations
- Abuse of cryptographic weaknesses
- SQL Injection for data extraction
- Privilege escalation to root access

## 🔍 Key Findings
- Misconfigured rsync service exposed sensitive data
- Weak access controls in internal web services
- Vulnerable input handling leading to SQL Injection
- Poor cryptographic practices enabling decryption
- Misconfigured sudo permissions allowed privilege escalation

## ⚠️ Security Impact
- Complete system compromise (root access)
- Exposure of sensitive files and credentials
- Authentication bypass and unauthorized access
- Multiple attack vectors chained together

## 🛡️ Mitigation Strategies
- Restrict access to sensitive services (rsync, SSH)
- Validate and sanitize user inputs
- Implement proper authentication and authorization
- Use strong encryption and secure key management
- Apply least privilege principle

## 🛠️ Tools & Techniques
- Nmap
- rsync enumeration
- SQL Injection
- Linux privilege escalation techniques
- Forensic analysis

## 📌 Conclusion
This project highlights how attackers combine multiple vulnerabilities to achieve full compromise, emphasizing the importance of layered security and proper system configuration.
