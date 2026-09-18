# VMware vSAN

## Broadcom Software Category

VMware

## Description Broadcom Primary Function & Focus

Software-Defined Storage

## Broadcom Broadcom Product Name

VMware vSAN

## Broadcom Prdouct Summary Description (This is important to get right)

VMware vSAN is a hyperconverged, software-defined storage layer that pools local server disks across an ESXi cluster into shared, resilient datastores, eliminating the need for a separate SAN/NAS array. It now ships only as a capacity entitlement bundled within VCF or VVF licensing rather than as a standalone product.

## Analyst Cautions and Industry Findings - Related to the Legacy Broadcom Product. Include newest findings on Broadcom exist strategies

Standalone vSAN licensing was discontinued in 2023; capacity is now bundled per physical core (0.25 TiB per core under VVF, confirmed by Broadcom TechDocs), with additional capacity requiring supplementary licensing or a step-up to full VCF. Storage-dense clusters, common in environments running large databases or backup repositories, can incur materially higher licensing costs than under the previous per-CPU or per-terabyte models, a pattern documented across multiple VMware licensing analyses published during 2025 and 2026. Industry commentary on VMware exit strategies generally treats storage as more tractable to replatform than networking, since data can be migrated using standard storage migration tooling; however, replicating vSAN's tight integration with vSphere HA/DRS requires a genuinely hyperconverged replacement rather than a bolt-on array. Red Hat OpenShift Data Foundation, built on Ceph, and Nutanix AOS are realistic alternatives, though OpenShift Data Foundation is primarily oriented toward container-native and OpenShift Virtualization workloads rather than general-purpose VM storage, so a mixed VM and container estate may require complementary tooling such as IBM Storage Fusion for VM-centric use cases.

Sources: Broadcom TechDocs, 'VMware vSphere Foundation Capacity License for vSAN'; general VMware/Broadcom licensing analyses published by Network World and CIO Dive through 2025-2026 covering per-core vSAN capacity bundling.

## Yes/No - Option for IBM 1:1 Replacement ?? Move from Broadcom from IBM/Red Hat (Same capability level)

Yes

## Replacement Strategy Summary

Red Hat + IBM

## PRIMARY - Key Product - IBM Alternative

OpenShift Data Foundation + IBM Fusion

## PRIMARY - Key Product Capability Statement - IBM Alternative

(not provided)

## PRIMARY - IBM Product Page URL

https://www.redhat.com/en/resources/add-capabilities-enterprise-deployments-datasheet

## SECONDARY - Product Name - Supporting Product From any vendor - ONLY Where needed to for FULL Capability match for Broadcom. Extend the IBM Key Product.

(not provided)

## SECONDARY - Product Description - From any vendor - A Secondary Support Product.

(not provided)

## SECONDARY - Product Page(s) URL

https://www.redhat.com/en/resources/add-capabilities-enterprise-deployments-datasheet

## Sources: Analyst reviews and exist strategy

Added the verified 0.25 TiB/core capacity figure and a caution that OpenShift Data Foundation is container-oriented rather than a direct general-purpose VM storage equivalent, which affects the realism of the column G/H alternative for mixed estates.
