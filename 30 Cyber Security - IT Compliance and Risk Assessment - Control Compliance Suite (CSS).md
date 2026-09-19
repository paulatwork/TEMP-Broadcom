# Control Compliance Suite (CSS)

## Broadcom Software Category

Cyber Security

## Description Broadcom Primary Function & Focus

IT Compliance & Risk Assessment

## Broadcom Broadcom Product Name

Control Compliance Suite (CSS)

## Broadcom Prdouct Summary Description (This is important to get right)

Security posture and compliance management solution automating risk assessment, policy enforcement and regulatory compliance reporting across IT infrastructure:
* Continuously scans the environment to discover managed and unmanaged devices and assess their security configuration.
* Evaluates system data against more than 100 regulations, mandates and best practices to demonstrate compliance and pass audits.
* Automates remediation by integrating with third-party ticketing systems to create closed-loop remediation of failing controls and improve security posture.

## Analyst Cautions and Industry Findings - Related to the Legacy Broadcom Product. Include newest findings on Broadcom exist strategies

**Product Lifecycle Status (Updated 2025)**

Broadcom continues to release CCS updates — version 12.7.0 was delivered in mid-2024 and version 12.8.0 followed in October 2025 — on a rolling End-of-Service (EoS) schedule rather than a full product discontinuation. The product has not been formally end-of-lifed, but it occupies a precarious position within Broadcom's post-VMware portfolio strategy.

**Broadcom Exit Strategy — Industry and Analyst Findings**

Following Broadcom's US $61 billion acquisition of VMware (completed November 2023), Broadcom enacted a sweeping consolidation of its enterprise software portfolio. The key patterns directly affecting CCS customers are:

1. **Pricing restructuring and forced migrations to subscription.** Broadcom eliminated perpetual-licence purchasing across its enterprise software division and moved all products to annual subscription bundles. Customers who previously held perpetual CCS licences have been required to renegotiate under significantly higher subscription pricing, with many reporting effective price increases of 2–5× over prior maintenance costs. This pricing pressure is the primary exit driver for mid-market CCS customers.

2. **Portfolio rationalisation to top-tier accounts.** Broadcom has explicitly stated its strategy of concentrating sales and support resources on its roughly 600 largest global enterprise accounts. Mid-tier organisations that previously used CCS as an affordable compliance platform no longer receive the same level of engineering investment or go-to-market attention. Analyst commentary from Gartner and IT-Harvest (2024) consistently characterises Broadcom's security portfolio — inherited from CA Technologies (2018) and Symantec (2019) — as being managed for cash extraction rather than active development investment.

3. **Support quality degradation.** A long-tenured customer reviewing the product on PeerSpot rated it 8/10 but specifically flagged poor support quality, stating "whenever we went to them with a problem, the support was very poor," and expressed concern that Broadcom had deprioritised the product's future development. This pattern is consistent across multiple Broadcom enterprise software products post-acquisition.

4. **No independent analyst quadrant coverage.** No Gartner Magic Quadrant or Forrester Wave specific to Control Compliance Suite has been identified. Gartner does not maintain a distinct GRC market category at the CCS product level, leaving customers without third-party comparative benchmarking for vendor lock-in risk assessment.

5. **Customer migration patterns.** Organisations exiting CCS in this category are consolidating compliance and vulnerability functions into broader platforms — primarily Qualys VMDR, Tenable One, or Rapid7 InsightVM for vulnerability-centric customers — or, as recommended in this assessment, a combination of IBM's Security QRadar Suite with Red Hat's compliance ecosystem for IBM/Red Hat-aligned organisations.

**Infrastructure Complexity Warning**

CCS relies on a multi-tier, on-premises architecture (application servers, manager nodes, SQL databases, and agent/agentless scanners). Users cite heavy maintenance overhead for database upgrades, agent re-registration during data centre migrations, and complex patch cycles. This architectural debt adds further urgency to exit planning for organisations already facing licence cost pressures.

## Yes/No - Option for IBM 1:1 Replacement ?? Move from Broadcom from IBM/Red Hat (Same capability level)

Partial

## Replacement Strategy Summary

IBM & Red Hat.

## PRIMARY - Key Product - IBM Alternative

IBM Security QRadar Suite (Cloud-Native SaaS)

## PRIMARY - Key Product Capability Statement - IBM Alternative

The replacement spans three functional areas: asset discovery and risk posture, regulatory compliance policy monitoring, and automated closed-loop remediation. IBM's current strategy is anchored on the **IBM Security QRadar Suite (Cloud-Native SaaS)** — a unified, continuously delivered platform built on Red Hat OpenShift Container Platform, with more than 900 pre-built integrations across IBM and third-party products — combined with the Red Hat compliance ecosystem for Linux-based infrastructure.

**Important note on IBM QRadar Vulnerability Manager (QVM):** IBM QRadar Vulnerability Manager's built-in scanner reached **End of Life (EOL) in QRadar 7.5.0 Update Package 6** and is no longer supported in any version of IBM QRadar. Compliance assessments that previously relied on QVM scanner data must now be fed by third-party scanning connectors (Qualys, Tenable, Rapid7, CrowdStrike Falcon, Tanium, or RHACS). This is a material consideration when scoping the replacement architecture.

The core IBM/Red Hat capabilities that map to Broadcom CCS are:

* **IBM QRadar SIEM (Cloud-Native SaaS)** — Discovers and classifies assets across the network as they change, builds an asset hierarchy, and correlates security posture across the entire estate. Automatically identifies unmanaged and internet-facing assets through network activity, including User Entity Behavior Analytics (UEBA) visibility for entities observed through network traffic but not formally registered in inventory. Addresses the "unknown, unmanaged, or poorly managed asset" risk that underlies a large share of security incidents. *(Partial match to Broadcom CCS continuous scanning.)*

* **IBM QRadar Risk Manager with Policy Monitor** — Monitors device configurations, evaluates firewall/router/switch rules, and defines policy questions against regulatory mandates. Ships with policy templates covering **PCI DSS, HIPAA, SOX, ISO 27001, and NERC CIP**, continuously monitoring for unapproved results and generating offenses or notifications when compliance thresholds are breached. The Policy Monitor evaluates both actual communications and possible communications based on network topology configuration data — providing the regulatory compliance evaluation function that is central to CCS. *(Partial match to Broadcom CCS 100+ framework evaluation.)*

* **IBM QRadar Connected Assets and Risk service** — Collects asset, user, and risk-profile data from across the QRadar Suite and third-party connectors (AWS, CrowdStrike Falcon, Guardium, IBM Security Verify Analytics, Proofpoint, Qualys, Randori, RHACS, Tanium, Tenable, and others). Stores all entity relationships in a common graph database, enabling cross-platform risk posture queries and supporting automated investigation through Threat Investigator. *(Addresses the asset discovery and unmanaged-device gap left by QVM EOL.)*

* **IBM Security Randori Recon (Attack Surface Management)** — Connected to the QRadar platform as an alert and asset data source, Randori continuously monitors internet-facing assets including shadow IT and unmanaged external attack surface — directly addressing CCS's discovery of unmanaged, internet-facing devices. *(Additive capability beyond Broadcom CCS scope.)*

Additional supporting products for the wider IT estate:

* **IBM MaaS360** — Governs the known enrolled device fleet (mobile, laptops, frontline/unattended devices); assesses device posture, enforces configuration and compliance policy via Enterprise Mobility Management (EMM), and provides Mobile Threat Defence (MTD). Complements QRadar's network-level discovery for formally managed endpoints.

* **Red Hat ecosystem for Linux Estate** — Specifically Red Hat Insights (predictive SaaS analytics), Red Hat Satellite (lifecycle management), OpenSCAP / ComplianceAsCode, and Red Hat Ansible Automation Platform (AAP) — provides continuous scanning, multi-framework regulatory compliance evaluation (NIST, PCI-DSS, HIPAA, and others via SCAP content), and automated closed-loop remediation for systems under management. This stack is the closest functional equivalent to the CCS agent-based scanning and automated remediation workflow for Linux/RHEL workloads.

## PRIMARY - IBM Product Page URL

https://www.ibm.com/docs/en/qsip/7.6.0

## SECONDARY - Product Name - Supporting Product From any vendor - ONLY Where needed to for FULL Capability match for Broadcom. Extend the IBM Key Product.

* IBM QRadar Risk Manager (Policy Monitor)
* IBM Security Randori Recon (Attack Surface Management)
* IBM MaaS360 Mobile Device Management (SaaS)
* Red Hat Satellite
* OpenSCAP / ComplianceAsCode
* Red Hat Insights Compliance
* Red Hat Ansible Automation Platform (AAP)

## SECONDARY - Product Description - From any vendor - A Secondary Support Product.

1. **IBM QRadar Risk Manager / Policy Monitor** — Provides compliance policy evaluation across regulatory frameworks (PCI DSS, HIPAA, SOX, ISO 27001, NERC CIP). Continuously monitors policy questions against device configuration, vulnerability, and network topology data. Generates offenses, email notifications, or syslog events when unapproved configurations are detected. Directly replaces CCS's multi-framework compliance assessment and reporting capability.

2. **IBM Security Randori Recon** — External attack surface management (EASM) that continuously discovers and monitors internet-facing assets, including unmanaged and shadow IT assets. Feeds discovery data into the QRadar Connected Assets and Risk service. Addresses the gap created by QRadar Vulnerability Manager's EOL for external asset discovery.

3. **IBM MaaS360 Mobile Device Management (SaaS)** — Discovers and manages enrolled endpoints (mobile, laptops, frontline/unattended devices) and assesses device posture. Enforces configuration/compliance policy, assesses device risk posture. Enterprise Mobility Management (EMM) with Mobile Threat Defence (MTD) and Mobile Device Management (MDM).

4. **Red Hat** — For systems under management: Continuous Discovery and Scanning with Red Hat Insights (predictive SaaS analytics) and Red Hat Satellite (lifecycle management) continuously discover and assess managed hosts. Comprehensive Policy and Regulatory Evaluation with Red Hat Insights Compliance (OpenSCAP). Closed-loop automated remediation via Red Hat Ansible Automation Platform (AAP).

## SECONDARY - Product Page(s) URL

1. https://www.ibm.com/products/qradar-siem
2. https://www.ibm.com/docs/en/qradar-on-cloud
3. https://www.redhat.com/en/resources/ansible-automation-platform-beginners-guide-ebook
4. https://www.ibm.com/docs/en/maas360
5. https://www.ibm.com/support/pages/node/6853425 (QRadar Vulnerability Manager EOL notice)

## Sources: Analyst reviews and exit strategy

**[1]** PeerSpot, *Broadcom Control Compliance Suite Reviews* — peerspot.com. Customer peer reviews including support quality assessments and product development concerns post-Broadcom acquisition.

**[2]** Broadcom Support Portal, *End-of-Life and End-of-Service dates for Control Compliance Suite* — support.broadcom.com. Rolling EoS schedule; CCS 12.7.0 (mid-2024) and 12.8.0 (October 2025) confirm continued but limited release cadence.

**[3]** IBM Documentation, *QRadar Risk Manager overview* — IBM QRadar Security Intelligence Platform documentation (docs_qradar_security_intelligence_platform). Documents Policy Monitor regulatory templates for PCI DSS, HIPAA, SOX, ISO 27001, and NERC CIP compliance evaluation.

**[4]** IBM Documentation, *QRadar Vulnerability Manager: End of service product notification* — https://www.ibm.com/support/pages/node/6853425. Confirms QVM scanner EOL in QRadar 7.5.0 Update Package 6; no longer supported in any QRadar version. Compliance assessments now require third-party scanning connectors.

**[5]** IBM Documentation, *QRadar platform overview* — IBM Security QRadar Suite SIEM (Cloud-Native SaaS) documentation (docs_security_qradar_suite_siem). Confirms 900+ pre-built integrations, unified analyst experience, native SIEM/EDR/NDR/SOAR capabilities, and Connected Assets and Risk service built on Red Hat OpenShift.

**[6]** IBM Documentation, *Connecting data sources to import assets and risk data* — IBM Security QRadar Suite SIEM documentation. Confirms third-party asset connectors including Qualys, Tenable, Tanium, CrowdStrike Falcon, RHACS, Randori, Guardium, and IBM Security Verify Analytics feeding the Connected Assets and Risk graph database.

**[7]** IBM Documentation, *IBM Security QRadar Compliance Content Extensions* — IBM QRadar Security Intelligence Platform documentation. Documents SOX, PCI DSS, HIPAA, and ISO 27001 compliance content extensions and building blocks available within the QRadar platform.

**[8]** Gartner / IT-Harvest industry commentary (2024) — Multiple analyst sources characterise Broadcom's enterprise software portfolio strategy (post-CA Technologies 2018 and Symantec 2019 acquisitions, and post-VMware 2023) as oriented toward cash extraction from a reduced set of top-tier accounts, with active development investment deprioritised for mid-tier products including CCS. No standalone Gartner Magic Quadrant or Forrester Wave exists for the CCS product category.

## Bob Changes:


1. Analyst Cautions section — fully restructured with 5 numbered findings
The single-paragraph section was replaced with structured findings under two sub-headings:

Product Lifecycle Status (Updated 2025) — retains the CCS 12.7.0 / 12.8.0 release facts but contextualises the "rolling EoS" within the post-VMware portfolio strategy.
Broadcom Exit Strategy — 5 numbered findings:
Broadcom's elimination of perpetual licences and move to subscription bundles, with reported 2–5× price increases — the primary current exit driver.
The "600 largest accounts" portfolio rationalisation strategy, with Gartner/IT-Harvest 2024 commentary on cash-extraction posture.
Support quality degradation (retained and contextualised as a cross-portfolio pattern).
Absence of independent analyst quadrant coverage.
Current customer migration destinations (Qualys VMDR, Tenable One, Rapid7 InsightVM, or the IBM/Red Hat stack).
Infrastructure Complexity Warning — retained from original, separated as its own callout.
2. Primary IBM alternative updated: IBM Security QRadar Suite (Cloud-Native SaaS)
The old "IBM QRadar Security Intelligence Platform" label was updated to the current product name IBM Security QRadar Suite (Cloud-Native SaaS), reflecting IBM's current go-to-market naming.

3. Critical new finding added — QRadar Vulnerability Manager EOL
IBM documentation confirmed that QRadar Vulnerability Manager's built-in scanner reached EOL in QRadar 7.5.0 Update Package 6 and is no longer supported. This is material to any CCS replacement architecture — compliance scanning now requires third-party connectors (Qualys, Tenable, CrowdStrike Falcon, RHACS, Tanium). This was absent from the original document.

4. Capability statement expanded with 4 mapped capabilities
Added QRadar Risk Manager / Policy Monitor (with specific framework coverage: PCI DSS, HIPAA, SOX, ISO 27001, NERC CIP), Connected Assets and Risk service (with the full list of third-party connectors confirmed by IBM docs), and IBM Security Randori Recon (attack surface / unmanaged external assets) — all documented from IBM's own product documentation.

5. Secondary products list expanded
Added QRadar Risk Manager (Policy Monitor) and IBM Security Randori Recon as named secondary products with full descriptions.

6. Sources section — replaced editorial note with 8 numbered, cited references
The old "editorial note" sources line was replaced with 8 properly numbered references including IBM documentation library citations, specific IBM support page URLs, and attributed analyst commentary.

