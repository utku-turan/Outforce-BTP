# SAP Build Work Zone
- runs on SAP BTP.
- application-centric launchpad experience
- SAP and third-party business applications from both cloud and on-premises deployments
- WYSIWYG page editor with a grid-based layout and a selection of pre-built widgets and custom cards for creating modern workspaces, or "home" pages, for different personas and use cases.
- A set of tightly interwoven features for enabling use cases around user-generated (web) content, communications, and engagement, including:
    - User-managed workspaces
    - Discussion forums
    - Knowledge bases or news feeds

*Default Components*:
- Based on SAP BTP.
- Integrated out of the box.
- Provide platform-level capabilities, such as central identity and access management across SAP solutions.
- Provide functionality to create customized themes to adjust look and feel.

*Optional Integrations*: 
- Based on your use cases and requirements.
- Optionally add several integration scenarios that don’t come pre-integrated; these include SAP as well as third-party products.
- An example for such an optional integration scenario would be building your own chatbot leveraging SAP Conversational AI.
- From a commercial perspective, such services are not included when you buy SAP Build Work Zone, nor are they required for deploying it.


## Editions
> - *Standard Edition* allows you to create an (SAP) application-centric entry point, providing a harmonized user experience layer that integrates applications, tasks, and notifications. The setup and configuration process provides an IT administrator-centric experience, allowing for flexible role-based setups. The setup and configuration process provides an IT administrator-centric experience, allowing for flexible role-based setups.
> - *Advanced Edition* offers additional features, such as powerful page-building and content-authoring tools, interactive workspaces, and the ability to blend business data with structured and unstructured information. Application-centric experience with web content, documents and knowledge sharing as well as user engagement in discussion forums, feeds, etc. are also additional capabilities of Advanced Edition. It empowers administrators, citizen developers and end users alike to contribute and create engaging, modern experiences.

## Capabilities
Here are the slides from SAP that displays the capabilities of SAP Build Work Zone:<br>
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/6d821a6f-eb10-4917-a924-fdb2108183e2) <br>
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/8e1b32d7-de3a-4042-88f6-1271b9afa15e) <br>

- Provide a contextual and uniform digital experience that enables individuals to conveniently access all necessary resources from a unified location, eliminating the need for inefficiently switching between multiple applications or screens.
- Empower users to personalize their digital workspace effortlessly through drag-and-drop customization, enhancing it with the resources and workflows required to optimize productivity.
- Expedite the development of new digital interfaces with the assistance of pre-built templates and a page design experience tailored for business users.

## Integration Scenarios and Patterns
The integration scenarios covering both SAP & 3rd business applications in cloud and on-premise deployments can be categorized into the following areas:<br>
- **Business Apps**: SAP Fiori tiles and Common Data Model (CDN) create a central entry-point to all supported (SAP) applications.
- **Central Services**: Central Services provide a unified approval inbox or user authentication and provisioning.
- **APIs and Webhooks**: Comprehensive (mostly) OData-based APIs and Webhooks to support different integration scenarios.
- **Content & Collaboration**: SAP Build Work Zone integrates with Microsoft Teams and SharePoint Online.
- **SAP SuccessFactors**: SAP Build Work Zone supports SAP SuccessFactors integrations, for example, to combine formal and informal learning.
- **Digital Supply Chain**: SAP Integrated Business Planning (IBP) in Supply Chain Management to follow-up on tasks.
- **Other purposes**: On a high level, they cover one or multiple of the following aspects:
    - Allow access to a full application or relevant parts of it within the SAP Build Work Zone experience.
    - Connect to other SAP (often SAP BTP) services in the area of creating a central entry point.
    - Connect SAP Build Work Zone with other solutions available in the IT landscape, for instance, in the area of existing document repositories.
    - Expose SAP Build Work Zone data via secure interfaces to an external system, for instance, to support gamification or advanced analytics scenarios – via ‘push’ & ‘pull’ mechanisms.
    - Integrate with LoB-specific processes where SAP Build Work Zone capabilities help enrich the overall user experience.

## Key Use Cases
- UX Integration
- Enablement & Learning
- Self-services & Support
- SAP Enterprise Portal Transition (SAP DX Services)
- Extensions
- Digital Workplace & Nextgen Portal

## Features
Here are the key features and strengths of of different business site types:<br>
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/58a38873-7bcd-4099-9c0f-7cb323ed6555)<br>
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/d97a635d-4f4e-463d-b0be-ffec365a357e)<br>

## Administrative Areas
It lets you create a dedicated environment for content management and collaboration within a defined scope, like a particular business department such as HR, IT, finance, procurement, and others.<br>
Area administrators have access to a specific, yet essential, set of system-level features, helping to alleviate the workload of IT or central administrators.<br>
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/ca474692-aee0-4558-a9fd-7fdf70a35b2d)<br>

## Homepages
Homepages serve as the default landing page for all users when they access SAP Build Work Zone. They are accessible through either clicking the logo in the menu bar or selecting the global menu entry for "Home."

It's important to note that homepages can vary depending on user personas or roles. Furthermore, they can be directly assigned to different member lists, offering greater flexibility in crafting truly personalized experiences tailored to your intended user personas.

Regardless of the company or department, all homepages share a common grid-based layout structure and a robust "What You See Is What You Get" (WYSIWYG) page editor. This editor is linked to a library of pre-designed widgets that can be seamlessly combined with custom UI integration cards. This allows for the seamless integration of application content with rich text, multimedia, and various forms of structured and unstructured data.

To cater to external stakeholders, such as suppliers or customers, there is a dedicated feature for creating homepages designed specifically for external users. This distinct experience is separate from the design and content of internal user homepages.

![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/e481032c-278b-45d3-97df-4745a0cea629)

## Workspaces
Workspaces serve as crucial components that facilitate various use cases and offer a wide array of features, encompassing content management, forums, and adaptable page design. One of the key strengths of workspaces lies in empowering all system users, including administrators, citizen developers, and regular end users alike. Depending on the system's configuration, any user can create and design workspaces tailored to address specific business challenges.

In SAP Build Work Zone, particularly in the advanced edition, workspaces play a pivotal role, providing an extensive platform for enhancing productivity. They enable you to customize your workspace with flexible page layouts, allowing you to efficiently organize data, implement best practices, and facilitate seamless communication and collaboration with colleagues and teams.

The creation and management of a workspace, including the addition of content, planning tools for project coordination, business applications, cards, widgets, and more, can only be performed by a workspace administrator or a designated workspace member. These privileged users also have the ability to create blog posts, wiki pages, and links. To collaborate with others within a workspace, individuals must join as workspace members. Workspace members can engage in communication through the workspace feed or forums, and they can use workspace pages to share information and content.

While the available features may vary from one workspace to another, there are four primary types that dictate the overall experience: 
- My Workspace
- Public Workspaces
- Private Workspaces
- External Workspaces

![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/ae3e9764-8205-4155-9229-55534c456f4b)
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/cc355e77-71c4-4741-8e6f-7487f7af1df7)
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/11e96133-dc93-480f-8ca1-5b60801ad160)
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/eb8f401f-63cc-4e70-86d0-e142de78caea)
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/4c1b9d3e-7a23-462a-a7ae-e69edb01b704)

## Workpages
Workpages play an important role in SAP Build Work Zone as they combine the different content artifacts into an engaging user-facing experience. They are used in workspaces as well as the default landing page(s) of opening SAP Build Work Zone, the so-called home pages. These are available as the first menu item in the top navigation bar and cannot currently be hidden.

![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/96e7c4c4-4ba7-40c6-8355-67bd413dba86)<br>

### Workpage Types
#### Workspace workpages
It is designed by the person who created the workspace, better known as the workspace administrator. It is the default landing page for the workspace. It is used to display content and feed of the workspace which is shared only by the members of the workspace.

#### My Workspace Workpage
All internal users of SAP Build Work Zone can design their own personal workspace. They can include apps and tools that they need daily. Content created here cannot be shared with or seen by other users.

### Sections
#### Feed Updates Section
When facilitating user interaction is a primary objective, the feed update section can be activated to offer a time-sequenced feed display of comments, posts, and various user activities within a workspace. Workspace members have the capability to share a diverse range of content, including documents, blogs, videos, and images. Additionally, they can interact with other workspace members through @mentions and employ tags within the feed to assist fellow members in locating their posts.<br>
It's noteworthy that feed items can also be generated beyond the confines of the workspace, and if enabled, workspace-level feed items will be visible to users in the company-level and home feeds.<br>

#### Membership Section
The membership section serves as the control center for regulating access to the workspace. This includes tasks such as extending invitations to new members or bestowing administrator privileges within the workspace.<br>

#### Recommendations Section
For a user-friendly means of exploring popular or suggested content within the workspace, the recommendations section has something for everyone.<br>

#### Sub-Workspaces Section
While workspaces, with their distinct sections and the capacity to establish various overview pages, offer effective methods to organize content, the introduction of nested workspaces, referred to as sub-workspaces, enhances flexibility further. This feature supports a single level of sub-workspaces, each with its independent membership, content, and feature management.<br>

#### Content Section
Whether you need to store comprehensive information regarding a specific business process, upload instructional videos, or share a presentation, the content section furnishes the essential functionality for organizing and managing content within a workspace. Content placed here can be conveniently accessed through the content widget on your overview pages, facilitating easy reference.<br>

#### Events Section
The workspace calendar serves as a tool for showcasing events within the current month or disseminating information about upcoming webinars. Members have the flexibility to navigate through the calendar, switch between views such as week, day, or list, configure time zones, set the calendar's first day of the week, and establish new events either manually or via import.

#### Knowledge Base Section
The knowledge base section empowers workspace members to generate and archive knowledge-base articles. Unlike the content section, which primarily deals with uploading externally created content assets, the knowledge base offers a structured approach to disseminate knowledge among your workspace members using forms. It's important to note that if this feature is deactivated after knowledge base articles have been published, these articles will cease to be visible within the workspace.<br>

#### Forum Section
In contrast to the feed section, a workspace's forum(s) section offers a highly organized and in-depth approach to facilitate user interaction. It can be used, for example, to create question and answer pages or to engage in discussions about ideas or topics.<br>

#### Task Section
Within the workspace, a collaborative task management tool is available to catalog current, overdue, and accomplished tasks. This feature proves invaluable when coordinating activities such as planning a new customer event, among other tasks and responsibilities.<br>

### Launchpad
The launchpad offers the following capabilities:
- Integration of applications deployed on SAP S/4HANA on-premise, SAP Business Technology Platform (BTP) in a multi-cloud environment, or the ABAP environment.
- Exposure of content from various content providers, including SAP S/4HANA on-premise, SAP Enterprise Portal, or SAP BTP in a multi-cloud environment.
- Empowerment of individual application widgets and application group widgets for use across both homepages and workspaces, promoting versatility in their deployment.

### UI Integration Cards
You can create and edit pages for your intranet and workspaces with a rich and visual built-in, no-code page editor – you can change and see the results immediately, no development skills required.<br> 
With SAP Build Work Zone, you can set up page access, translate, track changes and versions, and modify layouts with various pre-built widgets including SAP Fiori and UI integration cards.<br> 
UI integration cards can be created someone with more advanced technical skills using low-code or pro-code approaches, and then they can easily be used by citizen developers following the no-code approach to visual programming.<br> 
These cards can surface data from connected SAP and third-party business applications and present the information on the page in various designs and layouts.<br>
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/de0d5c7c-34ec-43ea-b6dc-92efed629b39)<br>

## Extending Work Zone
You can extend SAP Build Work Zone with:
- ***UI Integration Cards***: They are like micro-applications for displaying business critical information from SAP as well as from third-party systems.
- ***Workflows***: leverage SAP BTP Workflow. You can use already-created workflows from SAP Build Process Automation and/or create new ones that are directly accessible from within SAP Build Work Zone.
- ***Guided Experiences*** (Combination of UI Integration Cards and Workflows): The UI Integration Card acts as a wizard-like experience to trigger a workflow in SAP Build Process Automation, providing a unified multi-step experience for the user that connects to different SAP and third-party backend systems.
- ***Launchpad (Shell) plugins***: In case of substantial changes to the SAP Build Work Zone global navigation header. Add icons or other modifications to the header to reference to another application, security/compliance document or other pieces of information – even role-based visibility settings.
- ***Integration with SAP Conversational AI***: to connect to one or multiple chatbots. SAP Build Work Zone users can then interact with the chatbot(s) to address many innovative scenarios for HXM, procurement, or even IT self-service requests (such as requesting system access).

![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/05c3a686-69dd-44f0-859a-9874f7e79297)
