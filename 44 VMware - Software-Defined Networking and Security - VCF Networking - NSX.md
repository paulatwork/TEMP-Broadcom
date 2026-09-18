# VCF Networking, NSX

## Broadcom Software Category

VMware

## Description Broadcom Primary Function & Focus

Software-Defined Networking & Security

## Broadcom Broadcom Product Name

VCF Networking, NSX

## Broadcom Prdouct Summary Description (This is important to get right)

VCF Networking, built on NSX, is a software-defined networking and security platform providing Layer 2-3 overlay networking, distributed routing, and the distributed firewall for microsegmentation, delivered as an integrated layer of VMware Cloud Foundation rather than as a standalone licensed product.

## Analyst Cautions and Industry Findings - Related to the Legacy Broadcom Product. Include newest findings on Broadcom exist strategies

NSX is widely regarded, including in independent security commentary, as one of the most difficult layers of the VMware stack to exit. Distributed firewall policy objects, tags, groups and overlay network configurations are tightly coupled to the VMware control plane; specialist microsegmentation vendor ColorTokens describes these policies as encoding years of accumulated knowledge about application dependencies, trust boundaries and risk tolerance, with no automated cross-vendor export path, requiring manual policy re-authoring during migration. Standalone NSX licensing was eliminated in 2023, so customers who want NSX at all must purchase full VCF. Genuine like-for-like alternatives for VM-centric microsegmentation and network virtualisation include Cisco ACI, Illumio and Calico Enterprise; Red Hat's OpenShift networking stack (OVN-Kubernetes, Cilium) is Kubernetes-native and only replaces NSX's function where workloads are also being containerised onto OpenShift, so it should not be presented as a direct substitute for NSX in VM-only environments. Gartner's September 2025 guidance recommended selective, application-by-application replatforming over wholesale network re-architecture given the effort involved.

Sources: ColorTokens, 'Rethinking Microsegmentation During a VMware NSX Exit'; The Register, 'VMware to lose 35 percent of workloads in three years' (Gartner Symposium coverage, September 2025); Broadcom TechDocs migration guidance on distributed firewall configuration.

## Yes/No - Option for IBM 1:1 Replacement ?? Move from Broadcom from IBM/Red Hat (Same capability level)

Yes

## Replacement Strategy Summary

Red Hat

## PRIMARY - Key Product - IBM Alternative

OpenShift networking + partner networking

## PRIMARY - Key Product Capability Statement - IBM Alternative

(not provided)

## PRIMARY - IBM Product Page URL

https://www.redhat.com/en/technologies/cloud-computing/openshift/platform-plus

## SECONDARY - Product Name - Supporting Product From any vendor - ONLY Where needed to for FULL Capability match for Broadcom. Extend the IBM Key Product.

(not provided)

## SECONDARY - Product Description - From any vendor - A Secondary Support Product.

(not provided)

## SECONDARY - Product Page(s) URL

https://www.redhat.com/en/technologies/cloud-computing/openshift/platform-plus

## Sources: Analyst reviews and exist strategy

Replaced the direct quotation with a paraphrase per style guidance, added a genuine source (ColorTokens) for the migration-complexity claim as requested, and flagged that OpenShift networking only substitutes for NSX where workloads move to containers, a limitation on the column G/H alternative.
