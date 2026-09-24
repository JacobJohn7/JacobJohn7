# Hi, I'm Jacob John 👋

Cybersecurity student preparing for **CompTIA Security+ (SY0-801)** with a focus on Security Operations Center (SOC) analysis, network security monitoring (NSM), Active Directory administration, and endpoint hardening.

I build hands-on virtual laboratory environments (VirtualBox, pfSense, Windows Server 2019/2022, Active Directory, Ubuntu, Arch Linux) to practice real-world detection, log correlation, and threat mitigation.

---

### 🛡️ Featured Hands-On Security Labs

- **[Active-Directory-Lab-Homelab](https://github.com/JacobJohn7/Active-Directory-Lab-Homelab)**  
  Active Directory Domain Services (AD DS) infrastructure on Windows Server 2019 (`DC01` - `192.168.56.10`, domain `homelab.local`). Features automated PowerShell provisioning script (`Deploy-ADLab.ps1`) for Organizational Units (OUs), security groups (`Sec_Tier1_SOC`), and users, alongside domain-joined Windows 10 workstation setup (`192.168.56.108`) and AD port/service dissection (KDC 88/464, LDAP 389/636, SMB 445, Global Catalog 3268, WinRM 5985).

- **[Linux-Server-Hardening-Auditd-Fail2ban](https://github.com/JacobJohn7/Linux-Server-Hardening-Auditd-Fail2ban)**  
  Ubuntu Server security hardening featuring OpenSSH daemon configuration (`PermitRootLogin no`, `MaxAuthTries 4`, `ClientAliveInterval 15`), **UFW** stateful host firewall policy (default deny incoming/routed), **Fail2Ban** intrusion prevention with UFW banaction binding (`banaction = ufw`), and Linux **Auditd** CIS benchmark rules (`/etc/audit/rules.d/cis-hardening.rules`) tracking credential files and privilege modifications.

- **[pfSense-Suricata-NIPS-Lab](https://github.com/JacobJohn7/pfSense-Suricata-NIPS-Lab)**  
  Enterprise virtual firewall deployment (`pfSense 2.7.2`) configured as a central gateway for a multi-VM lab. Features hard network isolation (NAT disabled on client VMs to enforce 100% gateway inspection), **Suricata Inline NIPS** via BSD `netmap`, `snort2c` kernel table IP blocking, and **pfBlockerNG-devel** DNSBL domain sinkholing via Unbound DNS resolver.

- **[Windows-OS-Hardening-Sysmon-Lab](https://github.com/JacobJohn7/Windows-OS-Hardening-Sysmon-Lab)**  
  Windows 10 endpoint security hardening aligned with CIS Benchmarks (disabling SMBv1, LLMNR/NBT-NS, administrative auto-shares) and PowerShell Script Block Logging (Event ID 4104). Deploys **Sysmon v15.x** with custom XML telemetry rules for process creation (`Event ID 1`), network connections (`Event ID 3`), executable drops (`Event ID 11`), and DNS queries (`Event ID 22`).

- **[Network-Traffic-Analysis-IDS-Lab](https://github.com/JacobJohn7/Network-Traffic-Analysis-IDS-Lab)**  
  Network traffic analysis and intrusion detection lab combining **`tshark`** CLI PCAP triage (HTTP request extraction, TCP SYN scan aggregation), **`Zeek`** protocol session logging (`conn.log`, `http.log`, `dns.log`), custom **`Suricata`** web shell signatures (`local.rules`), and VirtualBox TCP checksum offloading configuration (`checksum-validation: no`).

---

### 🧰 Core Technical Toolkit

- **Active Directory & Identity:** AD DS, Domain Controller (Windows Server 2019/2022), Group Policy (GPO), Kerberos, LDAP/LDAPS, PowerShell ActiveDirectory Module, WinRM.
- **SIEM & Log Analytics:** Splunk Enterprise, SPL Queries, Universal Forwarder, Windows Event Viewer, Sysmon Operational Channel, MITRE ATT&CK Mapping.
- **Network Security & Firewalls:** pfSense 2.7.x, Suricata (NIDS/NIPS), pfBlockerNG-devel, Unbound DNS Resolver, BSD `netmap`, `pfctl`, UFW, Fail2Ban.
- **Endpoint Hardening & OS:** OpenSSH Hardening, Linux Auditd, CIS Benchmarks, Sysmon v15.x, Windows Server 2019/2022, Ubuntu Server/Desktop, Arch Linux.
- **Packet Analysis & Telemetry:** Zeek (Bro), `tshark` / Wireshark, PCAP slicing, TCP/IP protocol dissection.

---

### 📬 Contact & Links

- **GitHub Profile:** [github.com/JacobJohn7](https://github.com/JacobJohn7)
- **Target Certification:** CompTIA Security+ (SY0-801)
