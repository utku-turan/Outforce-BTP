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
