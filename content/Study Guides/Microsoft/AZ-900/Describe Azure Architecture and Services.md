---
title: "Part 2: Describe Azure Architecture and Services"
draft: false
tags:
  - AZ-900
---
## Describe the core architectural components of Azure
### What is Microsoft Azure
Microsoft Azure is a cloud computing platform that provides a wide range of services and solutions for building, deploying, and managing applications and services in the cloud. It's essentially a massive global network of Microsoft-managed datacenters that offer computing resources and services over the internet.
### Get started with Azure accounts
To get started with Azure, you'll need to create an Azure account. This can be done through the Azure portal or by signing up for a free trial or paid subscription. Once you have an account, you can start provisioning and managing your Azure resources.
### Describe Azure physical infrastructure
Azure's physical infrastructure consists of a global network of datacenters located in multiple regions around the world. These datacenters are built and managed by Microsoft, and they house the servers, networking equipment, and storage systems that power Azure's services.
### Describe Azure management infrastructure
The Azure management infrastructure is the backbone that enables you to control and manage your Azure resources. It includes the Azure portal, a web-based interface for managing your Azure services, as well as tools like Azure PowerShell, Azure CLI, and Azure Resource Manager for automating and scripting your deployments.
## Describe Azure compute and networking services
### Describe Azure virtual machines
Azure Virtual Machines (VMs) are one of the core compute services offered by Azure. They allow you to create and run virtual machines in the cloud, giving you the flexibility to run various operating systems and applications without having to manage physical hardware.
### Describe Azure virtual desktop
Azure Virtual Desktop, formerly known as Windows Virtual Desktop, is a desktop and app virtualization service that allows you to run Windows desktops and applications on the cloud. This enables users to access their desktop environments from anywhere, using any device.
### Describe Azure containers
Azure offers several container services, such as Azure Kubernetes Service (AKS) and Azure Container Instances. These services allow you to deploy and manage containerized applications in a scalable and efficient manner, leveraging the benefits of container technology.
### Describe Azure functions
Azure Functions is a serverless computing service that allows you to run code on-demand without having to provision or manage any underlying infrastructure. It's ideal for event-driven architectures, microservices, and automating various processes and workflows.
### Describe application hosting options
Azure provides various options for hosting your applications, including Azure App Service (for web apps, mobile backends, and APIs), Azure Virtual Machines, Azure Kubernetes Service, and Azure Container Instances, among others. You can choose the hosting option that best fits your application's requirements.
### Describe Azure virtual networking
Azure Virtual Network is a crucial networking service that allows you to create logically isolated networks in the cloud and securely connect your Azure resources to each other and to your on-premises networks.
### Describe Azure virtual private networks
Azure VPN Gateway is a service that enables you to create secure, encrypted connections between your on-premises networks and your Azure virtual networks through virtual private networks (VPNs).
### Describe Azure ExpressRoute
Azure ExpressRoute is a dedicated, private network connection service that provides a direct, low-latency connection between your on-premises infrastructure and Azure datacenters, bypassing the public internet.

Azure ExpressRoute is billed based on the ExpressRoute circuit bandwidth and data transfer. There are two main components to the billing:

1. Circuit Bandwidth Charge: This is a fixed monthly fee based on the bandwidth of the ExpressRoute circuit you provision. The higher the bandwidth, the higher the monthly fee.
2. Data Transfer Charge: In addition to the circuit bandwidth fee, you are charged for the volume of data transferred over the ExpressRoute circuit, both inbound and outbound. The rates are based on a per-GB model.

The circuit bandwidth charges are fixed and billed monthly, while the data transfer charges are metered and billed based on your actual usage. Additionally, ExpressRoute has a premium add-on option that provides additional features and capabilities at an extra cost.
### Describe Azure DNS
Azure DNS is a cloud-based domain name system (DNS) service that provides fast DNS resolution and domain hosting services, allowing you to manage your public and private DNS records in the cloud.
## Describe Azure storage services
### Describe Azure storage accounts
Azure Storage Accounts are cloud-based storage services that provide secure, durable, and highly available storage for your data. Each storage account provides access to various Azure storage services, such as Blob Storage, File Storage, Queue Storage, and Table Storage.
### Describe Azure storage redundancy
Azure Storage offers several levels of redundancy to ensure data durability and availability:

- Locally Redundant Storage (LRS): Data is replicated three times within a single datacenter.
- Zone-Redundant Storage (ZRS): Data is replicated across three separate availability zones within the same region.
- Geo-Redundant Storage (GRS): Data is replicated across two different Azure regions, providing protection against regional outages.
- Geo-Zone-Redundant Storage (GZRS): Data is replicated across three availability zones in the primary region and three availability zones in the secondary region.
### Describe Azure storage services
Azure provides several storage services to meet different data storage needs:

- Azure Blob Storage: For storing unstructured data, such as files, images, and backups.
- Azure File Storage: For creating and managing file shares in the cloud.
- Azure Queue Storage: For storing and retrieving messages for asynchronous processing.
- Azure Table Storage: For storing and querying semi-structured, NoSQL data.
- Azure Disk Storage: For providing persistent storage for virtual machines.
### Identify Azure data migration options
Azure offers various data migration options to help you move data to the cloud:

- Azure Data Box: A physical appliance for secure data transfer over the internet.
- Azure Import/Export Service: For transferring large amounts of data using physical storage devices.
- Azure Data Migration Service: A fully managed service for migrating databases to Azure.
- Azure Data Factory: A data integration service for ingesting, transforming, and moving data.
### Identify Azure file movement options
Azure provides several options for moving files and data between on-premises and cloud environments:

- Azure Storage Explorer: A graphical tool for managing Azure storage resources.
- AzCopy: A command-line tool for copying data to and from Azure Blob Storage.
- Azure File Sync: A service for seamlessly replicating files between on-premises and Azure File Storage.
- Azure Data Box: A physical appliance for secure data transfer over the internet.
## Describe Azure identity, access, and security
### Describe Azure directory services
Azure Active Directory (Azure AD) is a cloud-based identity and access management service that provides secure access to Azure and other Microsoft cloud services, as well as on-premises applications.
### Describe Azure authentication methods
Azure AD supports various authentication methods, including:

- Password-based authentication
- Multi-factor authentication (MFA)
- Passwordless authentication (e.g., Windows Hello, FIDO2 security keys)
- Conditional Access policies
- Integration with on-premises directories
### Describe Azure external identities
Azure AD External Identities (formerly Azure AD B2B and B2C) allows organizations to securely share resources and collaborate with external users, such as partners, vendors, or customers, without creating additional Azure AD accounts.
### Describe Azure conditional access
Conditional Access is a feature of Azure AD that allows you to enforce access controls based on specific conditions, such as user identity, location, device health, and risk levels. This helps ensure that only authorized users and devices can access your resources.
### Describe Azure role-based access control (RBAC)
Azure RBAC is an authorization system that provides fine-grained access management for Azure resources. It allows you to assign specific roles and permissions to users, groups, or applications, ensuring that they can only perform the necessary actions on the resources they need.
### Describe zero trust model
The zero trust model is a security approach that assumes no user or device should be trusted by default, regardless of their location or network. It requires continuous verification and validation of users, devices, and access requests before granting access to resources.
### Describe defense-in-depth
Defense-in-depth is a security strategy that involves layering multiple security controls and mechanisms to protect against various threats. It aims to provide redundancy and mitigate the risk of a single point of failure in the security posture.
### Describe Microsoft Defender for Cloud
Microsoft Defender for Cloud (formerly Azure Security Center) is a unified security management solution that provides advanced threat protection, security policy management, and continuous monitoring and remediation for your Azure resources, as well as hybrid and multi-cloud environments.
