# SAP BTP Basics
My notes from the SAP Training [Discovering SAP Business Technology Platform](https://learning.sap.com/learning-journeys/discover-sap-business-technology-platform)

## Introduction

**SAP BTP:**
- Platform-as-a-service (PaaS)
- in-memory capabilities, core platform services, and unique services for building and extending intelligent, mobile-enabled cloud applications.
- the technological foundation of the intelligent, sustainable enterprise.
- develop the exact application you need – without investing in on-premise or cloud infrastructure.

![image](https://github.com/user-attachments/assets/88a98448-a910-4b3d-9153-e8b2bd372340)

### Cloud Terminology
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
![image](https://github.com/user-attachments/assets/0c3aa458-f7a1-4a5a-9c69-03e63195fe55)

**SAP BTP Functionality Areas:**
- Application Development
- Automation
- Integration
- Data & Analytics
- Artificial Intelligence

**SAP BTP Commercial Models:**
- *Pay-As-You-Go:* start small and grow without constraints. start using cloud services in your production environment with no upfront cost, no minimum usage requirements, and no financial commitments.
- *CPEA: Cloud Platform Enterprise Agreement:* consumption of cloud credits based on actual usage. These cloud credits get paid upfront like a pre-paid model. Get access to all services available under CPEA and configure them in your global account with just one contract.
- *Subscription:* choose a fixed set of services for a fixed rate, regardless of actual consumption. The contract includes the exact services you can use in your project and will be provisioned in your global account for entitlements.
- *Free Tier Services:* limited by usage capacity on a monthly basis. They do not expire. You can consume them for as long as your account is active, and you have not reached the service plan limits. You can upgrade to a paid service plan through the SAP BTP cockpit – no technical migration required.

### Architecture of SAP BTP
![image](https://github.com/user-attachments/assets/bfe0e681-847d-4052-9f76-466f66fa86a5)
![image](https://github.com/user-attachments/assets/6c10a8c8-e487-4d29-8f79-f591c6c257e7)
![image](https://github.com/user-attachments/assets/6df943dd-bbe8-49ab-b519-e041c0b32ee4)


#### Global Account
- A global account is the realization of a contract you made with SAP.
- A global account is used to manage directories, subaccounts, members, entitlements, and quotas.
- You receive entitlements and quotas to use platform resources per global account and then distribute the entitlements and quotas to the subaccount for actual consumption.

#### Directory
- Directories allow you to organize and manage your subaccounts according to your technical and business needs.
- A directory can contain directories and subaccounts to create a hierarchy.
- Using directories to group other directories and subaccounts is optional - you can still create subaccounts directly under your global account.
- You can create a hierarchical structure that is 7 levels deep.
 - The highest level of a given path is always the global account and the lowest is a subaccount, which means that you can have up to 5 levels of directories.
  
#### Subaccount 
- Subaccounts let you structure a global account according to your organization's and project's requirements with regard to members, authorizations, and entitlements.
- A global account can contain one or more subaccounts in which you deploy applications, use services, and manage your subscriptions.
- Subaccounts in a global account are independent of each other.
- This is important to consider with respect to security, member management, data management, data migration, integration, and so on when you plan your landscape and overall architecture.

#### Entitlements
- An entitlement is your right to provision and consume a resource.
- Entitlements are the service plans that you're entitled to use.
- You could also say an entitlement is a booked option or are the booked services you can use in your SAP BTP global account.

#### Region
- You can deploy applications in different regions.
- Each region represents a geographical location (for example, Europe, US East) where applications, data, or services are hosted.
- A region is chosen at the subaccount level.
- For each subaccount, you select exactly one region.
- The selection of a region is dependent on many factors: for example, application performance (response time, latency) can be optimized by selecting a region close to the user.
- The global account itself is also running in a region.
- **Infrastructure:** The infrastructure layer of a region is either provided by SAP or by one of SAP's Instrastructure as a Service (IaaS) partners Amazon Web Services (AWS), Microsoft Azure, Google Cloud Platform (GCP), and Alibaba Cloud.
- **Environments:** Environments constitute the actual platform as a service offering of SAP BTP that allows for the development and administration of business applications. Each environment comes equipped with the tools, technologies, and runtimes that you need to build applications.
- **Services:** Services enable, facilitate, or accelerate the development of business applications and other platform services on SAP BTP. You find all available services in the SAP Discovery Center.
- **Data:** Your business and application data is managed through services like the SAP HANA Cloud service or the SAP Datasphere service.
- **Applications:** The business applications that you deploy in a region build on top of, and make use of, the layers underneath.

#### Subaccount
Subaccounts hold:
- **Applications:** Business applications or custom developments running and operating in this subaccount - they can even get bounded to services and subscriptions inside of this subaccount if needed.
- **Services:** Service instances created and running in this subaccount.
- **Subscriptions:** Service subscriptions and their capabilities accessible in this subaccount.

Each subaccount in SAP BTP is linked to a specific region, which determines the physical location where applications, data, or services are hosted. The assigned region is important for deploying applications and accessing the SAP BTP cockpit using the corresponding regional cockpit URL. However, the region of your subaccount is not dependent on your geographical location. For instance, even if you are based in the United States, your subaccount could be operating in a region in Europe.

The entitlements and quotas that have been purchased for a global account have to be assigned to the individual subaccounts.

- **Quota:** represents the numeric quantity that defines the maximum allowed consumption of a resource. In other words, how much of a service plan you're entitled to use.
- **Service plan:** is the representation of the costs and benefits for a given variant of a particular service. For instance, a database may be configured with various "T-shirt sizes", each of which is a different service plan.

#### Environment

