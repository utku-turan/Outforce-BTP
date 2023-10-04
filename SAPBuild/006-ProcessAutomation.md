## SAP Build Process Automation
Low-code and no-code solutions empower business users to automate workflows and processes effortlessly using intuitive drag-and-drop interfaces. Skilled developers can leverage visual tools and pre-existing content to accelerate outcomes and readily adapt to evolving needs. Development tools further enable the creation of intricate workflows and automation, which can be packaged for business users to seamlessly incorporate into their projects and processes.

Another famous slide from SAP:
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/8c03873f-15fd-49c3-8fce-dd8e81ac8416)

You can construct, modify, enhance, and innovate a wide array of business processes with minimal reliance on IT intervention. For instance:<br>
- Streamline labor-intensive, repetitive tasks like data entry into spreadsheets.
- Transform manual and partially automated processes into digital formats, as seen in cases like capital expenditure approvals.
- Automate processes with numerous steps, such as the input of sales order data.
- Automatically consolidate data from multiple systems and update purchase records.
- Customize and expand the predefined workflows of your business applications (whether SAP or non-SAP, on-premise, or cloud-based). This could entail adding multiple tiers of approvals for a sales order.
- Automate end-to-end cross-application workflows spanning multiple systems (e.g., ERP and human resources systems), like those found in employee onboarding processes.

### Product Capabilities
SAP Build Process Automation provides the following product functionalities:
- Intuitive creation of workflows for task automation and streamlined decision-making.
- Utilization of cohesive workflow management through SAP Intelligent Robotic Process Automation.
- Acceleration of projects with readily available content packages derived from optimal use case scenarios.
- Seamless integration with external applications.
- Assurance of risk-free development, eliminating the pitfalls associated with Shadow IT.

> Keywords:
> - Process
> - Advanced Workflow
> - Forms & Multi-step Approvals
> - Business rules & Decisions
> - Document Understanding
> - Unified Launchpad & Task Center
> - Process Visibility & Flexibility
> - Task Automation
> - Pre-built Content

### Working Modes
![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/5d8f7fcb-50f8-4c58-a89d-fca6f24df7db)

**Store:** Import pre-built processes and automations.<br>
**Process Builder:** Build processes and automations from scratch.<br>
**Reuse Workflows** from SAP Workflow Management.<br>
**Reuse Automation projects** from SAP Intelligent Robotic Process Automation<br>
**Hybrid mode** combining pre-packaged, process, automation, and workflow content<br>

### The Store
The Store is a pivotal element in SAP Build Process Automation. It provides ready-made content developed and maintained by SAP, available at no cost. This content encompasses readily deployable packages, comprising templated automations, workflows, processes, process visibility dashboards, forms, and actions.

The Store content is categorized into three Project Types:
- ***Actions:*** to accomplish the integrations. APIs are encapsulated as Actions within Actions projects. You can import pre-configured actions projects from the store.
- ***Process Automation:*** content related to the former SAP iRPA product. Pre-defined automation templates and SDK packages for specific business scenarios.
- ***Live Process:*** content related to the former SAP Workflow Management product. contained artifacts are mostly workflows or processes, business rules and business visibility scenarios. They are mostly pre-defined for a specific business scenario.

Similar to the Process Automation content, when importing Live Process content, you are importing templates that need to be adjusted to your specific needs afterward. In a typical scenario, you will retrieve a **process template**, a **decisions project**, and a **process visibility project**. These artifacts might be complemented by additional material like SAP Cloud Application Programming Model applications. Each of these artifact types can be adjusted to your needs.

## Lobby
Using the Lobby, you have the capability to create, manage, and deploy business processes and action projects that encapsulate APIs as integral components within your business scenarios. The project lists view enables you to assess existing projects or initiate new ones. You can effortlessly refresh, rearrange, filter based on type or collaborators, and execute actions like release, publication, and sharing.

Within the lobby, you have the ability to access and engage with various project capabilities, which encompass the following:
- **Store**: This area provides access to pre-constructed process automation content.
- **Monitor**: Here, you can oversee deployed workflows, automation tasks, and events.
- **Settings**: In this section, you can examine project details that have been deployed and configure agents.
- **My Inbox**: This designated space enables you to manage tasks from both desktop and mobile devices.

A screenshot of the lobby:
![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/784e381e-069a-4c6f-98c1-ec486126b44d)

With an SAP Build Process Automation subscription, you can create and manage three project types:
- ***Business Process Project:*** Create, deploy, automate, and run digital business process by configuring process artifacts. Examples of business process projects include Investment requests, invoice approvals, and sales order approvals.
- ***Task Automation:*** to create and run bots
- ***Actions Project:*** Embed external skills and capabilities into your business process projects by uploading an open API specification file in .json format. Actions projects allow external systems and solutions to communicate with SAP Build Process Automation.

## Using Conditions to Control the Flow
Streamline your process to follow distinct conditional pathways without requiring any coding. These conditions implement an 'If/Else' rule, and the business process adjusts based on the conditions specified in the process's condition settings.<br>

**Decision Capability**: This feature enables you to model and govern intricate business logic in a structured manner that's easy to maintain.<br>
**Policy Concept**: A decision comprises one or more policies, with each policy encompassing a set of rules. These rules serve to automate decision-making aspects within a business process.<br>
**Rule Components**: Once a decision (policy) is established, you formulate your business logic by incorporating rules into the policy or policies.<br>
**Decision Diagram**: A visual representation akin to a flowchart, illustrating the progression of decision logic execution from input to output.<br>
**Decision Table Rule**: A tabular presentation containing input and output role expressions, defining decision logic.<br>
**Text Rule**: A straightforward if-then formatted compilation of rule expressions.<br>

## Create and Configure Decision Logic in the Process
To incorporate a decision, start by *identifying the set of rules* pertinent to the decision-making process. Proceed to *define the applicable data types* essential for formulating these rules. These data types encompass all the required fields crucial for constructing the rules. For instance, if a rule design stipulates "Sales Order Amount greater than 100000," with the corresponding action being to assign the Approver's email as approver(@)test.com, the data types involved would be Sales Order with Amountfield, and Approver withEmailfield.<br>

A *Policy* represents an assortment of rules to be executed in a precise sequence, ensuring they run in the order they're added to the policy. The output of the final rule's execution exclusively serves as the ultimate outcome of the decision.<br>

A *Data type* outlines the structure of data that can serve as input and/or output parameters in automation, decisions, or various steps, activities, skills, processes, scenarios, triggers, or notifiers. Data types facilitate the manipulation and validation of data. While you can manually create a data type, certain data types can also be generated automatically when SDK packages or pre-packaged scenarios are imported or after running an automation.<br>

A *Decision diagram* functions as a visual flowchart outlining the sequence of execution for decision logic, spanning from input to output. Within a decision diagram, you can observe the input, output, policies of a decision, and the rules encompassed within those policies. Furthermore, each component of a decision, such as policies or rules, can be accessed directly via the decision diagram itself.<br>

A *Decision table* assumes the form of a tabular presentation for a rule, with headers designated as *"If" and "Then,"* arranged in row columns. The "If" header columns comprise expressions that undergo evaluation, while the "Then" header columns specify the resulting structure generated post decision execution.<br>

When handling attributes of data objects with the String data type, remember to enclose the text with single quotation marks *(' ')* both before and after.<br>

A *User Group* denotes a collection of roles or a group established within the BTP cockpit or your respective user management system. These groups include users who hold responsibilities for specific tasks. The utility of utilizing groups lies in the flexibility to add or remove users without necessitating modifications to the decision itself.<br>

To ensure a decisive output for all varieties of sales orders, consider adding an additional row to the decision table rule. This supplementary row should return the list of approvers authorized to approve sales orders valued "greater than 100000". For instance, for sales orders originating from defined shipping countries like India, Germany, or the United Kingdom, with a value less than or equal to 100,000, the first row's logic applies. Conversely, for sales orders exceeding 100000 in value, the second row's logic applies. In scenarios not matched by these rows, an empty result is returned.<br>

> [Here](https://education.hana.ondemand.com/education/pub/mmcp/index.html?show=project!PR_EE279D39FC3840A1:demo#TS_5D8AC4879BBB4A488802DA6DD4BEE8E4) is the link to SAP's  demo for creating and configuring Decision Logic in the process.<br>
> And here is the [video]().

## Release, Deploy, Run and Monitor the Process
After you have finished modeling your process with various forms, it is time to run it. Before you can run your process project, you have to first release and deploy it.

- The first step is to *release* a process project which creates a snapshot of its current status and gives it a dedicated version number. If you are releasing your process project for the first time, the version number will be 1.0.0.
- *Deploying* your process project can only be done after its release. The deployment makes it available for others to use. Please note that you cannot edit released or deployed process projects. If you need to make changes to an already released process project and deploy it, you will need to edit the process project and then re-release and re-deploy it.
- *Running* the process will demonstrate that the workflow has been triggered and the approval process project has started. To do this, you have to open the process builder of the deployed version and choose the form to get to the URL which is opened from the web browser.
- Now that your process project is running, we need to follow how well it is working. *Monitoring* business processes is key to successful automation. Using monitoring capabilities, you can proactively and consistently monitor process performance, identify any issues in the process project, and take necessary actions to ensure business process continuity.

### Monitoring
Monitoring business processes is one of the key aspects of successful automation. Using monitoring capabilities, you can proactively and consistently monitor process performance, identify any issues in the process, and take necessary actions to ensure business process continuity.

SAP Build Process Automation provides different applications for monitoring and managing different process skills. The applications include Process and Workflow Instances, Automation Jobs, Acquired Events, and so on. These applications are available under the Monitor tab in Application Development studio.

All deployed processes can be accessed by following Manage → Processes and Workflows application.

**Monitor -> Process and Workflow Instances**<br>
In there, you will see all the running, erroneous, and suspended process instances. Use the filter bar to get a more customized view of the process instances based on different statuses such as running, completed, suspended, terminated, and so on. To explore different process monitoring options, go to the Instances list, and choose your new process instance that was just triggered via the start form.

Observe the process instance information which provides the context for the process. You can see actual process data flowing across different activities in the process, and the execution logs where you can trace how the entire process has been progressing. You can also see some basic runtime information for each activity such activity name, who started it, when was it completed, and so on.

**Monitor -> Automation Jobs**<br>
![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/7cad5b29-bfd3-4567-8077-e3dfe4bafedb)

**Visibility Scenario -> Copy for Dashboard Link**<br>
![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/a9d2261a-1f62-45fd-bc13-2f3dc032e72b)
![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/b2b6ba61-270d-4540-9b4d-7d7b18d2189c)

Open the Visibility Scenario Dashboard by pasting the dashboard link in a browser window. The dashboard is there. The performance indicators are filling up. Depending on the time it has taken, there might be different results. Please now feel free to explore the details and discover what is included in each tile. You could even navigate into single instances.

## Actions
In SAP Build Process Automation, you use Actions to accomplish the integration. Application Programming Interfaces (APIs) from the source and target systems to interact with, are encapsulated as Actions within Actions projects. Those Actions projects are then held in an Actions projects library and from there, can be integrated into the business processes.

![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/6d167c9c-5e8b-4856-a1ce-6ff28cbb54c4)

This approach offers various advantages compared to direct API integration into the respective process:
- There is an abstraction of the API. The process developer does not need to know exactly about technical details of the API.
- APIs can be adjusted to the process developers needs, only exposing endpoints and data that is required or safe to use by the process developers.
- Actions can be configured once, and then be reused across different business process projects.
- Actions projects allow versioning and thus, make it easier to deal with changing process requirements or changing API versions.

As Actions rely on the OpenAPI Specification standard for API definition, they aren't limited to APIs from SAP systems, but provide the option to integrate any API that is or can be described in the OpenAPI Specification. A large number of API definitions, especially for but not limited to SAP solutions, can be found in the SAP Business Accelerator Hub.

The Actions Editor lets you compose multiple Actions from an underlying API into an Actions project. Note that you don't have to include all possible parameters of an API endpoint as parameters in the respective Actions, and you also don't have to include all available response body fields in the response provided through the Action. By that, only information relevant to the business process can be included.

Once your Actions have been defined, the project needs to be released into a version and then published to the Actions library.

![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/156c75a1-b859-400b-b120-77a9547df079)

After APIs have been encapsulated in an Actions project and published to the library, adding them as action to a process is quite simple. Select the corresponding step type Actions and browse the Actions library. Select the action required in your process, and choose Add. Once the Action step is included in your process, make sure to define its parameters:
- **Destination variable:** A process variable that will hold the technical SAP BTP destination name to be used for accessing the underlying API at process runtime. This variable can be filled with a destination name during deployment of the process.
- **Inputs:** Mapping of process content to all parameters, that the action requires in order to be performed (for example, the Sales Order Number, when retrieving a Sales Order entry from an SAP S/4HANA system).
- **Outputs:** Overview of the Actions call result, as defined in the respective action.

In order to use your configured Actions in an SAP Build process, the Actions project needs to be deployed and released to the Library. This procedure gives you governance over which APIs are ready to be used by process developers and which APIs still need refinement.

You and your colleagues are building a process that needs to read Sales Order data from your SAP S/4HANA system and at a later stage, also write Sales Order data back to the system. Now you're faced with the challenge of interacting with that SAP S/4HANA system in the process. As a solution to this challenge, SAP Build Process Automation provides the capability of Actions projects. You have already created an Actions project that encapsulates the Read Sales Order API endpoint of the SAP S/4HANA Sales Order API. Now you want to make use of the Action within a process. For that, you'll use the Action step type. As the process also needs technically to be able to reach the SAP S/4HANA system, a destination will be required too.

When connecting remote systems with your SAP BTP environment, it's vital to create a Destination for them. The Destination acts as sort of a technical address of the system to be connected. Destinations can include additional information such as credentials for access authentication and authorization.

## Using APIs for Integration
### REST APIs
*APIs (Application Programming Interfaces)* define how components can be contacted by other components in order to trigger certain functionality or exchange data.

*A REST API (also RESTful API)* is an API that adheres to the guidelines and constraints defined by the REST architectural style. It particularly puts emphasis on the interaction and communication of such components.

![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/598c6799-60f5-44d2-a0dd-f73c9774dedd)

### Discovering SAP Build Process Automations APIs in SAP Business Accelerator Hub
When entering the SAP API Business Hub and searching for the product SAP Build Process Automation, you'll find the according API package. Following, you find the different APIs it contains, and one example each on how these APIs could be leveraged.

![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/c6dcba01-1e53-47e8-bdc2-5345154835ab)<br>
![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/086879dc-1b50-4311-94aa-4b4245be6790)<br>

### Finding an Endpoint to Use
Let's say you would like to find out how to trigger a new process or workflow instance using the SAP Build Process Automation APIs.

![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/eea806ee-231a-45cd-bf9f-bca5f9282bb6)<br>
![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/ed91a008-c9e8-4e95-bc5d-a48a258ef41a)<br>
![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/77355772-a52c-44e8-a8e4-a41975be2aff)<br>
![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/45992033-8cee-4da0-9465-09e84445662c)<br>


## Robotic Process Automation
Robotic process automation (RPA) is a software technology that makes it easy to build, deploy, and manage software robots that emulate humans actions interacting with digital systems and software.<br>
Automations can expedite your processes and mitigate the risk of errors associated with manual data transfers.<br>

Robotic Process Automation (RPA) accelerates the digital transformation of business processes by automatically replicating tedious actions that have low added value. By bringing Chat Bots into the equation, using APIs rather than just UI elements, and combining Machine Learning (ML) and AI, we can push RPA to the next level, and the journey has just started.

### Business Value of Automations
![image](https://github.com/utku-turan/Outforce-BTP/assets/73386835/e1ddecc0-8394-453e-91d4-ca79f2b0a114)

### Use Cases for Automations
Let's look at some use cases covered by automations in SAP Build Process Automation. These include the following:
- Extracting data using different connectors and putting that data into a finance system
- Searching for invoice numbers in countless ERP instances
- Logging on to multiple SAP ERP Central Component instances, collecting purchase requisitions, and distributing them to shared services

During the course of a working day, users are often unaware of all the simple tasks they complete. Hidden tasks get lost in their daily work. At first you think you only need to automate the boring tasks. However, consider also the short, hidden tasks, where the potential for automation is lower (approximately 50%). These tasks may be performed, for example, 40 times a day or more. If for example, 50 people are doing the same thing, the potential for time saving is significantly higher than the time saving for boring tasks, estimated at approximately 12 full-time equivalents.

There are four main criteria for use cases:
- Manual and repetitive actions
- High volume
- Multiple applications and systems
- Workaround for native integrations (for ex: a legacy application)

### Task Automation
Task automation can run in two ways:
- *Unattended mode*: Bots are working autonomously with human supervision only – there is no human intervention in the part of the process RPA is running.
- *Attended mode*: The attended mode, in which bots will work with humans to assist them, to help the bot.

The ***Automation Editor*** of SAP Build Pro is composed of four main parts: 
- The Toolbar: save, undo, redo, delete, test
- The Workflow: the list of steps inside your automation
- The Right-Side Panel:  add steps, check inputs and outputs, automations, activities, data, controls
- The Console: Design and test console, errors and warnings, variables

### Using the Desktop Agent to run Automations
The Desktop Agent is a component that is installed locally on user desktops. It executes automation projects that launch and run applications of various kinds, reads information from screens, enters data, clicks options, and processes data. Automation projects are assigned to tenants running on the Desktop Agent. You can see what your Desktop Agent is always doing thanks to the convenient menu that is always accessible from your computer’s taskbar while your Desktop Agent is ready or active.

When it’s installed, the Desktop Agent is configured to start at Windows logon by default. The Agent can run in the attended or unattended mode. In the attended mode, you start the automations by clicking on them, and in the unattended mode, the automations run automatically without your intervention.

Using the Desktop Agent, you can perform different actions to run and monitor your projects, such as:
- Run projects
- Manage tenants
- Configure the connection settings
- Change the agent mode
- Monitor the Agent
- Collect and manage traces
