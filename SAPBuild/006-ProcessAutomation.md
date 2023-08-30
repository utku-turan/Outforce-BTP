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

## Lobby
Using the Lobby, you have the capability to create, manage, and deploy business processes and action projects that encapsulate APIs as integral components within your business scenarios. The project lists view enables you to assess existing projects or initiate new ones. You can effortlessly refresh, rearrange, filter based on type or collaborators, and execute actions like release, publication, and sharing.

Within the lobby, you have the ability to access and engage with various project capabilities, which encompass the following:
- **Store**: This area provides access to pre-constructed process automation content.
- **Monitor**: Here, you can oversee deployed workflows, automation tasks, and events.
- **Settings**: In this section, you can examine project details that have been deployed and configure agents.
- **My Inbox**: This designated space enables you to manage tasks from both desktop and mobile devices.

A screenshot of the lobby:


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
