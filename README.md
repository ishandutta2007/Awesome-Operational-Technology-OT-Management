# Awesome-Operational-Technology-OT-Management

# Top Operational Technology (OT) Management Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on OT Asset Visibility, Industrial Cybersecurity & Cyber-Physical Systems Protection*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Operational Technology (OT) Management**. These tools enable industrial and critical infrastructure organizations to discover, monitor, and secure OT assets—PLCs, HMIs, RTUs, industrial control systems (ICS), and connected cyber-physical systems—bridging the gap between IT and OT environments while protecting production uptime and safety.

**Examples** include ServiceNow Operational Technology Management, Claroty, Nozomi Networks, Dragos, Forescout Technologies, Armis, Tenable OT Security, SCADAfence, Cisco Cyber Vision, TXOne Networks, and Microsoft Defender for IoT (the category leaders).

**Open-source emphasis**: This section is expanded with active projects for self-hosted OT asset management, ICS security monitoring, and industrial network visibility—ideal for plant engineers, ICS security teams, and organizations building sovereign OT infrastructure without per-asset or per-site licensing lock-in.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[ServiceNow Operational Technology Management](https://www.servicenow.com/)**  
  Enterprise OT management on the Now Platform with a unified workspace for industrial and hardware assets, firmware management with content normalization, OT incident/change/vulnerability response workflows, and IT/OT CMDB convergence; Yokohama release adds firmware lifecycle automation and the Zurich release expands OT visibility .

- **[Claroty](https://claroty.com/)**  
  Cyber-physical systems protection platform with agentless OT asset discovery, real-time vulnerability scoring, and risk remediation tracking; xDome replaces spreadsheet-based inventories with automated always-up-to-date asset visibility across distributed sites, integrating with existing tools like SolarWinds and Cisco DNA .

- **[Nozomi Networks](https://www.nozominetworks.com/)**  
  AI-powered OT and IoT security platform with Vantage IQ AI assistant for threat investigation and vulnerability prioritization, passive network sensors for agentless discovery, multi-factor risk scoring at asset/zone/site/enterprise levels, and OT-specific threat intelligence from Nozomi Networks Labs .

- **[Dragos](https://www.dragos.com/)**  
  OT cybersecurity platform named a Leader in the 2026 Gartner Magic Quadrant for CPS Protection Platforms; features 600+ ICS protocol support, OT-corrected CVSS scoring with "Now, Next, Never" prioritization, four detection types enriched by civilian OT threat intelligence, and Neighborhood Keeper for collective defense .

- **[Forescout Technologies](https://www.forescout.com/)**  
  Cyber-physical protection platform (CPS PP) with continuous asset discovery, multifactor risk assessment, network segmentation, and automated enforcement across IT, OT, IoT, and IoMT environments; Vistaro platform uses agentic AI and Vedere Labs threat intelligence for Universal Zero Trust Network Access .

- **[Armis](https://www.armis.com/)**  
  Agentless OT/IoT security platform with on-premises deployment for air-gapped environments, Attack Path Mapping for proactive defense, Digital Twins for simulating system behavior, and Secure Remote Access with zero-trust controls .

- **[Tenable OT Security](https://www.tenable.com/)**  
  ICS security platform with 360-degree visibility across converged IT/OT attack surfaces, active querying using native ICS protocols to identify silent devices, risk-based vulnerability management with predictive prioritization, and configuration change tracking with "last known good state" snapshots .

- **[SCADAfence](https://scadafence.com/)**  
  OT and IoT security platform (acquired by Honeywell) offering network monitoring, asset discovery, governance, remote access, and IoT device security for large-scale industrial networks; being integrated into Honeywell Forge Cybersecurity+ suite .

- **[Cisco Cyber Vision](https://www.cisco.com/)**  
  OT security platform with active discovery probe capability to identify silent devices like PLCs, 100+ industrial protocol support, FIPS-compliant release option, and integration with Cisco's broader security and networking portfolio .

- **[TXOne Networks](https://www.txone.com/)**  
  Operations-first OT security portfolio with four coordinated approaches: Element (entry point validation for air-gapped equipment), Stellar (OT-native endpoint protection from Windows 2000 through Windows 11), Edge (inline network protection with virtual patching), and Sennin (enterprise orchestration console) .

- **[Microsoft Defender for IoT](https://azure.microsoft.com/en-us/products/iot-defender)**  
  Agentless network-layer monitoring for OT/IoT environments with specialized protocol identification, machine learning-based risk assessment, integration with Microsoft Sentinel and third-party SIEM/SOAR/XDR tools, and deployment options for cloud-connected or fully on-premises sensors .

## Open-Source GitHub Projects

- **[Industrace](https://github.com/industrace/industrace)**  
  Open-source CMDB purpose-built for ICS and OT environments (AGPL-3.0); maps assets, visualizes networks, and tracks changes with demo data covering PLCs, HMIs, robots, switches, and sensors; includes distributed network probe for discovery, RBAC, SSO, REST API, and IEC 62443 scoping; Docker-deployable for controlled pilot deployments .

### Additional Strong Open-Source Options

- **Suricata + ELK Stack** — Open-source network intrusion detection paired with Elasticsearch/Logstash/Kibana for OT traffic monitoring and alerting; research demonstrates successful detection of S7 PLC attacks with real-time dashboard visualization and push notifications .
- **Snap7** — Open-source Siemens S7 PLC communication library (client/server); useful for security testing and building custom OT protocol monitors, though it lacks built-in security controls and should be used responsibly in authorized assessments only .
- **OpenSCAP** — Security compliance scanning framework with profiles applicable to industrial control system hardening, including CIS benchmarks for OT-adjacent systems.
- **Zeek** — Network security monitor with protocol analyzers for industrial protocols (Modbus, DNP3, S7comm via packages); complements Suricata for deep OT network visibility.

**Frameworks for building custom systems**: Combine **Industrace** for OT asset inventory and CMDB, **Suricata** with **ELK** or **Zeek** for ICS intrusion detection and traffic analysis, and **Snap7** for protocol-level monitoring and testing in a self-hosted OT visibility stack; note that full OT security platforms require commercial threat intelligence feeds and protocol expertise that open-source tools alone cannot fully replace.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- OT management platforms handling industrial control data must comply with applicable safety regulations, industry standards (IEC 62443, NIST CSF), and organizational security policies; OT environments prioritize availability and safety over confidentiality.
- Self-hosted open-source solutions for OT security are significantly limited compared to commercial platforms—Industrace provides asset inventory but lacks the threat intelligence, protocol depth, and vendor support of Claroty, Nozomi, or Dragos; open-source IDS (Suricata, Zeek) requires substantial OT protocol tuning and SOC expertise.
- Verify license terms for commercial use; Industrace uses AGPL-3.0.

---

**Made for OT security engineers, plant operations managers, ICS asset owners, and critical infrastructure defenders.**  
Let's make operational technology management more open, visible, and resilient.
