# Hi, I'm Jacob John 👋

Cybersecurity student preparing for **CompTIA Security+ (SY0-701)** with a focus on Security Operations Center (SOC) analysis, network security monitoring (NSM), endpoint hardening, and SIEM rule engineering.

I build hands-on virtual laboratory environments (VirtualBox, pfSense, Windows Server 2022, Ubuntu, Arch Linux) to practice real-world detection, log correlation, and threat mitigation.

---

### 🛡️ Featured Hands-On Security Labs

- **[pfSense-Suricata-NIPS-Lab](https://github.com/JacobJohn7/pfSense-Suricata-NIPS-Lab)**  
  Enterprise virtual firewall deployment (`pfSense 2.7.2`) configured as a central gateway for a multi-VM lab. Features hard network isolation (NAT disabled on client VMs to enforce 100% gateway inspection), **Suricata Inline NIPS** via BSD `netmap`, `snort2c` kernel table IP blocking, and **pfBlockerNG-devel** DNSBL domain sinkholing via Unbound DNS resolver.

- **[Windows-OS-Hardening-Sysmon-Lab](https://github.com/JacobJohn7/Windows-OS-Hardening-Sysmon-Lab)**  
  Windows 10 endpoint security hardening aligned with CIS Benchmarks (disabling SMBv1, LLMNR/NBT-NS, administrative auto-shares) and PowerShell Script Block Logging (Event ID 4104). Deploys **Sysmon v15.x** with custom XML telemetry rules for process creation (`Event ID 1`), network connections (`Event ID 3`), executable drops (`Event ID 11`), and DNS queries (`Event ID 22`).

- **[SOC-Incident-Report-BruteForce-Splunk](https://github.com/JacobJohn7/SOC-Incident-Report-BruteForce-Splunk)**  
  Windows Active Directory authentication log ingestion (`inputs.conf`) into **Splunk Enterprise**. Features custom SPL queries for NTLM/Kerberos substatus code analysis (`0xc000006a` bad password vs `0xc0000064` user not found), failure-to-compromise correlation (`EventID 4625` -> `4624`), threshold alerting, and Active Directory machine account noise filtering (`TargetUserName!="*$"`).

- **[Network-Traffic-Analysis-IDS-Lab](https://github.com/JacobJohn7/Network-Traffic-Analysis-IDS-Lab)**  
  Network traffic analysis and intrusion detection lab combining **`tshark`** CLI PCAP triage (HTTP request extraction, TCP SYN scan aggregation), **`Zeek`** protocol session logging (`conn.log`, `http.log`, `dns.log`), custom **`Suricata`** web shell signatures (`local.rules`), and VirtualBox TCP checksum offloading configuration (`checksum-validation: no`).

---

### 🧰 Core Technical Toolkit

- **SIEM & Log Analytics:** Splunk Enterprise, SPL Queries, Universal Forwarder, Windows Event Viewer, Sysmon Operational Channel, MITRE ATT&CK Mapping.
- **Network Security & Firewalls:** pfSense 2.7.x, Suricata (NIDS/NIPS), pfBlockerNG-devel, Unbound DNS Resolver, BSD `netmap`, `pfctl`.
- **Packet Analysis & Telemetry:** Zeek (Bro), `tshark` / Wireshark, PCAP slicing, TCP/IP protocol dissection.
- **Endpoint Security & OS:** Windows Server 2022, Windows 10, Ubuntu Server/Desktop, Arch Linux, PowerShell, Bash scripting.

---

### 📬 Contact & Links

- **GitHub Profile:** [github.com/JacobJohn7](https://github.com/JacobJohn7)
- **Target Certification:** CompTIA Security+ (SY0-701)
