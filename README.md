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
- [Encryption Tools](#encryption-tools)
  - [VeraCrypt](#veracrypt--download--documentation----software-for-establishing-and-maintaining-volume-encryption)
  - [Cryptsetup](#cryptsetup--download--documentation--open-source-utility-used-to-setup-disk-encryption)
- [Endpoint / Extended Detection and Response ( EDR / XDR )](#endpoint--extended-detection-and-response--edr--xdr-)
  - [OSSEC](#ossec--download--documentation----open-source-host-based-intrusion-detection-system-hids-with-edr-functions)
  - [Wazuh](#wazuh--download--documentation----open-source-security-platform-that-unifies-xdr-and-siem-capabilities)
- [Firewalls](#firewalls)
  - [IPFire](#ipfire--download--documentation----linux-distribution-hardened-to-act-as-a-dedicated-stateful-inspection-firewall)
  - [IPTables](#iptables--documentation----user-space-utility-program-that-allows-a-system-administrator-to-configure-the-ip-packet-filter-rules-of-the-linux-kernel-firewall)
    - [UFW](#ufw--documentation----provides-a-user-friendly-interface-to-modify-the-iptables-for-ubunutu)
    - [Firewalld](#firewalld--documentation----provides-a-user-friendly-interface-to-modify-the-iptables-for-centosredhat)
  - [OPNsense](#opnsense--download--documentation----easy-to-use-and-easy-to-build-freebsd-based-firewall-and-routing-platform)
  - [pfSense](#pfsense--download----customised-distribution-of-freebsd-tailored-for-use-as-a-firewall-and-router)
  - [Windows Defender Firewall](#windows-defender-firewall--documentation----host-based-firewall-that-is-included-with-the-windows_)
- [Honeytokens / Honeypots](#honeytokens--honeypots)
  - [Canarytokens](#canarytokens--download--documentation----opensource-honeytokens-for-networks-computers-clouds-and-phones)
  - [Manuka](#manuka--download--documentation----open-source-intelligence-osint-honeypot-that-monitors-reconnaissance-attempts-by-threat-actors)
  - [OpenCanary](#opencanary--download--documentation----daemon-that-runs-canary-services-which-trigger-alerts-when-used)
- [Incident Response](#incident-response)
  - [The Hive](#the-hive--download--documentation----incident-response-platform)
  - [Velociraptor](#velociraptor--download--documentation----open-source-endpoint-monitoring-digital-forensic-and-cyber-response-platform)
- [Infrastructure Deployment / Maintenance](#infrastructure-deployment--maintenance)
  - [Ansible](#ansible--download--documentation----infrastrucutre-as-code-tool-used-for-configuration-management)
  - [Oracle VM VirtualBox](#oracle-vm-virtualbox--download--documentation----virtualisation-software-used-to-create-virtual-machines)
  - [Terraform](#terraform--download--documentation----infrastructure-as-code-tool-that-lets-you-define-both-cloud-and-on-prem-resources)
  - [Vagrant](#vagrant--download--documentation----tool-for-building-and-managing-virtual-machine-environments-in-a-single-workflow)
- [Intrusion Detection / Prevention Systems (IDS / IPS)](#intrusion-detection--prevention-systems-idsips)
  - [Fail2Ban](#fail2ban--download--documentation----python-written-ips-software-framework-designed-to-prevent-brute-force-attacks)
  - [OSSEC](#ossec--download--documentation----open-source-host-based-intrusion-detection-system-hids-with-edr-functions-1)
  - [Snort](#snort--download--documentation----open-source-network-based-intrusion-prevention-system-nips)
  - [Suricata](#suricata--download--documentation----open-source-engine-with-nids-nips-and-network-monitoring-capabilities)
- [Network Analysis Tools (Network Analysers) / Monitoring ](#network-analysis-tools-network-analysers)
  - [OpenNMS Horizon](#opennms-horizon--download--documentation----open-source-network-monitoring-solution)
  - [Wireshark](#wireshark--download--documentation----network-packet-and-protocol-analyser-prsenting-captured-data-in-as-much-detail-as-possible)
  - [Zeek](#zeek--download--documentation----passive-open-source-network-traffic-analyser)
- [Network Mapping Tools](#network-mapping-tools)
  - [Angry IP Scanner](#angry-ip-scanner--download--documentation----widely-used-open-source-and-multi-platform-network-scanner)
  - [Masscan](#masscan--download--documentation----similar-to-nmap-however-operates-much-faster-and-can-scan-a-large-number-of-ports)
  - [nmap](#nmap--download--documentation----open-source-tool-for-network-exploration-and-security-auditing)
  - [zmap](#zmap--download--documentation----fast-single-packet-network-scanner-designed-for-internet-wide-network-surveys)
- [Programming / Scripting / Decarative (Database) Languages](#programming--scripting--decarative-database-languages)
  - [Bash](#bash---default-scripting-language-for-most-linux-distributions)
  - [C](#c---general-purpose-programming-language-that-provides-low-level-access-to-system-memory)
  - [Go](#golang---high-level-programming-language-designed-at-google)
  - [JavaScript](#javascript---most-popular-programming-language-for-web-pages)
  - [Powershell](#powershell---default-scripting-language-for-windows)
  - [Python](#python---clear-and-powerful-object-oriented-programming-language)
  - [Structured Query Language (SQL)](#structured-query-language-sql---language-used-to-query-sql-or-relational-databases)
- [Security Distributions (Linux)](#security-distributions-linux)
  - [Kali Linux](#kali-linux--download--documentation----_distribution-which-allows-users-to-perform-advanced-penetration-testing-and-security-auditing)
  - [ParrotOS](#parrotos--download--documentation----distribution-designed-for-security-experts-developers-and-privacy-aware-people)
  - [Security Onion](#security-onion--download--documentation----distribution-built-by-defenders-for-defenders)
- [Security Information and Event Management (SIEM)](#security-information-and-event-management-siem)
  - [OpenSearch](#opensearch--download--documentation---distributed-search-and-analytics-engine)
    - [Security Analytics for Opensearch](#security-analytics-for-opensearch--documentation----security-information-and-event-management-siem-solution-for-opensearch)
  - [Prelude OSS](#prelude-oss--download--documentation----agentless-siem-system)
  - [Wazuh](#wazuh--download--documentation----open-source-security-platform-that-unifies-xdr-and-siem-capabilities-1)
- [Security Monitoring](#security-monitoring)
  - [Elasticsearch](#elasticsearch--download--documentation----distributed-search-and-analytics-engine-component-of-elk-stack)
  - [Kibana](#kibana--download--documentation----data-visualisation-software-component-of-elk-stack)
  - [Logstash](#logstash--download--documentation----data-collection-engine-component-of-elk-stack)
  - [Suricata](#suricata--download--documentation----open-source-engine-with-nids-nips-and-network-monitoring-capabilities-1)
  - [Velociraptor](#velociraptor--download--documentation----open-source-endpoint-monitoring-digital-forensic-and-cyber-response-platform-1)
- [Threat Hunting](#threat-hunting)
  - [APT-Hunter](#apt-hunter--download--documentation----threat-hunting-tool-for-windows-event-logs)
  - [Cuckoo Sandbox](#cuckoo-sandbox--download--documentation----open-source-automated-malware-analysis-system)
  - [The Hunting ELK](#the-hunting-elk--download--documentation----open-source-threat-hunting-platform-with-advanced-analytics-capabilities)
- [Virtual Private Network (VPN)](#virtual-private-netowrk-vpn)
  - [OpenVPN](#openvpn--download--documentation----traditional-ssltls-based-virtual-private-network)
  - [Firezone](#firezone--download--documentation----open-source-platofrm-to-securely-manage-remote-access)
- [Vulnerability Scanners](#vulnerability-scanners)
  - [Nessus Essentials](#nessus-essentials--download--documentation----proprietary-vulnerability-scanner-developed-by-tenable)
  - [OpenVAS](#openvas--download--documentation----full-featured-scan-engine-that-executes-vulnerability-tests-vts-against-target-systems)
  - [Vega](#vega--download--documentation----gui-based-platform-for-testing-web-application-security)

## Encryption Tools

##### **VeraCrypt** ( [Download](https://www.veracrypt.fr/en/Downloads.html) / [Documentation](https://www.veracrypt.fr/en/Documentation.html) ) - _Software for establishing and maintaining volume encryption._

##### **Cryptsetup** ( [Download](https://gitlab.com/cryptsetup/cryptsetup) / [Documentation](https://www.veracrypt.fr/en/Documentation.html) ) _Open-source utility used to setup disk encryption._

## Endpoint / Extended Detection and Response ( EDR / XDR )

##### **OSSEC** ( [Download](https://www.ossec.net/ossec-downloads/) / [Documentation](https://www.ossec.net/docs/) ) - _Open-source Host-Based Intrusion Detection System (HIDS) with EDR functions._

##### **Wazuh** ( [Download](https://wazuh.com/install/) / [Documentation](https://documentation.wazuh.com/current/index.html) ) - _Open-source security platform that unifies XDR and SIEM capabilities._
  
## Firewalls
  
##### **IPFire** ( [Download](https://www.ipfire.org/downloads/ipfire-2.29-core187) / [Documentation](https://www.ipfire.org/docs) ) - _Linux distribution hardened to act as a dedicated stateful inspection firewall._
  
##### **IPTables** ( [Documentation](https://linux.die.net/man/8/iptables) ) - _User-space utility program that allows a system administrator to configure the IP packet filter rules of the Linux kernel firewall._
  ##### **UFW** ( [Documentation](https://help.ubuntu.com/community/UFW) ) - _Provides a user-friendly interface to modify the IPTables for Ubunutu._
  ##### **Firewalld** ( [Documentation](https://firewalld.org/documentation/) ) - _Provides a user-friendly interface to modify the IPTables for Centos/RedHat._

##### **OPNsense** ( [Download](https://opnsense.org/download/) / [Documentation](https://docs.opnsense.org/) ) - _Easy-to-use and easy-to-build FreeBSD based firewall and routing platform._

##### **pfSense** ( [Download](QwOTk.*_ga_TM99KBGXCB*MTcyNTUwNDA5OS4xLjEuMTcyNTUwNDE0NS4xNC4wLjA.) ) - _Customised distribution of FreeBSD tailored for use as a firewall and router._
    
##### **Windows Defender Firewall** ( [Documentation](https://learn.microsoft.com/en-us/windows/security/operating-system-security/network-security/windows-firewall/) ) - Host-based firewall that is included with the Windows._

## Honeytokens / Honeypots

##### **Canarytokens** ( [Download](https://github.com/thinkst/canarytokens-docker) / [Documentation](https://docs.canarytokens.org/guide/) ) - _Opensource Honeytokens for networks, computers, clouds and phones._

##### **Manuka** ( [Download](https://github.com/spaceraccoon/manuka) / [Documentation](https://github.com/spaceraccoon/manuka) ) - _Open-source intelligence (OSINT) honeypot that monitors reconnaissance attempts by threat actors._
  
##### **OpenCanary** ( [Download](#installation) / [Documentation](https://opencanary.readthedocs.io/en/latest/) ) - _Daemon that runs canary services, which trigger alerts when used._

## Incident Response

##### **The Hive** ( [Download](https://docs.strangebee.com/thehive/download/) / [Documentation](https://docs.strangebee.com/) ) - _Incident Response Platform._

##### **Velociraptor** ( [Download](https://docs.velociraptor.app/downloads/) / [Documentation](https://docs.velociraptor.app/docs/overview/) ) - _Open-source endpoint monitoring, digital forensic and cyber response platform._

## Infrastructure Deployment / Maintenance

##### **Ansible** ( [Download](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) / [Documentation](https://docs.ansible.com/users.html) ) - _Infrastrucutre as code tool used for configuration management._

##### **Oracle VM VirtualBox** ( [Download](https://www.virtualbox.org/wiki/Downloads) / [Documentation](https://www.virtualbox.org/wiki/Documentation) ) - _Virtualisation software used to create Virtual Machines._

##### **Terraform** ( [Download](https://developer.hashicorp.com/terraform/install?product_intent=terraform) / [Documentation](https://developer.hashicorp.com/terraform/docs) ) - _Infrastructure as code tool that lets you define both cloud and on-prem resources._
  
##### **Vagrant** ( [Download](https://developer.hashicorp.com/vagrant/install?product_intent=vagrant) / [Documentation](https://developer.hashicorp.com/vagrant/docs) ) - _Tool for building and managing virtual machine environments in a single workflow._

## Intrusion Detection / Prevention Systems (IDS/IPS)

##### **Fail2Ban** ( [Download](https://github.com/fail2ban/fail2ban) / [Documentation](https://github.com/fail2ban/fail2ban/tree/master/man) ) - _Python Written IPS software framework designed to prevent brute-force attacks._

##### **OSSEC** ( [Download](https://www.ossec.net/ossec-downloads/) / [Documentation](https://www.ossec.net/docs/) ) - _Open-source Host-Based Intrusion Detection System (HIDS) with EDR functions._

##### **Snort** ( [Download](https://www.snort.org/downloads) / [Documentation](https://www.snort.org/documents) ) - _Open-source Network-Based Intrusion Prevention System (NIPS)._

##### **Suricata** ( [Download](https://suricata.io/download/) / [Documentation](https://docs.suricata.io/en/latest/) ) - _Open-source engine with NIDS, NIPS and Network Monitoring capabilities._

## Network Analysis Tools (Network Analysers) / Monitoring

##### **OpenNMS Horizon** ( [Download](https://github.com/OpenNMS/opennms) / [Documentation](https://docs.opennms.com/horizon/33/index.html) ) - _Open-source network monitoring solution_

##### **Wireshark** ( [Download](https://www.wireshark.org/download.html) / [Documentation](https://www.wireshark.org/docs/wsug_html_chunked/index.html) ) - _Network packet and protocol analyser, prsenting captured data in as much detail as possible._

##### **Zeek** ( [Download](https://zeek.org/get-zeek/) / [Documentation](https://docs.zeek.org/en/master/index.html) ) - _Passive, Open-Source network traffic analyser._

## Network Mapping Tools

##### **Angry IP Scanner** ( [Download](#google_vignette) ) - _Widely-used open-source and multi-platform network scanner._

##### **Masscan** ( [Download](#masscan) / [Documentation](https://www.kali.org/tools/masscan/) ) - _Similar to nmap however operates much faster and can scan a large number of ports._

##### **nmap** ( [Download](https://nmap.org/download) / [Documentation](https://nmap.org/docs.html) ) - _Open-source tool for network exploration and security auditing._

##### **zmap** ( [Download](https://github.com/zmap/zmap?tab=readme-ov-file) / [Documentation](https://github.com/zmap/zmap/wiki/Getting-Started-Guide) ) - _Fast single packet network scanner designed for Internet-wide network surveys._

## Programming / Scripting / Decarative (Database) Languages

##### **[Bash](https://www.gnu.org/software/bash/)** - _Default scripting language for most Linux distributions._

##### **[C](https://devdocs.io/c/)** - _General-purpose programming language that provides low-level access to system memory._

##### **[GoLang](https://go.dev/doc/)** - _High-level programming language designed at Google._

##### **[JavaScript](https://devdocs.io/javascript/)** - _Most popular programming language for Web pages._

##### **[Powershell](https://learn.microsoft.com/en-us/powershell/)** - _Default scripting language for Windows._

##### **[Python](https://docs.python.org/3/)** - _Clear and powerful object-oriented programming language._

##### **[Structured Query Language (SQL)](https://dev.mysql.com/doc/)** - _Language used to query SQL or “relational” databases._

> I have only provided the links to the official documentation. Many of these langauges are already pre-installed on distributions or can be easily accessed either by installing packages or installing an IDE like VS Code or PyCharm. There is also a plethora of free and accessible training material for these languages. Find a method that suits your learning style.

## Security Distributions (Linux)

##### **Kali Linux** ( [Download](#kali-platforms) / [Documentation](https://www.kali.org/docs/) ) - _Distribution which allows users to perform advanced penetration testing and security auditing._

##### **ParrotOS** ( [Download](https://parrotsec.org/download/) / [Documentation](https://parrotsec.org/docs/) ) - _Distribution designed for security experts, developers and privacy aware people._

##### **Security Onion** ( [Download]() / [Documentation](https://docs.securityonion.net/en/2.4/) ) - _Distribution built by defenders for defenders._

## Security Information and Event Management (SIEM)

##### **OpenSearch** ( [Download](https://opensearch.org/downloads.html) / [Documentation](https://opensearch.org/docs/latest/)) - _Distributed search and analytics engine._

##### **Security Analytics for OpenSearch** ( [Documentation](https://github.com/opensearch-project/security-analytics/tree/main) ) - _Security Information and Event Management (SIEM) solution for OpenSearch._

##### **Prelude OSS** ( [Download](https://www.prelude-siem.org/projects/prelude/files) / [Documentation](https://www.prelude-siem.org/projects/prelude/wiki) ) - _Agentless SIEM system._

##### **Wazuh** ( [Download](https://wazuh.com/install/) / [Documentation](https://documentation.wazuh.com/current/index.html) ) - _Open-source security platform that unifies XDR and SIEM capabilities._

## Security Monitoring

##### **Elasticsearch** ( [Download](https://www.elastic.co/downloads/elasticsearch) / [Documentation](https://www.elastic.co/guide/en/elasticsearch/reference/8.15/index.html) ) - _Distributed search and analytics engine. Component of ELK Stack_

##### **Kibana** ( [Download](https://www.elastic.co/downloads/kibana) / [Documentation](https://www.elastic.co/guide/en/kibana/current/index.html) ) - _Data visualisation software. Component of ELK Stack._

##### **Logstash** ( [Download](https://www.elastic.co/downloads/logstash) / [Documentation](https://www.elastic.co/guide/en/logstash/current/index.html) ) - _Data collection engine. Component of ELK Stack._

##### **Suricata** ( [Download](https://suricata.io/download/) / [Documentation](https://docs.suricata.io/en/latest/) ) - _Open-source engine with NIDS, NIPS and Network Monitoring capabilities._

##### **Velociraptor** ( [Download](https://docs.velociraptor.app/downloads/) / [Documentation](https://docs.velociraptor.app/docs/overview/) ) - _Open-source endpoint monitoring, digital forensic and cyber response platform._

## Threat Hunting

##### **APT-Hunter** ( [Download](https://github.com/ahmedkhlief/APT-Hunter) / [Documentation](https://shells.systems/introducing-apt-hunter-threat-hunting-tool-via-windows-event-log/) ) - _Threat hunting tool for Windows event logs._

##### **Cuckoo Sandbox** ( [Download](https://cuckoosandbox.org/) / [Documentation](https://cuckoo.sh/docs/) ) - _Open-source automated malware analysis system._

##### **The Hunting ELK** ( [Download](https://thehelk.com/installation.html) / [Documentation](https://thehelk.com/intro.html) ) - _Open-source Threat Hunting platform with advanced analytics capabilities._

## Virtual Private Netowrk (VPN)

##### **OpenVPN** ( [Download](#documentation) ) - _Traditional SSL/TLS-based virtual private network._

##### **Firezone** ( [Download](https://www.firezone.dev/kb/client-apps) / [Documentation](https://www.firezone.dev/kb) ) - _Open-source platform to securely manage remote access_

## Vulnerability Scanners

##### **Nessus Essentials** ( [Download](https://www.tenable.com/products/nessus/nessus-essentials) / [Documentation](https://docs.tenable.com/Nessus.htm) ) - _Proprietary vulnerability scanner developed by Tenable._

##### **OpenVAS** ( [Download](https://github.com/greenbone/openvas-scanner) / [Documentation](https://greenbone.github.io/docs/latest/) ) - _Full-featured scan engine that executes Vulnerability Tests (VTs) against target systems._

##### **Vega** ( [Download](https://subgraph.com/vega/download/index.en.html) / [Documentation](https://subgraph.com/vega/documentation/index.en.html) ) - _GUI based platform for testing web application security._

