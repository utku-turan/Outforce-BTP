# SAP BTP Basics
My notes from the SAP Training [Discovering SAP Business Technology Platform](https://learning.sap.com/learning-journeys/discover-sap-business-technology-platform)

## Introduction

**SAP BTP:**
- Platform-as-a-service (PaaS)
- in-memory capabilities, core platform services, and unique services for building and extending intelligent, mobile-enabled cloud applications.
- the technological foundation of the intelligent, sustainable enterprise.
- develop the exact application you need – without investing in on-premise or cloud infrastructure.

![image](https://github.com/user-attachments/assets/88a98448-a910-4b3d-9153-e8b2bd372340)

**Cloud Terminology:**
- Cloud computing can lower your costs by allowing you to use only the resources you need on demand.
- Cloud computing offerings are available in different deployment models and service models.
- Cloud landscapes are clustered over several regions to ensure higher availability and lower latency.
- With the increasing amount of cloud capabilities, the importance of virtualization and container technologies is becoming even more relevant than ever before.
- Multi Cloud: combines several cloud offerings from multiple providers in one single heterogenous architecture to improve cloud infrastructure capabilities and cost.
- Hyperscaler: large provider of computing services. AWS, Microsoft Azure, Google Cloud Platform, and Alibaba Cloud
- SAP BTP is available in several regions with these providers. SAP supports multi-cloud landscapes through this.

**Deployment Models:**
- Public Cloud: Resources are shared but operative data is separated on application level.
- Private Cloud: Resources are not shared, assigned to one customer.
- Hybrid Cloud: Mixture of Public and Private Cloud. (sometimes also on-premise)

**Service Models:**
- IaaS (Infrastructure as a Service): subscribing to hardware resources (Network storage, databases, etc.)
- PaaS (Platform as a Service):
  - subscribing to middleware functionalities on top of your virtual infrastructure.
  - Adapt functions and extend the platform with your custom logic and applications. (e.g. SAP BTP)
  - usually with predefined services which you can activate and use.
  - security services for authorization and authentication, clustering, load balancing, routing, or database services. 
- SaaS (Software as a Service): subscribing to applications based on your demand. (e.g. Netflix, SAP Analytics Cloud, S/4HANA Cloud) Often, you don't have much ability to customize, you can only consume them, and sometimes make some small configurations.

**Business Processes:**
- Lead to Cash: CRM and Customer Experience, from lead to order fulfillment and service delivery
- Design to Operate: Digital Supply Chain, entire lifecycle of products in an end-to-end supply chain process, how a product is designed, planned, manufactured, and delivered, to how it operates and is maintained.
- Source to Pay: Network and Spend Management, finding, negotiating with, and contracting the supplier of goods, and culminates in final payment for these goods. 
- Recruit to Retire: HR and People Engagement, focuses on the employee's lifecycle in the organization, starts with workforce planning, then hiring and onboarding, employee data, time recording, payroll, and employee retiring.

**SAP Signavio:**
- BPM (Business Process Management) software
- provides features to structure, model, and analyze business processes.
- Capture relevant process information (for example, through interviews)
- Design processes (visualize tasks, decisions, and responsibilities)
- Execute processes (for example, by systems or employees)
- Document processes (for example, by creating a handbook)
- Measure processes (for example, cycle times, costs, other KPIs)

### Main Use-Cases for SAP BTP:
- **Keep the core clean:** Create and operate highly integrated side-by-side solution extensions to individualize your business processes without harming the stable application core. You can deliver new features agile and fast with SAP BTP as the underlying platform.
- **Optimize & automate business processes:** Automate manual tasks as well as cross-application workflows, leveraging a broad set of pre-defined content. The SAP Business Technology Platform offers SAP Build Process Automation - a low-code/no-code based tooling to enable also business or process experts - besides the classical developers - to create automated processes or process extensions. It also offers automations for manual tasks by leveraging robotic automation technologies. In collaboration with the SAP Business Process Intelligence (BPI) portfolio with solutions like Signavio Process insights or Customer insights from the Qualtrics applications, it provides an opportunity to directly take actions to possible findings from process or experience analysis.
- **Drive decisions based on data:** Support your business users with the information at hand or AI-based recommendations to improve decision speed and quality – leveraging any data sources. It's essential that organizations have a consolidated view across all their data assets and are able to achieve insight and make real-time decisions. Good data quality and data handling is important because of the increasing amount of data. To get value from your data, you must analyze and interpret it. Good data quality and good technologies to handle data is key for a flexible and scalable business.
- **Accelerate move to Cloud**

## SAP BTP: Architecture and Services
