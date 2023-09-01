# What is SAP Build?
SAP Build is SAP's low-code offering built on SAP Business Technology Platform (SAP BTP).<br>
It can be used to create enterprise applications, automate processes, and design business sites with drag-and-drop simplicity.<br>
SAP's Introduction to SAP Build video: https://youtu.be/tOGT7uJed8Y<br>

SAP Build currently has 3 major tools/capabilities:
> - With the help of ***SAP Build Apps***, citizen developers can easily create and deploy front-end applications with custom functionality, stand-alone apps, and even side-by-side extensions to S/4HANA.<br>
> - ***SAP Build Process Automation*** lets business users adapt, improve, and innovate business processes without any coding, and with the ability to connect to SAP Workflow Management, SAP Intelligent Robotic Process Automation , and embedded Al capabilities.<br>
> - ***SAP Build Work Zone*** can be used by IT professionals and business users to build business sites to provide access points to relevant applications, processes, and information.<br>

Here is the famous slide from SAP on SAP Build:<br>
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/1e32ff7b-7a0e-4a39-9fe5-5f20c8aea98b)

## Details of SAP Build
[Here](004-SAPBuildDetails.md) you can find more information on details of SAP Build.

You can also discover plenty of pre-built content packages for SAP Build in the SAP Build Content Catalog: <https://store.build.cloud.sap/store>

## What is Hyperautomation?
Hyperautomation refers to the use of smart technologies to identify and automate as many processes as possible – as quickly as possible. The term hyperautomation describes a *strategy* more than a specific technology. The driving force behind it is the idea that *business processes work better when they are automated*. Automated business processes are faster and more accurate, plus they lend themselves to better tracking and analysis. Essentially, hyperautomation refers to the use of *smart technologies* like robotic process automation (RPA), low-code/no-code (LCNC) platforms, artificial intelligence (AI), and machine learning to identify and automate as many processes as possible – as quickly as possible.

## What is Low-code / No-code development?
***Low-code*** combines traditional programming language-based environment with no-code platforms, suitable for developers with at least basic tech skills.<br>
***No-code*** simplifies by using visual development tools like drag-and-drop, accessible to tech and non-tech users, such as citizen developers.<br>
For details, check [here](002-LCNC.md).

### Developer Types
- Professional developers -> IT professionals building apps or automations faster using SAP Build, with the ability to quickly prototype and test ideas.
- Citizen developers -> Business users using SAP Build to build apps or process automations.

### Governance
Citizen developers will be able to build apps and processes with SAP Build. These apps have to be secure, scalable, and compliant with corporate standards. These developments must be controlled by IT.<br>
Details of [Governance in BTP](003-Governance.md).


# Main tools of SAP Build

## SAP Build Process Automation
***SAP Build Process Automation*** empowers you to create workflows and automate everyday tasks without needing to write code. It offers a streamlined and efficient approach to automating business processes.<br> 
Through its user-friendly, no-code interface, you can seamlessly craft workflow management and robotic process automation (RPA) solutions. These include integrated AI for decision support and document handling, all achieved without the need for coding.<br>

### What is a Business process?
A business process refers to a set of activities that have to be performed to complete an end-to-end business scenario.<br>
For details, check [here](005-BusinessProcess.md).<br>

### Business Process Management
Details of BPM and BPMS from SAP Build perspective can be found [here](005-BusinessProcess.md#business-process-management-bpm).<br>

## SAP Build Process Automation Details
Let's take a look at some important [Topics](006-ProcessAutomation.md) regarding the SAP Build Process Automation Product.
> - [Capabilities](006-ProcessAutomation.md#product-capabilities)
> - [Lobby](006-ProcessAutomation.md#Lobby)
> - [Conditions](006-ProcessAutomation.md#using-conditions-to-control-the-flow)
> - [Decision Logic](006-ProcessAutomation.md#create-and-configure-decision-logic-in-the-process)

### Process Visibility
Uncover the status of your process through the [visibility functionalities](007-ProcessVisibility.md) offered by SAP Build Process Automation.<br>

### Robotic Process Automation
SAP Build RPA is the new product replacing (or rebranding) SAP Intelligent RPA.<br>
You can find some details [here](006-ProcessAutomation.md#robotic-process-automation).<br>

## Hands-on
And, here are the most important hands-on topics of SAP Build Process Automation:<br>

### Interactive Forms
You can use an [interactive form](008-InteractiveForms.md) to trigger a process to start or to add an approval step in the process.<br>

### Automations
> You can check this [step-by-step guide]() on how to create an automation that reads some records from an Excel file and processes according to a condition.<br>

> Next video guides you on how to [register a Desktop agent]().<br>

> And this one shows you how to [run the process]().<br>

> Another example of [Process Automation]<br>


## SAP Build Apps
SAP Build Apps, previously known as *SAP AppGyver*, represents a visual development solution enabling the creation of sophisticated enterprise applications without coding. SAP Build Apps provides the capability to construct both *Web & Mobile Applications*, encompassing front-end user interfaces and event logic, as well as *Application Backends*, which involve back-end data management and server-based logic.

This tool facilitates:
- Visual construction and personalization of enterprise apps. (dragging and dropping pre-built components and then configuring them to your needs.)
- Seamless integration with both SAP and non-SAP systems. (connect to all types of backend data, including SAP systems, via SAP BTP destinations.)
- Create data models and application logic, also by dragging and dropping flow functions and configuring them.
- Promotion of collaborative efforts among fusion teams.
- Learn quickly with in-product guided help and learning modules.

[Additional Info](009-SAPBuildApps.md)
### SAP Build Apps Capabilities
[Capabilities](009-SAPBuildApps.md#Capabilities)
### Using SAP Build Apps
[Here](010-BuildAppsParts.md) you can find information about the parts of the SAP Build Apps tool.<md> 

## Creating an App with SAP Build Apps
[Here](010-BuildAppsParts.md#AppExample) is an example on how to create an app using SAP Build Apps.
Steps:
- Create a new project.
- Create the UI.
- Add some custom logic.
- Connect to an API.
- Fetch data from the API.
- Display data from the API.


### Extending an App with an API
### Developing a No-Code Extension With SAP Build Apps

## SAP Build Work Zone
### What is SAP Build Work Zone?
### Work Zone Editions
### Work Zone Capabilities and Use cases
### Integration scenarios and Patterns

## SAP Build Work Zone Features
### Administrative Areas
### Homepages
### Workspaces
### Workpages
### Extending Work Zone

## Continue your SAP Build Learning Journey

### Discover Use cases for LCNC Apps and Automations

### Maturity of Automations

### Pre-built Content

## Training materials on SAP Build
> Beginner<br>
<https://learning.sap.com/learning-journey/utilize-sap-build-for-low-code-no-code-applications-and-automations-for-citizen-developers><br>
> Advanced<br>
<https://learning.sap.com/learning-journey/compose-and-automate-with-sap-build-the-no-code-way><br>
<https://learning.sap.com/learning-journey/create-processes-and-automations-with-sap-build-process-automation><br>
<https://learning.sap.com/learning-journey/develop-apps-with-sap-build-apps-using-drag-and-drop-simplicity><br>
> Tutorials<br>
<https://developers.sap.com/tutorial-navigator.html?tag=software-product%3Atechnology-platform%2Fsap-build%2Fsap-build-apps-enterprise-edition><br>
> Additional resources<br>
[AppGyver No-Code Academy](https://youtube.com/playlist?list=PLV9VMatP3XOjMgp84HLgiia_xGJzyqSKn)<br>
[SAP Build App Programming 101](https://youtube.com/playlist?list=PLV9VMatP3XOhlq34LEB2PIqWPLSrb99ft)<br>

### SAP Certification on SAP Build
> [C_LCNC_02 - SAP Certified Citizen Developer Associate - SAP Build Low-code/No-code Applications and Automations](https://learning.sap.com/certification/sap-certified-citizen-developer-associate-sap-build-low-code-no-code-applications-and-automations)<br>
