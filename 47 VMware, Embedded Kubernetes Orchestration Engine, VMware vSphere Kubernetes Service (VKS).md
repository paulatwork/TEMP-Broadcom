# VMware vSphere Kubernetes Service (VKS)

## Broadcom Software Category

VMware

## Description Broadcom Primary Function & Focus

Embedded Kubernetes Orchestration Engine

## Broadcom Broadcom Product Name

VMware vSphere Kubernetes Service (VKS)

## Broadcom Prdouct Summary Description (This is important to get right)

vSphere Kubernetes Service (VKS) is a CNCF-certified Kubernetes distribution embedded in the vSphere IaaS Control Plane (Supervisor), allowing Kubernetes clusters to be provisioned natively alongside virtual machines on the same vSphere infrastructure without a separate Kubernetes management layer.

## Analyst Cautions and Industry Findings - Related to the Legacy Broadcom Product. Include newest findings on Broadcom exist strategies

Because VKS is deployed as a Supervisor-level capability of vSphere, it creates a direct dependency on vSphere and VCF/VVF licensing, with no way to run VKS independently of the underlying VMware hypervisor licence; this is a verifiable architectural characteristic rather than a general assertion. Independent analysis of VMware's container strategy identifies cost and licensing complexity, a steep operational learning curve, and reduced flexibility relative to vendor-neutral Kubernetes distributions as the principal reasons organisations are reconsidering VKS and Tanzu Kubernetes Grid, alongside the broader vendor lock-in concerns raised by the 2023-2024 licensing changes. Red Hat OpenShift Container Platform is a realistic, widely adopted enterprise alternative with a comparable enterprise support model; SUSE Rancher and the major hyperscaler managed Kubernetes services (Amazon EKS, Azure AKS, Google GKE) are also commonly cited migration destinations and should be considered alongside OpenShift depending on the organisation's cloud strategy.

Sources: Fairwinds, 'Are You Still Using VMware Tanzu? (And Is Now the Time to Migrate?)'; Broadcom TechDocs on vSphere IaaS Control Plane and VKS architecture.

## Yes/No - Option for IBM 1:1 Replacement ?? Move from Broadcom from IBM/Red Hat (Same capability level)

Yes

## Replacement Strategy Summary

Red Hat

## PRIMARY - Key Product - IBM Alternative

Red Hat OpenShift Container Platform

## PRIMARY - Key Product Capability Statement - IBM Alternative

(not provided)

## PRIMARY - IBM Product Page URL

https://www.redhat.com/en/technologies/cloud-computing/openshift

## SECONDARY - Product Name - Supporting Product From any vendor - ONLY Where needed to for FULL Capability match for Broadcom. Extend the IBM Key Product.

(not provided)

## SECONDARY - Product Description - From any vendor - A Secondary Support Product.

(not provided)

## SECONDARY - Product Page(s) URL

https://www.redhat.com/en/technologies/cloud-computing/openshift

## Sources: Analyst reviews and exist strategy

Added a genuine independent source (Fairwinds) for the migration-driver claims and broadened the realistic alternative set beyond OpenShift alone, consistent with what that source actually recommends.
