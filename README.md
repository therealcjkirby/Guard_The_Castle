# <ins> *_Guard The Castle - Home Labs_* </ins>

<p align="center">
  <img width="900" height="500" src="https://pixeljoint.com/files/icons/full/addeddragonreflection.gif">
</p>

## <ins> Objective </ins>
Guard The Castle aims to provide a starting point for aspiring Blue Team Cybersecurity Professionals looking to expand their knowledge through the use of home labs and practical learning. Guard the Castle was structured with the intention to be accessible to anyone with a working computer, with that in mind only free and/or open-source tools are mentioned. 
> :grey_exclamation: Disclaimer, some of the tools mentioned have a paid version that offers a more comprehensive solution. For the purpose of this project it is NOT necessary to use the paid versions, however some offer free trial periods to test out the paid versions. I would suggest establishing a strong understanding of the free version before you use these trials to get the most out of it.

> :information_source: Links to download the tools used and the related documentation will also be provided.

## <ins> Tools / Software </ins>

<details open>

<summary>Infrastructure Building / Maintenance</summary>
<br/>

- *Oracle VM VirtualBox* ( [Download](https://www.virtualbox.org/wiki/Downloads) / [Documentation](https://www.virtualbox.org/wiki/Documentation) ) - _Virtualisation software used to create Virtual Machines_
  
- *Vagrant* ( [Download](https://developer.hashicorp.com/vagrant/install?product_intent=vagrant) / [Documentation](https://developer.hashicorp.com/vagrant/docs) ) - _Tool for building and managing virtual machine environments in a single workflow._
  
- *Ansible* ( [Download](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) / [Documentation](https://docs.ansible.com/users.html) ) - _Infrastrucutre as code tool used for configuration management_

- *Terraform* ( [Download](https://developer.hashicorp.com/terraform/install?product_intent=terraform) / [Documentation](https://developer.hashicorp.com/terraform/docs) ) - _Infrastructure as code tool that lets you define both cloud and on-prem resources._
  
</details>
<br/>
<details open>

<summary>Firewalls</summary>
<br/>

- *pfSense* ( [Download](https://www.pfsense.org/download/) / [Documentation](https://docs.netgate.com/pfsense/en/latest/?_gl=1*jffkzm*_gcl_au*MjEyMzA0MTk5LjE3MjU1MDQwOTk.*_ga*OTkxOTIyMDk4LjE3MjU1MDQwOTk.*_ga_TM99KBGXCB*MTcyNTUwNDA5OS4xLjEuMTcyNTUwNDE0NS4xNC4wLjA.) ) - _Customised distribution of FreeBSD tailored for use as a firewall and router._
  
- *IPFire* ( [Download](https://www.ipfire.org/downloads/ipfire-2.29-core187) / [Documentation](https://www.ipfire.org/docs) ) - _Linux distribution hardened to act as a dedicated stateful inspection firewall._
  
- OPNsense ( [Download](https://opnsense.org/download/) / [Documentation](https://docs.opnsense.org/) ) - _Easy-to-use and easy-to-build FreeBSD based firewall and routing platform._
  
- *IPTables* ( [Documentation](https://linux.die.net/man/8/iptables) ) - _User-space utility program that allows a system administrator to configure the IP packet filter rules of the Linux kernel firewall._
  - UFW ( [Documentation](https://help.ubuntu.com/community/UFW) ) - _Provides a user-friendly interface to modify the IPTables for Ubunutu._
  - Firewalld ( [Documentation](https://firewalld.org/documentation/) ) - _Provides a user-friendly interface to modify the IPTables for Centos/RedHat._
    
- Windows Defender Firewall ( [Documentation](https://learn.microsoft.com/en-us/windows/security/operating-system-security/network-security/windows-firewall/) ) - Host-based firewall that is included with the Windows._
</details>
<br/>
<details open>

<summary>Security Information and Event Management (SIEM)</summary>
<br/>

- *OpenSearch* ( [Download](https://opensearch.org/downloads.html) / [Documentation](https://opensearch.org/docs/latest/)) - _Distributed search and analytics engine._
  - *Security Analytics for OpenSearch* ( [Documentation](https://github.com/opensearch-project/security-analytics/tree/main) ) - _Security Information and Event Management (SIEM) solution for OpenSearch._

- *Wazuh* ( [Download](https://wazuh.com/install/) / [Documentation](https://documentation.wazuh.com/current/index.html) ) - _Free and open source security platform that unifies XDR and SIEM capabilities._

- *Prelude OSS* ( [Download](https://www.prelude-siem.org/projects/prelude/files) / [Documentation](https://www.prelude-siem.org/projects/prelude/wiki) ) - _Agentless SIEM system._

</details>
<br/>
<details open>

<summary>Vulnerability Scanners</summary>
<br/>

- *OpenVAS* ( [Download](https://github.com/greenbone/openvas-scanner) / [Documentation](https://greenbone.github.io/docs/latest/) ) - _Full-featured scan engine that executes Vulnerability Tests (VTs) against target systems._
- *Nessus Essentials* ( [Download](https://www.tenable.com/products/nessus/nessus-essentials) / [Documentation](https://docs.tenable.com/Nessus.htm) ) - Proprietary vulnerability scanner developed by Tenable.


</details>
<br/>
<details open>

<summary>Intrusion Detection / Prevention Systems</summary>
<br/>

- *OSSEC* ( [Download](https://www.ossec.net/ossec-downloads/) / [Documentation](https://www.ossec.net/docs/) ) - _Open Source Host-Based Intrusion Detection System (HIDS)._

- *Snort* ( [Download](https://www.snort.org/downloads) / [Documentation](https://www.snort.org/documents) ) - _Open source Network-Based Intrusion Prevention System (NIPS)._

</details>
<br/>
<details open>

<summary>Network Analysis Tools (Network Analysers)</summary>
<br/>

- *Wireshark* ( [Download](https://www.wireshark.org/download.html) / [Documentation](https://www.wireshark.org/docs/wsug_html_chunked/index.html) ) - _Network packet and protocol analyser, prsenting captured data in as much detail as possible._

- *Zeek* ( [Download](https://zeek.org/get-zeek/) / [Documentation](https://docs.zeek.org/en/master/index.html) ) - _Passive, Open-Source network traffic analyser._

</details>
<br/>
<details open>

<summary>Network Mapping Tools</summary>
<br/>

- *nmap* ( [Download](https://nmap.org/download) / [Documentation](https://nmap.org/docs.html) ) - _Open source tool for network exploration and security auditing._

- *Masscan* ( [Download](https://www.kali.org/tools/masscan/#masscan) / [Documentation](https://www.kali.org/tools/masscan/) ) - _Similar to nmap however operates much faster and can scan a large number of ports._

- *Angry IP Scanner* ( [Download](https://angryip.org/download/#windows) / [Documentation](https://angryip.org/documentation/#google_vignette) ) - _Widely-used open-source and multi-platform network scanner._

- *zmap* ( [Download](https://github.com/zmap/zmap?tab=readme-ov-file) / [Documentation](https://github.com/zmap/zmap/wiki/Getting-Started-Guide) ) - _Fast single packet network scanner designed for Internet-wide network surveys._

</details>
