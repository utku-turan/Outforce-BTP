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
- Runtime + Services + Tools that you need to build applications.
- the actual Platform as a Service offering of SAP BTP
- anchored in SAP BTP on the subaccount level
- multi-environment subaccount is possible. (Advantage is that you only need to manage users, authorizations, and entitlements once per subaccount.)

![image](https://github.com/user-attachments/assets/c4039bbc-ba4b-4d1d-911a-ef2a9f1a9ce0)

**Cloud Foundry Environment:**
- The Cloud Foundry environment enables the creation of polyglot cloud applications.
- an open-source, cloud-native platform as a service (PaaS)
- includes a comprehensive set of tools and specifications for the entire application development lifecycle.
- application deployment, lifecycle management, service dependency management, security, etc.
- Interaction with Cloud Foundry is facilitated through the CF command line interface (CF CLI), allowing for extensive automation via scripting.
- Applications can be developed using open standards with Java, Node.js, and Python build packs provided by SAP, or with community build packs for languages such as PHP, Ruby, or Go.

**Kyma Environment:**
- a fully managed Kubernetes runtime, based on the open-source Kyma project.
- open-source, cloud-native platform
- managing application lifecycles, but with a stronger emphasis on containers, container orchestration, and scalability.
- enables developers to extend SAP solutions using serverless functions and integrate these with containerized microservices.
- supports the deployment of microservices and the development of full-stack applications.

**ABAP Environment:**
- primarily designed for creating extension applications for ABAP-based products like SAP S/4HANA Cloud
- also allows for the development of standalone cloud applications
- cloud-enabled environment operating within the Cloud Foundry or Kyma environments and is based on the latest ABAP platform cloud release, used for SAP S/4HANA Cloud.
- includes familiar components from the standalone Application Server ABAP, and supports the ABAP RESTful Application Programming Model (RAP), SAP Fiori, and Core Data Services (CDS).


### SAP BTP Cockpit
- serves as the primary user interface for managing and administering SAP BTP accounts.
- https://<region>.cockpit.btp.cloud.sap   (Region can be eu10, us10, ap10, etc.)
- For managing the Cloud Foundry environment, you can use the SAP BTP cockpit or the Cloud Foundry command-line interface: cf cli.
- To manage the Kyma environment, you can either use the Kyma Dashboard or the Kubernetes CLI tool, kubectl.
- To work with the ABAP environment, you need to use Kyma or Cloud Foundry and, on top of that, you could subscribe to the Web access for ABAP service to get an administrative SAP Fiori Launchpad for the ABAP environment.

### Services in SAP BTP
- Many capabilities on SAP BTP are offered as services.
- Some are free, while others require additional payment.
- To use a service, you must either subscribe to it or create an instance of it. (instantiated or subscribed)
- Before doing so, it's essential to understand the available service plans to choose the one that best fits your needs.
- **Instance:** Service instances provide interface based access to capabilities (sometimes a user interface when created in an environment).
  - A service instance represents a set of capabilities that are consumed via APIs and/or bindings.
  - Some services also require an additional environment, such as Cloud Foundry or Kyma, to function correctly.
  - These environments provide the necessary runtime support for the service.
  - In cases where the service involves a graphical application or user interface, an additional environment is definitely required, as service instances themselves do not have a built-in runtime.
  - This environment ensures the service has the infrastructure needed to run and be accessed by users or other applications.
- **Subscription:** Subscriptions provide capabilities through a graphical application running in it's own environment - no additional environment is required.
  - A service subscription operates independently without the need for an additional runtime environment or other services.
  - These services typically include an application that can be directly accessed and used.
  - You can leverage the features of this application to support your specific scenarios, making service subscriptions a straightforward option for functionality that doesn't require further infrastructure setup.

#### Example Use of Services on SAP BTP
![image](https://github.com/user-attachments/assets/2ac30a1a-907f-403d-a051-992c07b4313e)

In the example use case for SAP BTP services, the following steps are outlined for developing and deploying a SAPUI5 application using SAP BTP tools:
- **Development Tools:** The developers use ***SAP Business Application Studio*** as the integrated development environment (IDE) to build the SAPUI5 application.They develop the application using the ***SAP Cloud Application Programming Model (CAP)***, a framework to develop services and applications efficiently.
- **Deployment and Hosting:** The application is deployed in the ***Cloud Foundry Environment*** on SAP BTP, which provides the runtime for hosting the application.
- **Data Storage:** The application stores its data using ***SAP HANA Cloud***, a database-as-a-service offering on SAP BTP.
- **Continuous Integration and Delivery (CI/CD):** For setting up automated build, test, and deployment pipelines, the developers use the ***Continuous Integration & Delivery service*** provided by SAP BTP.
- **Security and Authorization:** To manage user authentication and authorization, the application is integrated with ***Authorization and Trust Management*** service, ensuring secure access control.
- **Logging and Monitoring:** The application is connected to the ***Application Logging Service***, enabling developers to monitor application logs for operational insights and troubleshooting.
- **Handling Load Dynamically:** To ensure the application scales dynamically based on traffic or resource demands, the developers use the ***Application Autoscaler*** service. They configure scaling rules and bind it to the application to manage load fluctuations automatically.

This combination of services demonstrates how SAP BTP offers a full-stack platform for building, deploying, and managing applications while ensuring security, scalability, and operational efficiency.

#### SAP Discovery Center
Key Capabilities:
- **Service Catalog:** Provides comprehensive information about out-of-the-box services, tools, APIs, and applications that assist in integrating and extending SAP solutions.
- **Mission Catalog:** Contains ready-to-run projects offering real, actionable support for implementation, helping teams accelerate their project progress.
- **Learning Materials & Step-by-Step Guidance:** Includes educational content and detailed instructions to assist users in navigating and utilizing SAP tools effectively.
- **Dedicated Coaches & Community Integration:** Offers access to dedicated coaches for personalized assistance and includes integration with the SAP Community for knowledge sharing and collaboration.

Benefits:
- **On-Demand Material and Support:** Users have access to relevant resources whenever needed, ensuring they can find the right tools and guidance on demand.
- **Accelerates Innovation:** By providing pre-configured solutions and support, the platform enables organizations to innovate faster and implement new solutions quickly.
- **Low-Touch Enablement:** Offers a self-service online tool, enabling users to independently explore, learn, and implement solutions with minimal direct intervention.


### Connectivity in SAP BTP
**SAP Connectivity Service:**
- Provides a connectivity proxy to access on-premise resources via the Cloud Connector.
- Offers secure connectivity from SAP BTP to on-premise systems, ensuring encrypted communication.

**SAP Destination Service:**
- Retrieves and stores the technical details required to connect an application to a remote service, whether it’s through the internet or the Cloud Connector.
- Manages connections to remote services by specifying destinations with defined parameters, enabling applications to interact with external resources.

**Cloud Connector:**
- Acts as a bridge between SAP on-premise backends (or supported non-SAP systems) and SAP BTP subaccounts.
- Creates a bidirectional encrypted tunnel, ensuring secure communication between on-premise systems and the cloud.
- Simplifies setup and provides a clear configuration of shared systems, allowing selective exposure of on-premise resources without revealing the full internal landscape.
- Key Features:
  - ***Reverse Invoke Proxy:*** Allows SAP BTP to securely access on-premise resources.
  - ***High Availability:*** Cloud Connector can be configured for high availability to avoid it becoming a single point of failure.
  - ***Monitoring & Alerting:*** Provides options for monitoring and setting up alerts to ensure connectivity is reliable and uninterrupted.
- Usage of the Cloud Connector:
  - Setup: Install and configure the Cloud Connector within your on-premise landscape.
  - Define Shared Resources: Configure which on-premise system resources will be accessible through the Cloud Connector.
  - Consume Destinations: Access these shared resources from SAP BTP using the Destination service, which manages the technical information for remote connections.

#### Connectivity Types
![image](https://github.com/user-attachments/assets/3cbb8fb0-9208-4fc0-ba65-5f9760776662)

In general, there are two primary types of connections to and from SAP BTP:
- **Internet Connectivity:** This type is used when accessing capabilities or data from resources available on the internet. It typically employs HTTPS for secure communication.
- **Cloud to On-Premise Connectivity:** This is utilized to leverage existing resources within your on-premise landscape. It requires the Cloud Connector to establish a secure connection, facilitating bi-directional communication between the cloud and on-premise systems.

Both connection types enable seamless integration and interaction with various resources, enhancing the overall functionality of SAP BTP.

# SAP BTP: Application Development and Automation
## Overview
### Application Development Overview
![image](https://github.com/user-attachments/assets/18317854-18ba-46e2-aa93-bf8eaf840231)

SAP advises maintaining a clean core in software and utilizing extensions rather than modifications. This approach encourages the adoption of new custom development concepts to enhance your software portfolio. The application development capabilities of SAP BTP provide a suite of solutions designed to simplify the creation of application extensions or custom applications. While these tools are optimized for SAP applications, they also support the extension of third-party applications.

SAP offers a diverse range of tools and frameworks for both frontend and backend developers. Additionally, there are tools available for low-code or even no-code development experiences. This comprehensive toolset enables the creation of a unified user experience for end-users.

### Automation Overview
![image](https://github.com/user-attachments/assets/753e416b-9e6a-4c1d-88ce-9b340b1143c5)

To automate your business processes for greater agility and reduced manual tasks, the automation capabilities of SAP BTP can be invaluable. These capabilities allow you to build easily, automate swiftly, and enhance agility through visual drag-and-drop tools and prebuilt, industry-specific content.

## Low-Code/No-Code with SAP Build
- No-code development is primarily intended to help employees that are process experts to automate tasks, build applications, or otherwise optimize their own business activities.
- Professional developers use no-code tools to accelerate their basic development work so that they can focus on more complicated concepts.
- Low-code development is designed to allow employees with software knowledge, such as process development experts and professional developers, to build and integrate end-user processes and applications, and to create WYSIWYG (What You See Is What You Get) building blocks for no-code development.
- With SAP Build, you can create apps, automate processes, and design unified experiences using simple drag-and-drop tools. This empowers citizen developers to contribute to your development and automation projects. SAP Build enables you to build visually, integrate effortlessly, and collaborate efficiently.

![image](https://github.com/user-attachments/assets/dea0753b-521c-43f6-b429-2955bf9a5275)

SAP Build comprises three key components for creating no-code projects:
- **SAP Build Apps:** unique development experience, enabling rapid innovation through a user-friendly interface for building customized apps on top of SAP solutions.
  - With drag-and-drop functionality, users can design UIs using a consistently updated component library, requiring no developer experience.
  - It allows for creating logic with visual flow functions and supports individual styling and advanced theming, ensuring a seamless user experience across web, iOS, and Android platforms.
  - Data binding is straightforward through OData and REST APIs, and data processing is efficient with over 500 predefined functions and formulas for calculations, text formatting, and dynamic styles.
- **SAP Build Process Automation:** enables organizations to automate workflows and processes visually.
  - Citizen developers can easily build and enhance business processes with minimal IT support, utilizing no-code features.
  - User experience is enriched with capabilities like the process and forms builders, both featuring drag-and-drop functionalities.
  - Advanced workflow management tools, including business rules, process visibility, and AI, are also integrated.
  - Embedded robotic process automation and reusable components like bots for a comprehensive solution combining workflow and process automation.
- **SAP Build Work Zone:** serves as a centralized hub for accessing relevant business applications, processes, and communication.
  - create digital workplace solutions with drag-and-drop simplicity, enhancing productivity and engagement.
  - unified, intelligent, and personalized work experience, integrating SAP applications, third-party services like SharePoint Online and Microsoft Teams, and custom applications developed with SAP Build Apps or Process Automation.
  - Administrators and users have various options to quickly share and find information, collaborate through blogs, multimedia, surveys, wiki pages, and more.

## Development Tools and Frameworks
### SAP Business Application Studio (BAS)
- New development environment offering a modern, flexible, and extensible platform for building applications that meet the needs of today's enterprises.
- modern environment specifically designed for business application development, used to develop application extensions on the SAP BTP.
- a unified development experience for both professional and citizen developers, regardless of the devices or operating systems they use.
- accessible via a web browser, it retains the familiar feel of desktop tools like Microsoft Visual Studio Code.
- By subscribing to this service in your SAP BTP subaccount, you gain access to a comprehensive development environment that includes optimized editors, terminal access, debuggers, and command line functionality tailored for various use cases.
- predefined roles for developers, extension developers, and administrators.
- ***Dev Spaces:*** isolated environments equipped with specialized tools and pre-installed runtimes.
- These spaces simplify and expedite the setup process for different application types, such as SAP Fiori, Full Stack Cloud Applications, and SAP HANA Native Applications.
- enhance your environment with extra extensions from the Open VSX Registry, reflecting its open-source nature.
- supports low-code and no-code development, allowing users to model CDS models through a graphical editor or create SAP Fiori Elements applications via guided procedures.

![image](https://github.com/user-attachments/assets/afc35421-0e41-4d52-95f5-7f78f0d57d34)
![image](https://github.com/user-attachments/assets/6bd19699-78f6-4325-8679-de38e33ffecd)

### ABAP Development Tools
- The ABAP Development Tools (ADT) are a set of tools for ABAP programming built on the Eclipse IDE.
- They can be used for ABAP programming for on-premise systems and for coding in the ABAP environment of SAP BTP.
- Allow ABAP developers to carry out development tasks utilizing the features of the ABAP application server in an Eclipse-based integrated development environment (IDE).

### SAP BTP Cockpit
- The SAP BTP cockpit is the main hub for cloud development, including deployment and administrative tasks.
- It is the preferred tool for all operational and administration-related activities.
- Developers use it to deploy applications on SAP BTP or integrate services provided by SAP BTP into their applications.
- Numerous services are beneficial for software development, such as:
  - SAP Business Application Studio
  - SAP HANA Cloud
  - Cloud Transport Management
  - Feature Flags Service
  - And many others
- The SAP BTP cockpit is a key tool for administrators.

### Development Frameworks from SAP
**SAP UI Development Toolkit for HTML5 (SAPUI5):**
- SAPUI5 is built on the Model-View-Controller (MVC) design principle and provides a modern, flexible framework for developing web applications tailored to business requirements.
- It includes tools for planning, testing SAPUI5 apps, managing icons, and more.

**Java and Spring:** 
- Using the Cloud Foundry or Kyma runtime, you can develop and run Java-based software projects directly on SAP BTP, ensuring easy integration with your enterprise systems.
- These applications can also consume SAP BTP services. Furthermore, frameworks such as Spring and the SAP Cloud Application Programming Model can be utilized.

**SAP Cloud Application Programming Model:** 
- This is a comprehensive set of languages, libraries, and tools for creating enterprise applications, centered around a domain model powered by SAP HANA Core Data Services (CDS).
- It supports both service and application development, allowing integration with SAP Fiori projects.
- The SAP Cloud Application Programming Model is flexible, supporting both Node.js and Java stacks.

**SAP Fiori User Experience:** 
- SAP Fiori design system includes design languages for different technologies such as web, native mobile, and conversational platforms.
- Each design language defines visual styles, controls, layouts, and common functions, and includes guidelines and resources for developers and designers.
- SAP Fiori can be developed using various technologies, with SAPUI5 as the main HTML5 reference.
- Native mobile languages are available for iOS and Android.

**SAP's Mobile Development Tools:** <br>
To create mobile applications, SAP offers a range of technologies:
- ***SAP Mobile Development Kit (MDK):*** Create multi-channel apps with JavaScript, which can be converted into native apps for iOS, Android, or web.
- ***SAP BTP SDK for iOS:*** Swift-based development of native apps for iOS, with extensions for reusable SAP content.
- ***SAP BTP SDK for Android:*** Android Studio-based development of native Android apps, with support for tools like SAP Fiori Guidelines for Android and the SAP BTP SDK Wizard.

**ABAP RESTful Application Programming Model:**
- This model allows developers to efficiently create SAP HANA-optimized, enterprise-ready OData-based Fiori UI services and Web APIs, both in the cloud and on-premise.
- It leverages technologies like ABAP Core Data Services (CDS) for rich data models, OData services for service model infrastructure, and ABAP-based application services for custom logic, alongside SAPUI5-based user interfaces.


## Continuous Integration, Delivery and Deployment
A key goal in software development is to automate as many steps as possible to reduce manual effort. With continuous concepts, there are various ways to achieve this.

**Continuous Integration:**
- The different types of Continuous X are not isolated but build on each other, with Continuous Integration as the foundation.
- It involves several principles and ensures that a stable build is always available.
- Continuous Integration merges code changes into a single software project, triggering automated tests and builds from this unified codebase.

**Continuous Delivery:**
- Building on Continuous Integration, Continuous Delivery ensures the software is always ready for deployment to production.
- Deployment can either be manually triggered (e.g., by pressing a button) or automatically following a deliberate action (e.g., after committing changes to the main version control line).
- Key points about Continuous Delivery:
  - The software is always ready for deployment to production.
  - A human decision triggers deployment to production.
  - Feedback from production is quickly integrated into the team's backlog.

**Continuous Deployment:**
- Extending Continuous Delivery, Continuous Deployment means that each code change triggers an automatic deployment to production.
- It's important to note that the distinction between Continuous Delivery and Continuous Deployment is sometimes blurred, so it's essential to clarify these terms in discussions about CI/CD.
- In Continuous Deployment, the deployment to production is automated, unlike the manual trigger used in Continuous Delivery.

### CI/CD Pipeline
![image](https://github.com/user-attachments/assets/cdb5de84-32aa-41fd-a692-4186a2e4ae23)

- A pipeline, at its core, is a sequence of activities executed in a predefined order.
- Continuous Integration, Continuous Delivery, and Continuous Deployment together form the CI/CD pipeline, with the aim of maximizing automation in software development and minimizing manual tasks.
- By combining all these components, you can establish a fully automated pipeline to build, test, and deploy your application.
- In summary, Continuous Integration (CI) involves adopting agile principles, while Continuous Delivery/Deployment (CD) combines agile techniques with a robust delivery process.
- The objective is to validate every change (commit), ideally through automation, to ensure reliable delivery.


# SAP BTP: Integration
## API
- Application Programming Interface
- mediator (represented by a piece of software) between applications/websites and you as a user
- they are omnipresent and enable users and developers to focus on "what" needs to be done and not "how".
- separate communication from the task. If a service communicates through an API, the user (or consumer) of the API is entirely focused on the features the API provides. The user only uses the API’s features without thinking about the job itself. The focus is based on the request and the result (response) and nothing else.
- Benefits of APIs
  - Easier and faster to integrate
  - More profitable & cost efficient with increased efficiency & innovation
  - Automation
  - Standardized interfaces enable faster and easier integration of existing and new systems
  - Opportunity to create business processes; Less development and maintenance of the interfaces lead to lower costs
  - Lower human input and easier workflow updates

![image](https://github.com/user-attachments/assets/6dc88535-86b8-4f79-a9fc-9b917e56cd7c)

![image](https://github.com/user-attachments/assets/b934c6ed-bc26-4ce2-873a-eb1b85582657)

For REST APIs, CRUD verbs:
| CRUD   | REST        |
|:-------|:------------|
| READ	 | GET         |
| CREATE | POST        |
| UPDATE | PUT / PATCH |
| DELETE | DELETE      |

![image](https://github.com/user-attachments/assets/0228be09-73af-4adb-929f-a1aed30f8ba4)


## SAP Business Accelerator Hub
- offers a comprehensive collection of sandbox APIs for various SAP products
- These sandbox APIs allow developers to build extensions, applications, or integrations and test them using provided testing data.
- The process is simplified by the use of API keys, which you can obtain by logging in with your SAP ID account and selecting Show API Key on the specific API's page.
- To access the SAP Business Accelerator Hub, visit: https://api.sap.com/.
- explore APIs, browse through API references, view schemas, and even try the APIs directly on the platform.


## SAP Integration Suite

![image](https://github.com/user-attachments/assets/c167db58-e284-46e1-9634-610110be3624)

- integration platform as a service (iPaaS)
- integrate on-premise and cloud-based applications and processes with tools and pre-built content managed by SAP.

### Core Capabilities

#### Cloud Integration
- for hybrid and cloud application integration, seamless data exchange across systems
- web interface with pre-built templates for SAP and non-SAP scenarios
- supports Application-to-Application (A2A) and Business-to-Business/Business-to-Government (B2B/B2G) integrations
- hosted on secure cloud infrastructure, it ensures high availability and a strong focus on security.
- provides prepackaged integration content to accelerate project initiation, allowing quick productivity while accommodating custom requirements.
- facilitates integration with business networks across a broad ecosystem.

#### API Management
- Design your APIs using open standards such as the OpenAPI specification and OData.
- Create APIs by exposing and combining backend interfaces from applications or middleware.
- Safeguard your APIs against security risks, control traffic, and optimize performance with over 40 built-in policies, including edge caching.
- Track and analyze API usage, performance metrics, and errors.
- Collaborate with application developers and generate revenue by monetizing your digital assets through APIs.

#### Open Connectors
- Pre-built connectors for over 170 non-SAP applications.
- Choose the connectors you require and authenticate via providers.
- Develop custom connectors with standardized features such as authentication, pagination, error handling, and search functionality.

#### Integration Advisor
- Proposal service utilizing a machine learning approach.
- Crowdsource-based learnings.
- Automatically generates documentation and runtime artifacts.
- Facilitates community collaboration for developing and maintaining customized integration interfaces and mappings.


# SAP BTP: Data and Analytics

![image](https://github.com/user-attachments/assets/8651a3fb-d50b-4578-b9cb-811b6b7984b8)

## Data-to-Value
- The SAP Business Technology Platform offers a unified persistence strategy for all data-driven innovations, enabling enterprises to transform data into value.
- Across your organization, data is stored in multiple locations, and certain use cases require robust database capabilities. However, data alone holds no value unless it's properly stored, integrated, modeled, shared, and analyzed.
- SAP BTP provides the essential building blocks to address these needs with capabilities for data storage, management, warehousing, analytics, and enterprise planning through a comprehensive solution portfolio, including SAP HANA Cloud, SAP Data Intelligence, SAP Datasphere, and SAP Analytics Cloud.
- **Database:** Storing and integrating your data through SAP BTP and database-as-a-service offerings like SAP HANA Cloud or others.
- **Data Management & Data Warehousing:** Managing and modeling your data through data management and data warehousing capabilities from SAP BTP and start utilizing offerings like SAP Data Intelligence, SAP Datasphere, Modelling with SAP HANA Cloud and SAP Master Data Governance Cloud.
- **Analytics & Planning:** Accelerate your enterprise planning and gather a value out of your data and start utilizing capabilities from SAP Analytics Cloud.

### SAP HANA Cloud
- SAP HANA Cloud is a fully managed in-memory multi-tier cloud database as a service (DBaaS).
- As the cloud-based data foundation for SAP Business Technology Platform, SAP HANA Cloud integrates data from across the enterprise, enabling faster decisions based on live data.
- SAP HANA Cloud is one of the four pillars of the SAP Business Technology Platform and provides the data services to handle constantly growing data volumes in central place.
- The SAP BTP offers SAP HANA Cloud as the strategic database of choice.
- You can also enhance your SAP HANA Cloud with data lake capabilities.
- You can also utilize things like SAP ASE as a service or other services like an Object Store service.
- **Multi-Service Database:** Combining the known SAP HANA qualities like in-memory, multi-model, hybrid transaction, and analytics processing in real-time with high volume and extreme transactionally focused services.
- **Data on Demand:** All data, regardless of size, category, and complexity, available to you whenever you need it.
- **Easy Integration:** A unified access layer to simplify data processing while consolidating and harmonizing data integration to your intelligent applications.
- **Power of the Cloud:** Cloud qualities like low TCO, elasticity, serverless principles, high availability, resilience, and autonomous behavior.
- **Streamlined Access:** Simplified data-access, which connects all your information without demanding that all data be loaded into a single storage solution.
- **Developer Experience:** SAP HANA Cloud provides an integrated development environment in which the developer can develop and model custom applications.
- Here are some examples of where SAP HANA Cloud can be used:
  - ***Next-Generation Applications:*** SAP HANA Cloud serves as the database for modern applications that require high-speed performance and the ability to manage vast amounts of data efficiently and at scale.
  - ***Data Warehouses and Analytics:*** It powers data warehouses, such as SAP Datasphere and custom-built solutions. Additionally, SAP HANA Cloud enables advanced analytics by connecting and integrating distributed data into a unified, consistent data model, supporting tools like SAP Analytics Cloud.
  - ***On-Premise Application Extensions:*** SAP HANA Cloud can extend on-premise applications by offering additional storage and processing power. This is particularly useful when scaling to accommodate large volumes of new users.
  - ***Cloud-Based SAP Application Extensions:*** It allows you to enhance the functionality of existing SAP applications by integrating cloud-based services for greater flexibility and expanded capabilities.

### SAP BTP Data Services
Almost any type of cloud application can be developed and operated on SAP Business Technology Platform (BTP). Besides leveraging the powerful SAP HANA in-memory database, SAP BTP also offers various data services like Object Store, Redis, hyperscaler options, and PostgreSQL service:
- **Object Store:** The Object Store service allows you to store and manage objects (creation, upload, download, and deletion). This service is tied to the IaaS layer, supporting platforms like Azure Blob Storage, Amazon Web Services (AWS), and Google Cloud Platform.
- **PostgreSQL, Hyperscaler Option:** This is a managed relational database service based on native PostgreSQL offerings from hyperscale providers such as AWS and Microsoft Azure. It enables you to provision and manage PostgreSQL databases (like AWS RDS PostgreSQL or Azure Database for PostgreSQL) on hyperscalers and integrate them with your applications running on SAP BTP’s Cloud Foundry environment.
- **Redis on SAP BTP, Hyperscaler Option:** This provides a managed in-memory data store service based on Redis, hosted by hyperscalers like AWS and Microsoft Azure. You can provision and manage Redis cache instances (e.g., AWS ElastiCache for Redis or Azure Cache for Redis) and bind them to business applications running on SAP BTP’s Cloud Foundry environment.

## Data Management and Data Warehousing
### SAP HANA Cloud Modeling
![image](https://github.com/user-attachments/assets/ae980220-e0fc-4f72-9163-aae43677f5a9)

Traditional databases primarily offered storage capabilities with limited data processing, requiring applications to retrieve raw data and handle complex data processing using application code, such as ABAP or Java. This approach placed the processing burden on the application server.

In contrast, SAP HANA Cloud provides not only advanced multitier data storage but also sophisticated data processing capabilities. Instead of applications retrieving raw data, they can now request processed information directly from the SAP HANA Cloud database. Data processing is shifted from the application layer to the in-memory SAP HANA Cloud database, making processing faster and applications leaner. This agility results in less complex applications, as they no longer need to manage the data processing logic themselves.

SAP HANA Cloud uses calculation views as a data processing layer built on top of tables. These views are typically stacked, where lower calculation views define the basic data structure, and higher ones add calculations and semantics until ready for consumption. Calculation views are dynamic, calculating results on-the-fly using live data from either local SAP HANA Cloud tables or remote tables from other databases, without persisting the processed data.

With SAP HANA Cloud, you can combine any type of data: text, geometries, IoT data, and so on, to create multi-models that power high-performance, advanced analytics.

- **Predictive:** Develop predictive models using in-built algorithms including machine learning.
- **Graph:** Store and query highly networked data models such as supply chains or online communities (for example, LinkedIn contacts).
- **Hierarchy:** Query hierarchies to extract valuable semantics such as ancestors, dependents, distance between nodes, or siblings.
- **Spatial:** Store and query geometric data to add spatial information to analytics such as mapping.

### SAP Datasphere
SAP Datasphere, previously known as SAP Data Warehouse Cloud, is a comprehensive data service built on the SAP Business Technology Platform and serves as the foundation for a business data fabric. It allows organizations to provide meaningful data to any consumer while maintaining business context and logic.

SAP Datasphere embodies the concept of a business data fabric—a data management architecture that focuses on creating an integrated, semantically rich data layer across diverse data landscapes. This enables seamless, scalable data access without the need for duplication. It unifies key capabilities such as data integration, cataloging, semantic modeling, data warehousing, data federation, and data virtualization.

With SAP Datasphere, organizations can:
- ***Access authoritative data:*** Deliver data in its full business context, easily model business processes, and maintain governance throughout the data lifecycle.
- ***Enrich all data projects:*** Virtually access or physically store data from any source, collaborate with trusted data partners, and integrate with leading data and AI platforms.
- ***Simplify the data landscape:*** Leverage hybrid architectures, enable self-service data access, and integrate with existing SAP BW models and transformations.

- Self-service data access -> Virtual data products
- Data discovery -> Business content, data marketplace, recommendations
- Orchestration -> Data transformation and data ops
- Processing and persistency -> Warehousing, business semantics (analytic/relational models), knowledge graph
- Data governance -> Metadata management, catalog, lineage, privacy, data quality
- Data ingestion -> Data replication, data federation, real-time data, application integration

### Enterprise Planning and Analytics with SAP Analytics Cloud
- With SAP Analytics Cloud, enterprises can leverage their data to gain insights and enhance planning processes, ultimately improving decision-making. 
- Over time, data analysis has transitioned from being IT-driven to empowering business users to conduct self-service analysis.
- SAP Analytics Cloud (SAC) continues this evolution by providing a cloud-based, self-service business intelligence solution with integrated planning and augmented capabilities.
- SAC connects people, data, and ideas, enabling rapid and informed decisions.
- It can access on-premise analytics, including SAP BusinessObjects BI and third-party solutions.
- Being cloud-based, SAC allows users to work on it via a browser or mobile device with proper access.
- The platform's key capabilities can be grouped into three areas:
  - ***Business Intelligence (BI) & Augmented Analytics:*** SAC offers various tools for data analysis, reporting, and summarizing, such as Analytics Hubs, Digital Boardroom, Smart Insights, and Smart Predict. With augmented analytics powered by AI and machine learning, users can automatically uncover insights, simulate scenarios, and predict future outcomes. Integration with Microsoft Office or Microsoft 365 is also available.
  - ***Planning:*** SAC's planning capabilities allow for rapid, accurate planning, budgeting, forecasting, and reporting. Features like Data Actions automate forecasts, and Value Driver Trees simulate business impacts. Private versions enable collaboration through what-if analysis.
  - ***Collaboration:*** SAC's collaboration tools enhance teamwork, regardless of location, with features like context-based chat, data approval simulations, and notifications, simplifying the collective decision-making process.


# SAP BTP: Artificial Intelligence (AI)

![image](https://github.com/user-attachments/assets/8b435407-a6a7-4102-a5ff-c4cb4d356161)

## AI integrated into business processes and solutions







