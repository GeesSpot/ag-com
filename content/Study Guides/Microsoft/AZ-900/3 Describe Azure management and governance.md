---
title: Describe Azure management and governance
draft: false
tags:
  - AZ-900
---
## Describe cost management in Azure
### Describe factors that can affect costs in Azure
There are several factors that can impact your overall costs when using Azure services. Understanding these factors is crucial for effective cost management and optimization:

1. Resource types and configurations: The types of resources you provision (e.g., virtual machines, storage, databases) and their configurations (such as instance sizes, storage tiers, and performance levels) directly affect your costs.
2. Usage and consumption: Costs are typically based on your actual usage and consumption of Azure services. The more resources you consume, the higher your costs will be.
3. Data transfers: Inbound data transfers to Azure are free, but outbound data transfers are charged based on the volume of data transferred out of Azure datacenters.
4. Geographic regions: The pricing for some Azure services may vary based on the region where your resources are deployed.
5. Reserved instances and pricing models: Azure offers pricing models like reserved instances and Azure Hybrid Benefit, which can provide cost savings if you have predictable workloads or existing on-premises licenses.
6. Support plans: The level of Azure support plan you choose (e.g., Basic, Developer, Standard, or Professional Direct) can affect your overall costs.
### Compare the Pricing and Total Cost of Ownership calculators
- Pricing calculator: This tool allows you to estimate the costs of various Azure services and resources based on your specific requirements and usage patterns. You can configure different scenarios and get detailed pricing estimates.
- Total Cost of Ownership (TCO) calculator: The TCO calculator is designed to help you compare the costs of running your workloads in the cloud versus on-premises. It takes into account not only the direct costs of Azure services but also factors like hardware, software, facilities, and labor costs for on-premises infrastructure.
### Describe the Microsoft Cost Management tool
Microsoft Cost Management is a built-in tool within the Azure portal that provides comprehensive cost monitoring, analysis, and optimization capabilities. It allows you to:

- View and analyze your Azure spending across subscriptions, resource groups, and services.
- Set up budgets and cost alerts to proactively monitor and control your spending.
- Optimize your costs by identifying and taking action on underutilized resources or potential savings opportunities.
- Export cost data for further analysis or integration with external systems.
- Forecast future costs based on your historical usage patterns.
### Describe the purpose of tags
Tags in Azure are metadata labels that you can apply to your Azure resources, resource groups, or subscriptions. Tags serve several purposes in cost management and organization:

1. Cost tracking and allocation: By tagging resources with cost centers, departments, or project names, you can easily identify and allocate costs to the appropriate business units or stakeholders.
2. Resource organization: Tags allow you to logically group and categorize your resources based on specific criteria, making it easier to manage and locate them.
3. Access control and governance: Tags can be used in combination with Azure Policy and Role-Based Access Control (RBAC) to enforce compliance and control access to resources based on their tags.
4. Cost optimization: By tagging resources, you can identify underutilized or unnecessary resources and take actions to optimize your costs.
5. Automation and scripting: Tags can be leveraged in automation scripts and templates to apply consistent configurations or perform actions on resources based on their tags.

Using tags effectively can greatly improve your ability to manage, monitor, and optimize your Azure costs and resources.
## Describe features and tools in Azure for governance and compliance
Governance and compliance are critical aspects of managing cloud resources effectively and securely. Azure provides several features and tools to help organizations maintain control, enforce policies, and meet regulatory requirements.
### Describe the purpose of Microsoft Purview
Microsoft Purview is a unified data governance service that helps organizations manage and govern their on-premises, multi-cloud, and software-as-a-service (SaaS) data. Its key purposes include:

1. Data discovery and mapping: Purview automatically scans and catalogs data sources across your entire data estate, providing a comprehensive map of your data landscape.
2. Data classification and labeling: It uses machine learning and built-in classifiers to automatically classify and label sensitive data, making it easier to identify and protect critical information.
3. Data lineage and impact analysis: Purview tracks the flow of data across systems, enabling you to understand data lineage and assess the potential impact of changes.
4. Data access control and monitoring: It helps enforce data access policies and monitor data usage patterns, ensuring that only authorized users can access sensitive information.
### Describe the purpose of Azure Policy
Azure Policy is a service that enables you to define and enforce organizational policies across your Azure resources. Its key purposes include:

1. Policy enforcement: You can create and assign policies to enforce desired configurations, security standards, and compliance requirements for your Azure resources.
2. Auditing and remediation: Azure Policy continuously evaluates your resources for compliance and allows you to take remediation actions to bring non-compliant resources back into compliance.
3. Consistent management: By applying policies at the management group, subscription, or resource group level, you can ensure consistent management and governance across your entire Azure environment.
### Describe the purpose of resource locks
Resource locks in Azure are a feature that allows you to restrict operations on high-value resources, preventing accidental or unauthorized modifications or deletions. The main purposes of resource locks include:

1. Prevent accidental deletion: By applying a delete lock, you can protect critical resources from being accidentally deleted, mitigating the risk of data loss or service disruptions.
2. Restrict resource modifications: With a read-only lock, you can ensure that resources are not modified or updated, maintaining their intended configuration.
3. Enforce governance and compliance: Resource locks can be used in conjunction with Azure Policy and RBAC to enforce governance policies and ensure compliance with regulatory requirements.
4. When multiple locks are assigned to a resource, the most restrictive lock takes precedence. For example, if a `ReadOnlyLock` is applied to a resource group, and a `DeleteLock` is applied to a specific resource within that group, the `DeleteLock` on the individual resource will take precedence, preventing both deletion and modification.
### Describe the purpose of the Service Trust portal
The Service Trust portal is a dedicated website provided by Microsoft that offers transparency and insights into the security, compliance, privacy, and compliance practices for Microsoft Cloud services, including Azure. Its key purposes include:

1. Compliance documentation: The portal provides access to audit reports, compliance guides, and certifications for various industry standards and regulations, such as ISO, NIST, FedRAMP, and GDPR.
2. Transparency into security practices: It offers detailed information on Microsoft's security practices, including incident response processes, data handling procedures, and security controls implemented in Azure datacenters.
3. Regional compliance mapping: The portal helps organizations understand the compliance offerings and certifications available in different geographic regions, enabling them to make informed decisions about data residency requirements.
4. Compliance manager: This feature within the Service Trust portal allows organizations to manage their compliance activities, assess their risk, and track their compliance posture across Microsoft Cloud services.
## Describe features and tools for managing and deploying Azure resources
### Describe tools for interacting with Azure
Azure provides various tools and interfaces for interacting with and managing your resources, including:

1. Azure Portal: A web-based graphical user interface (GUI) that allows you to create, manage, and monitor Azure resources through a user-friendly interface.
2. Azure PowerShell: A command-line shell and scripting environment for managing Azure resources using PowerShell cmdlets.
3. Azure CLI: A cross-platform command-line tool for managing Azure resources using command-line interfaces.
4. Azure Cloud Shell: A web-based shell environment that provides pre-installed Azure tools (PowerShell and CLI) for managing resources directly from your web browser.
5. Azure SDKs: Software Development Kits (SDKs) for various programming languages (e.g., .NET, Java, Python, Node.js) that allow you to programmatically manage Azure resources.
### Describe the purpose of Azure Arc
Azure Arc is a service that extends Azure management capabilities to on-premises, multi-cloud, and edge environments. Its primary purposes include:

1. Hybrid management: Azure Arc allows you to manage and govern resources across your entire hybrid and multi-cloud infrastructure from a single pane of glass within the Azure portal.
2. Consistent governance: By bringing non-Azure resources under Azure management, you can apply consistent Azure policies, security controls, and compliance standards across your entire IT estate.
3. Simplified operations: With Azure Arc, you can streamline operations by using familiar Azure tools and services to manage resources, regardless of their location (on-premises, other clouds, or edge).
4. Cost optimization: By consolidating management and governance across your hybrid environment, Azure Arc can help optimize costs and improve operational efficiency.
### Describe Azure Resource Manager and Azure ARM templates
Azure Resource Manager (ARM) is the deployment and management service in Azure that enables you to create, update, and delete resources in a secure and consistent manner.

Azure Resource Manager Templates (ARM templates) are JSON files that define the infrastructure and configuration of your Azure resources. They provide several benefits:

1. Declarative syntax: ARM templates use a declarative syntax, allowing you to define the desired state of your resources rather than writing imperative scripts.
2. Infrastructure as Code (IaC): ARM templates enable you to treat your infrastructure as code, making it easier to version, share, and automate deployments.
3. Consistent deployment: Templates ensure that resources are deployed consistently across different environments (development, staging, production), reducing configuration drift.
4. Resource organization: ARM templates allow you to organize and group related resources together, making it easier to manage and maintain your infrastructure.
5. Parameterization: You can define parameters in templates, enabling you to customize deployments based on specific requirements or environments.

ARM templates can be deployed using various tools, such as the Azure portal, PowerShell, Azure CLI, and Azure Pipelines (for continuous integration and continuous deployment scenarios).