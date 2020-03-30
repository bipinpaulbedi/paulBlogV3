---
description: architect's checklist for transforming zero to cloud | 2020-March-30
---

# Simplified azure cloud adoption framework

The [Cloud Adoption Framework](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/) helps customers undertake a simplified cloud adoption journey. The framework contains detailed information about an end-to-end cloud adoption journey and is designed primarily for cloud architects and the cloud strategy teams leading cloud adoption efforts. This blog post primarily focus on step-by-step checklist that can help you complete your journey based on Microsoft azure cloud adoption framework recommended practices.

![Image Source - Microsoft](../.gitbook/assets/caf-overview.png)

#### Azure adoption checklist

* [x] **Start strategy and plan** - establishing clear [business outcomes](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/strategy/business-outcomes/), a clearly defined [digital estate plan](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/digital-estate/), and well-understood [adoption backlogs](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/migrate/migration-considerations/prerequisites/migration-backlog-review)
  * [x] Get critical business events e.g. data-center exit
  * [x] Get cloud business motivation against each event e.g. Cost savings
  * [ ] Classify each motivation as migration or innovation e.g. Cost saving for migration or Increasing business agility for innovation
  * [ ] **See** [**documenting business outcomes**](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/strategy/business-outcomes/business-outcome-template)**, or download the** [**business outcome template**](https://archcenter.blob.core.windows.net/cdn/business-outcome-template.xlsx) **\[TOOL\]**
  * [ ] Define fiscal outcomes e.g. increased revenue, reduced cost or increased profit
  * [ ] Define agility outcomes e.g. faster time to market or low provision time
  * [ ] Define reach-ability outcomes e.g. global access or data sovereignty
  * [ ] Define customer engagement outcomes e.g. cycle time, see [six sigma](https://www.isixsigma.com/dictionary/cycle-time/)
  * [ ] Define performance outcomes e.g. Increase in number of transactions or capacity
  * [ ] Define reliability outcomes e.g. High uptime
  * [ ] Understand and explain the myths
    * [ ] The cloud is always cheaper
    * [ ] Everything should go into the cloud
    * [ ] Mirroring my on-premises environment will help me save money in the cloud
    * [ ] Server costs drive business cases for cloud migration
    * [ ] An operating expense model is better than a capital expense model
    * [ ] Moving to the cloud is like flipping a switch
  * [ ] Calculate revenue deltas
  * [ ] Calculate cost deltas e.g. operating cost reductions
  * [ ] Calculate gains $$Gains = Revenue Deltas + CostDeltas$$ 
  * [ ] Build a business justification $$ROI = (Gain - Investment)/Investment$$
  * [ ] Transform account model i.e. cost center to profit center using charge back or showback or awareness-back models
  * [ ] Identify first adoption project
  * [ ] Inform business about depth of justification vs time to business impact
  * [ ] Inform business about depth of initial planning vs delayed technical decisions
  * [ ] Inform business about long-term operations vs time to adoption
  * [ ] Inform business about re-hosting vs re-architecture
  * [ ] Inform business about feature focus vs customer empathy
  * [ ] Inform business about well-governed vs speed/agility
  * [ ] Inform business about broad management investments vs no -ops /low ops
  * [ ] Inform business about centralized control vs delegated control
  * [ ] Document business outcome with respect to accountable department/person, measurable target, time frame and priority
  * [ ] Understand and explain the myths
    * [ ] It's easy to make rationalization decisions early in the process
    * [ ] Cloud adoption has to wait for all workloads to be rationalized
    * [ ] Business justification has to wait for all workloads to be rationalized
  * [ ] Articulate 5R's
    * [ ] Does the system require Re-hosting i.e. lift and shift
    * [ ] Does the system require Refactoring
    * [ ] Does the system require Re-architecture
    * [ ] Does the system require Rebuild
    * [ ] Does the system require Replacement
  * [ ] Identify digital asset planning approach Workload-driven, Asset-driven or Incremental approach
  * [ ] Create [inventory of digital assets](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/digital-estate/inventory)
  * [ ] Rationalize the digital estate using incremental inventory, quantitative analysis i.e. streamline decisions or qualitative analysis i.e. temporary assumptions
  * [ ] Align cost models using [Azure Migrate](https://docs.microsoft.com/azure/migrate/migrate-overview), [Total cost of ownership \(TCO\) calculator](https://azure.microsoft.com/pricing/tco/calculator), [Azure pricing calculator](https://azure.microsoft.com/pricing/calculator) or [Azure Cost Management](https://azure.microsoft.com/services/cost-management)
  * [ ] **Create a cloud adoption plan using** [**Azure DevOps Demo Generator**](https://aka.ms/adopt/plan/generator) **\[TOOL\]**
  * [ ] Define workloads in cloud adoption plan
  * [ ] Priotise workloads in cloud adoption plan
  * [ ] Align assets to workloads
  * [ ] Review plan and create iteration and release path
  * [ ] Generate estimated timelines
  * [ ] Identify team capability gaps and concerns
  * [ ] Train staff via Microsoft Learn
  * [ ] **Validate your findings using** [**Data Migration Assistant**](https://www.microsoft.com/en-us/download/details.aspx?id=53595) **and** [**Azure Migrate**](https://azure.microsoft.com/en-us/services/azure-migrate/) **\[TOOL\]**
* [ ] **Start Readiness** - ensure the readiness of staff through [skills and learning plans](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ready/suggested-skills).
  * [ ] Organise your resources in management groups, subscription, resource groups and resources
  * [ ] [Use Microsoft recommended naming strategy](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ready/azure-best-practices/naming-and-tagging)
  * [ ] Tag resource for better metadata, documentation, automation and cost tracking
  * [ ] Define permission using Azure RBAC
  * [ ] For cost management and define limits, dev/test pricing or reserve instance to manage cost
  * [ ] **Use the** [**Governance Benchmark tool**](https://cafbaseline.com) **to identify potential gaps in your organization's cloud governance approach \[TOOL\]**
  * [ ] Use Azure blueprints to define templates for role, policy, arm, resource groups
  * [ ] Define compliance policy
  * [ ] Define plan to Monitoring and Reporting
    * [ ] Utilise Azure monitor to measure infrastructure performance
    * [ ] Utilise service health for status and uptime
    * [ ] Utilise Azure advisor for recommendation for availability, security, performance, cost and operational excellence
    * [ ] Utilise [Azure Security Center](https://docs.microsoft.com/azure/security-center) to monitor and create a secure infrastructure
  * [ ] Finalise you IAC tool
  * [ ] Define different landing zone as shared services, hub and spoke model, or independent zones
  * [ ] Deploy first landing zone. [See example](https://docs.microsoft.com/en-us/azure/governance/blueprints/samples/caf-migrate-landing-zone/deploy)
  * [ ] Monitor and review compute options
  * [ ] Monitor and review networking options
  * [ ] Monitor and review storage options
  * [ ] Monitor and review data options
  * [ ] Monitor and review RBAC
  * [ ] [Implement a secure hybrid network](https://docs.microsoft.com/en-us/azure/architecture/reference-architectures/dmz/secure-vnet-dmz?toc=https://docs.microsoft.com/azure/cloud-adoption-framework/toc.json&bc=https://docs.microsoft.com/azure/cloud-adoption-framework/_bread/toc.json)
  * [ ] [Implement IAM best practices](https://docs.microsoft.com/en-us/azure/security/fundamentals/identity-management-best-practices?toc=https://docs.microsoft.com/azure/cloud-adoption-framework/toc.json&bc=https://docs.microsoft.com/azure/cloud-adoption-framework/_bread/toc.json)
  * [ ] [Implement networking best practices](https://docs.microsoft.com/en-us/azure/security/fundamentals/network-best-practices?toc=https://docs.microsoft.com/azure/cloud-adoption-framework/toc.json&bc=https://docs.microsoft.com/azure/cloud-adoption-framework/_bread/toc.json)
  * [ ] [Implement operational best practices](https://docs.microsoft.com/en-us/azure/security/fundamentals/operational-best-practices?toc=https://docs.microsoft.com/azure/cloud-adoption-framework/toc.json&bc=https://docs.microsoft.com/azure/cloud-adoption-framework/_bread/toc.json)
  * [ ] [Review other best practices](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ready/azure-best-practices/)
* [ ] **Start Adoption** - Ensure proper implementation of desired changes, across IT and business processes, to achieve business outcomes.
  * [ ] **Start Migration** - Iterative execution of the [cloud implementation methodology](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/getting-started/migrate#cloud-implementation) adhering to the tested process of Assess, Migrate, Optimize, and Secure & Manage to create a repeatable process for migrating workloads.
    * [ ] Utilise Azure Migrate to confirm the migration suitability of on-premises assets, performance-based sizing and cost estimates for running on-premises assets in Azure
    * [ ] Review incremental rationalisation by power of 10 methodology
    * [ ] Review all 5R's
    * [ ] Inform all stakeholders
    * [ ] **Perform migration using \[TOOLS\]**
      * [ ] Azure Migrate
      * [ ] Azure Site Recovery
      * [ ] Azure Database Migration Service
      * [ ] Data Migration Assistant
      * [ ] SQL Server Migration Assistant
      * [ ] Database Experimentation Assistant
      * [ ] Cosmos DB Data Migration Tool
      * [ ] UnifyCloud
      * [ ] Cloudamize
      * [ ] Zerto
      * [ ] Carbonite
      * [ ] Movere
      * [ ] Cosmos DB Partners
      * [ ] Azure DevOps
      * [ ] Microsoft Planner
      * [ ] Microsoft Project
      * [ ] Microsoft Team
    * [ ] Monitor and Test
    * [ ] Obtain assistance if required via Microsoft support
    * [ ] Validate and compare your scenario against [sample scenarios](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/migrate/azure-best-practices/contoso-migration-overview)
    * [ ] Validate for [business continuity](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/migrate/azure-best-practices/) best practices
    * [ ] Monitor and continuously improve migration process by defining assessment criteria
    * [ ] Migrate using promoting, remediating, replicating or staging workloads for multiple environments
    * [ ] Define and execute business promotion and retrospective [activities](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/migrate/migration-considerations/optimize/)
    * [ ] Create environement of continuous learning and up skilling
  * [ ] **Start Innovation** - Drive business value through innovation activities that unlock new technical skills and expanded business capabilities.
    * [ ] Perform qualitative and quantitative testing
    * [ ] **Enhance data discoverability using** [**Azure Data Catalog**](https://docs.microsoft.com/azure/data-catalog)**,** [**Azure Data Share**](https://docs.microsoft.com/azure/data-share) **and** [**Azure Time Series Insights**](https://docs.microsoft.com/azure/time-series-insights/time-series-insights-update-overview) **\[Tools\]**
    * [ ] Innovate using PaaS \(App service\), Cloud native \(Serverless\) or Isolating point of failure \(Azure front door, traffic manager\)
    * [ ] Empower adoption by collaboration and LiveOps
    * [ ] Interact through devices i.e. IOT Hub, Location intelligence etc. e.g. Azure Sphere
    * [ ] Innovate in [cloud native landscape](https://www.cncf.io/) by experimenting in deployment and clustering e.g. Kubernetes
    * [ ] [Adopt innovation best practices](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/innovate/best-practices/)
    * [ ] [Adopt innovation proce best practices](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/innovate/considerations/)
* [ ] **Start Operating**
  * [ ] Define Governing body. Align corporate policy to tangible risks, mitigated through policy, process, and cloud-based governance tooling.
    * [ ] Envision an end state
    * [ ] Identify business risk, compliance and processes
    * [ ] Define maturity vectors and governance considerations
      * [ ] Sensitive data in the cloud
      * [ ] Mission-critical apps in the cloud
      * [ ] Cloud cost management
      * [ ] Multicloud
      * [ ] Complex/legacy identity management
      * [ ] Multiple layers of governance
    * [ ] Define governance principles for
      * [ ] Cost Management - [Download governance discipline template](https://archcenter.blob.core.windows.net/cdn/fusion/governance/Cost%20Management%20Discipline%20Template.docx)
      * [ ] Security Baseline - [Download governance discipline template](https://archcenter.blob.core.windows.net/cdn/fusion/governance/Security%20Baseline%20Discipline%20Template.docx)
      * [ ] Resource Consistency - [Download governance discipline template](https://archcenter.blob.core.windows.net/cdn/fusion/governance/Resource%20Consistency%20Discipline%20Template.docx)
      * [ ] Identity Baseline - [Download governance discipline template](https://archcenter.blob.core.windows.net/cdn/fusion/governance/Identity%20Baseline%20Discipline%20Template.docx)
      * [ ] Deployment Acceleration - [Download governance discipline template](https://archcenter.blob.core.windows.net/cdn/fusion/governance/Deployment%20Acceleration%20Discipline%20Template.docx)
    * [ ] Utilise [governance benchmark tool](https://cafbaseline.com) to help you identify gaps in your organization across six key domains
  * [ ] Define management team. Expand IT operations to ensure cloud-based solutions can be operated through secure, cost effective processes using modern, cloud-first operations tools.
    * [ ] Define Process, tools and purpose for
      * [ ] Inventory and visibility
      * [ ] Operational compliance
      * [ ] Protect and recover
    * [ ] Define plan and tools for monitoring and alerting
    * [ ] Create specialisation for platforms or workloads
    * [ ] Establish an operational fitness review
    * [ ] Define resiliency checklist for specific Azure services
    * [ ] Define plan for failure mode analysis for Azure applications
    * [ ] Create a disaster recovery plan and process
      * [ ] Informing stakeholders
      * [ ] Data recovery
      * [ ] Business continuity
      * [ ] RPO
      * [ ] RTO
  * [ ] Define support team. Align people and teams to deliver proper cloud operations and adoption.
    * [ ] Define RACI matrix
    * [ ] Create cloud capability matrix
    * [ ] Build technical skills

Additional tools that you might have to review for a successful cloud adoption

* [Cloud Governance](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/)
* [Reliability Architecture](https://docs.microsoft.com/azure/architecture/framework/resiliency/overview)
* [Skill Building](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ready/suggested-skills)
* [DevOps Approach](https://docs.microsoft.com/azure/devops/learn/)
* [Architecture Center](https://docs.microsoft.com/azure/architecture/)
* [Pricing Calculator](https://azure.microsoft.com/pricing/calculator)







