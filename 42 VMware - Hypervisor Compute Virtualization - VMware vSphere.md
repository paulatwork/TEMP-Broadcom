# VMware vSphere

## Broadcom Software Category

VMware

## Description Broadcom Primary Function & Focus

Hypervisor Compute Virtualization

## Broadcom Broadcom Product Name

VMware vSphere

## Broadcom Prdouct Summary Description (This is important to get right)

VMware vSphere is the core hypervisor (ESXi) and management layer (vCenter) used to provision, run and manage virtual machines across physical hosts, and underpins every VCF and VVF deployment as the base compute layer beneath vSAN, NSX and the management components.

## Analyst Cautions and Industry Findings - Related to the Legacy Broadcom Product. Include newest findings on Broadcom exist strategies

Standalone perpetual vSphere/ESXi licences were discontinued in 2023 in favour of subscription-only, per-core licensing with a 16-core-per-CPU minimum, meaning older hosts with fewer cores per socket are billed as though fully populated. Organisations continuing to run vSphere on expired perpetual licences without an active subscription lose access to security patches and CVE remediation, a risk consistently flagged in trade press covering the Broadcom transition. Broadcom's restriction, in 2025, of public access to the VDDK software development kit, on which third-party migration and backup tools including Microsoft Azure Migrate, Red Hat's Migration Toolkit and Nutanix Move depend, has added practical friction to vSphere exit projects. Gartner's September 2025 guidance projected that more than one-third of VMware workloads will move to other platforms by 2028, but stated that full hypervisor migrations typically take three or more years, and ranked Nutanix and public cloud as more mature migration destinations than Red Hat virtualisation, a consideration relevant to the Red Hat-centric alternative proposed for this row. As a real-world example, Nutanix has reported, as a vendor claim, migrating Western Union off vSphere across 900 to 1,200 applications and 3,900 cores within six months.

Sources: Network World, 'Broadcom hampers VMware migration by blocking downloads of key SDK'; The Register, 'VMware to lose 35 percent of workloads in three years' (September 2025); Slashdot/Ars Technica coverage of Nutanix .NEXT conference claims (April 2026).

## Yes/No - Option for IBM 1:1 Replacement ?? Move from Broadcom from IBM/Red Hat (Same capability level)

Yes

## Replacement Strategy Summary

Red Hat

## PRIMARY - Key Product - IBM Alternative

OpenShift Virtualization

## PRIMARY - Key Product Capability Statement - IBM Alternative

(not provided)

## PRIMARY - IBM Product Page URL

https://www.redhat.com/en/technologies/cloud-computing/openshift/virtualization-engine

## SECONDARY - Product Name - Supporting Product From any vendor - ONLY Where needed to for FULL Capability match for Broadcom. Extend the IBM Key Product.

(not provided)

## SECONDARY - Product Description - From any vendor - A Secondary Support Product.

(not provided)

## SECONDARY - Product Page(s) URL

https://www.redhat.com/en/technologies/cloud-computing/openshift/virtualization-engine

## Sources: Analyst reviews and exist strategy

Tightened column D for precision (ESXi/vCenter naming). Replaced generic caution language with the verified VDDK-blocking finding and the Western Union migration example, and added the Gartner alternative-ranking caveat.
