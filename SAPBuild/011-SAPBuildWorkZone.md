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
