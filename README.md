# <ins> *_Guard The Castle - Home Labs_* </ins>

<p align="center">
  <img width="900" height="500" src="https://pixeljoint.com/files/icons/full/addeddragonreflection.gif">
</p>

# <ins> Objective </ins>
Guard The Castle aims to provide a starting point for aspiring Blue Team Cybersecurity Professionals looking to begin their journey or expand their knowledge of Cybersecurity through the use of home labs and practical learning!  
  
With the growing number of tools and resources available it can be difficult to know where to start. This repository hopes to provide a healthy foundation of tools that you can look to add to your arsenal. Some tools appear on the list more than once due to their diverse features. For example a tool may work as both a HIDS but have EDR functionality as well.
  
Guard the Castle was structured to be used by anyone and everyone, as such only **FREE** and/or **OPEN-SOURCE** tools are mentioned. 
> :grey_exclamation: Disclaimer, some of the tools mentioned have a paid version that offers a more comprehensive solution. For the purpose of this project it is NOT necessary to use the paid versions, however some offer free trial periods to test out the additional features. I strongly suggest establishing a strong understanding of the free version before you use these trials to get the most out of it.

> :information_source:  Links to download the tools used and the related documentation will also be provided.

# <ins> Contents </ins>
- Endpoint / Extended Detection and Response ( EDR / XDR )
  - OSSEC
  - Wazuh
- Firewalls
  - IPFire
  - IPTables
  - OPNsense
  - pfSense
- Honeytokens / Honeypots
  - Canarytokens
  - Manuka
  - OpenCanary
- Incident Response
  - The Hive
- Infrastructure Deployment / Maintenance
  - Ansible
  - Oracle VM VirtualBox
  - Terraform
  - Vagrant
- Intrusion Detection / Prevention Systems (IDS / IPS)
  - Fail2Ban
  - OSSEC
  - Snort
- Network Analysis Tools (Network Analysers)
  - Wireshark
  - Zeek
- Network Mapping Tools
  - Angry IP Scanner
  - Masscan
  - nmap
  - zmap
- Programming / Scripting / Decarative (Database) Languages
  - Bash
  - C
  - JavaScript
  - Powershell
  - Python
  - Structured Query Language (SQL)
- Security Distributions (Linux)
  - Kali Linux
  - ParrotOS
  - Security Onion
- Security Information and Event Management (SIEM)
  - OpenSearch
    - Security Analytics for Opensearch
  - Prelude OSS
  - Wazuh

## Endpoint / Extended Detection and Response ( EDR / XDR )

##### **OSSEC** ( [Download](https://www.ossec.net/ossec-downloads/) / [Documentation](https://www.ossec.net/docs/) ) - _Open Source Host-Based Intrusion Detection System (HIDS) with EDR functions_

##### **Wazuh** ( [Download](https://wazuh.com/install/) / [Documentation](https://documentation.wazuh.com/current/index.html) ) - _Open source security platform that unifies XDR and SIEM capabilities._
  
## Firewalls
  
##### **IPFire** ( [Download](https://www.ipfire.org/downloads/ipfire-2.29-core187) / [Documentation](https://www.ipfire.org/docs) ) - _Linux distribution hardened to act as a dedicated stateful inspection firewall._
  
##### **IPTables** ( [Documentation](https://linux.die.net/man/8/iptables) ) - _User-space utility program that allows a system administrator to configure the IP packet filter rules of the Linux kernel firewall._
  ##### **UFW** ( [Documentation](https://help.ubuntu.com/community/UFW) ) - _Provides a user-friendly interface to modify the IPTables for Ubunutu._
  ##### **Firewalld** ( [Documentation](https://firewalld.org/documentation/) ) - _Provides a user-friendly interface to modify the IPTables for Centos/RedHat._

##### **OPNsense** ( [Download](https://opnsense.org/download/) / [Documentation](https://docs.opnsense.org/) ) - _Easy-to-use and easy-to-build FreeBSD based firewall and routing platform._

##### **pfSense** ( [Download](https://www.pfsense.org/download/ ) / [Documentation](https://docs.netgate.com/pfsense/en/latest/?_gl=1*jffkzm*_gcl_au*MjEyMzA0MTk5LjE3MjU1MDQwOTk.*_ga*OTkxOTIyMDk4LjE3MjU1MDQwOTk.*_ga_TM99KBGXCB*MTcyNTUwNDA5OS4xLjEuMTcyNTUwNDE0NS4xNC4wLjA.) ) - _Customised distribution of FreeBSD tailored for use as a firewall and router._
    
##### **Windows Defender Firewall** ( [Documentation](https://learn.microsoft.com/en-us/windows/security/operating-system-security/network-security/windows-firewall/) ) - Host-based firewall that is included with the Windows._

## Honeytokens / Honeypots

##### **Canarytokens** ( [Download](https://github.com/thinkst/canarytokens-docker) / [Documentation](https://docs.canarytokens.org/guide/) ) - _Opensource Honeytokens for networks, computers, clouds and phones_

##### **Manuka** ( [Download](https://github.com/spaceraccoon/manuka) / [Documentation](https://github.com/spaceraccoon/manuka) ) - _Open-source intelligence (OSINT) honeypot that monitors reconnaissance attempts by threat actors._
  
##### **OpenCanary** ( [Download](https://github.com/thinkst/opencanary?tab=readme-ov-file#installation) / [Documentation](https://opencanary.readthedocs.io/en/latest/) ) - _Daemon that runs canary services, which trigger alerts when used._

## Incident Response

##### **The Hive** ( [Download](https://docs.strangebee.com/thehive/download/) / [Documentation](https://docs.strangebee.com/) ) - _Incident Response Platform._

## Infrastructure Deployment / Maintenance

##### **Ansible** ( [Download](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) / [Documentation](https://docs.ansible.com/users.html) ) - _Infrastrucutre as code tool used for configuration management_

##### **Oracle VM VirtualBox** ( [Download](https://www.virtualbox.org/wiki/Downloads) / [Documentation](https://www.virtualbox.org/wiki/Documentation) ) - _Virtualisation software used to create Virtual Machines_

##### **Terraform** ( [Download](https://developer.hashicorp.com/terraform/install?product_intent=terraform) / [Documentation](https://developer.hashicorp.com/terraform/docs) ) - _Infrastructure as code tool that lets you define both cloud and on-prem resources._
  
##### **Vagrant** ( [Download](https://developer.hashicorp.com/vagrant/install?product_intent=vagrant) / [Documentation](https://developer.hashicorp.com/vagrant/docs) ) - _Tool for building and managing virtual machine environments in a single workflow._

## Intrusion Detection / Prevention Systems (IDS/IPS)

##### **Fail2Ban** ( [Download](https://github.com/fail2ban/fail2ban) / [Documentation](https://github.com/fail2ban/fail2ban/tree/master/man) ) - _Python Written IPS software framework designed to prevent brute-force attacks_

##### **OSSEC** ( [Download](https://www.ossec.net/ossec-downloads/) / [Documentation](https://www.ossec.net/docs/) ) - _Open Source Host-Based Intrusion Detection System (HIDS) with EDR functions_

##### **Snort** ( [Download](https://www.snort.org/downloads) / [Documentation](https://www.snort.org/documents) ) - _Open source Network-Based Intrusion Prevention System (NIPS)._

## Network Analysis Tools (Network Analysers)

##### **Wireshark** ( [Download](https://www.wireshark.org/download.html) / [Documentation](https://www.wireshark.org/docs/wsug_html_chunked/index.html) ) - _Network packet and protocol analyser, prsenting captured data in as much detail as possible._

##### **Zeek** ( [Download](https://zeek.org/get-zeek/) / [Documentation](https://docs.zeek.org/en/master/index.html) ) - _Passive, Open-Source network traffic analyser._

## Network Mapping Tools

##### **Angry IP Scanner** ( [Download](https://angryip.org/download/#windows) / [Documentation](https://angryip.org/documentation/#google_vignette) ) - _Widely-used open-source and multi-platform network scanner._

##### **Masscan** ( [Download](https://www.kali.org/tools/masscan/#masscan) / [Documentation](https://www.kali.org/tools/masscan/) ) - _Similar to nmap however operates much faster and can scan a large number of ports._

##### **nmap** ( [Download](https://nmap.org/download) / [Documentation](https://nmap.org/docs.html) ) - _Open source tool for network exploration and security auditing._

##### **zmap** ( [Download](https://github.com/zmap/zmap?tab=readme-ov-file) / [Documentation](https://github.com/zmap/zmap/wiki/Getting-Started-Guide) ) - _Fast single packet network scanner designed for Internet-wide network surveys._

## Programming / Scripting / Decarative (Database) Languages

##### **[Bash](https://www.gnu.org/software/bash/)** - _Default scripting language for most Linux distributions._

##### **[C](https://devdocs.io/c/)** - _General-purpose programming language that provides low-level access to system memory_

##### **[GoLang](https://go.dev/doc/)** - _High-level programming language designed at Google_

##### **[JavaScript](https://devdocs.io/javascript/)** - _Most popular programming language for Web pages_

##### **[Powershell](https://learn.microsoft.com/en-us/powershell/)** - _Default scripting language for Windows._

##### **[Python](https://docs.python.org/3/)** - _Clear and powerful object-oriented programming language_

##### **[Structured Query Language (SQL)](https://dev.mysql.com/doc/)** - _Language used to query SQL or “relational” databases._

> I have only provided the links to the official documentation. Many of these langauges are already pre-installed on distributions or can be easily accessed either by installing packages or installing an IDE like VS Code or PyCharm. There is also a plethora of free and accessible training material for these languages. Find a method that suits your learning style.

## Security Distributions (Linux)

##### **Kali Linux** ( [Download](https://www.kali.org/get-kali/#kali-platforms) / [Documentation](https://www.kali.org/docs/) ) - _Distribution which allows users to perform advanced penetration testing and security auditing.*

##### **ParrotOS** ( [Download](https://parrotsec.org/download/) / [Documentation](https://parrotsec.org/docs/) ) - _Distribution designed for security experts, developers and privacy aware people._

##### **Security Onion** ( [Download](https://github.com/Security-Onion-Solutions/securityonion/blob/2.4/main/DOWNLOAD_AND_VERIFY_ISO.md) / [Documentation](https://docs.securityonion.net/en/2.4/) ) - _Distribution built by defenders for defenders_

## Security Information and Event Management (SIEM)

##### **OpenSearch** ( [Download](https://opensearch.org/downloads.html) / [Documentation](https://opensearch.org/docs/latest/)) - _Distributed search and analytics engine._

##### **Security Analytics for OpenSearch** ( [Documentation](https://github.com/opensearch-project/security-analytics/tree/main) ) - _Security Information and Event Management (SIEM) solution for OpenSearch._

##### **Prelude OSS** ( [Download](https://www.prelude-siem.org/projects/prelude/files) / [Documentation](https://www.prelude-siem.org/projects/prelude/wiki) ) - _Agentless SIEM system._

##### **Wazuh** ( [Download](https://wazuh.com/install/) / [Documentation](https://documentation.wazuh.com/current/index.html) ) - _Open source security platform that unifies XDR and SIEM capabilities._

## Vulnerability Scanners

##### **Nessus Essentials** ( [Download](https://www.tenable.com/products/nessus/nessus-essentials) / [Documentation](https://docs.tenable.com/Nessus.htm) ) - Proprietary vulnerability scanner developed by Tenable.

##### **OpenVAS** ( [Download](https://github.com/greenbone/openvas-scanner) / [Documentation](https://greenbone.github.io/docs/latest/) ) - _Full-featured scan engine that executes Vulnerability Tests (VTs) against target systems._

