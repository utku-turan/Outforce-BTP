# SAP Build Apps
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/efef8485-4e5e-4940-afd6-24471a906a2b)

> - ***Page Selector***: Lets you create new pages and switch which page is displayed.
> - - ***Special Areas***: Data for bringing data into the app, Launch for launching and testing the app.
> - ***Canvas***: where you build the interface.
> - ***Components***: components that can be added to the canvas, buttons, images, etc.
> - ***Properties***: where you configure the components you added. Also for other things you have to configure, like the page or logic components.
> - ***Tree View***: all the components on the page are shown here in a tree hierarchy.
> - ***View/Variables***: There is also the logic pane where you indicate how the application should react to the ser and other events. By default, this is closed, but you can open it up by clicking the link at the bottom of the canvas.

## Logic Pane
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/b49561d2-bae3-4a1c-8bc4-4a1447eb3e77)

How the application should react to the user and other events.<br>
To ensure that business rules are appropriately met by the application, the supporting logic needs to be defined as a flow of events, actions, and functions. <br>
***Events*** are triggers, actions are responses, and functions produce a result. Logic flow can be simple or branching, and used to customize any kind of behavior in an app.<br>

It works like the canvas, with widgets on the left that you can drag into your logic pane and that you connect to one another.<br> 
These widgets are called *flow functions* – because you are creating a flow of actions, starting from the triggering event through all the flow functions you connect to it.<br>

## UI component tools
The components area on the left of the screen contains all the UI components for bringing onto the screen.<br>
There are three tabs: 
> - ***Core***: Contains about 25 basic components, like buttons and input fields.
> - ***Marketplace***: Contains many more complex components that you can install into your app. Choose Marketplace to view a whole world of components.
> - ***Installed***: Shows all components you've installed, both core and Marketplace components.

> ***SAP AppGyver Preview app*** -> to display the app you're developing from your phone.
> It’s a good idea to use the Preview app while building, so you can see the changes you’re making to the UI and the components in real-time, and test them out.

## Backends of SAP Build Apps
SAP Build Apps lets you create your own data sources – you can design data tables, called entities, and populate them with data. These data sources can then be used in your applications, instead of you relying on only data from external sources.<br>

> - ***Entities***: DB tables that cotain tabular data.
> - ***Functions***: Actions that can use the data but also make calculations and return subsets of the data based on parameters sent from the application.
> - ***Deployment***: When the entities and functions are ready, you need to deploy them. Once deployed, they can be used by your applications.

![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/6705f304-9751-4ba3-b35a-8d0da1a07b0e)
![image](https://github.com/utku-turan/Learning-BTP/assets/73386835/9fb01322-862e-4d5f-a254-08a8c0fba39b)

## Bindings
A data variable coming from your data resource is just a piece of information. It doesn’t yet have a display in the UI of your app, so we need do do anther step in order to put it on the screen. That step is called creating a binding between a data variable and a UI component. Bindings can be used to create a link between a piece of data and a UI component.

***Variables*** are used to store data which we will get from the API, so that you can work with it and display it in the user interface of the app.

All of the variables in the application form the ***application state***. The state is not something you can see, rather it’s the idea that all the combinations of all the different variables can be thought of as different application states.

## App Example
[Here]() is the video that shows how to create an app and the steps below.

> - Create a new project.
> - Create the UI.
> - Add some custom logic.
> - Connect to an API.
> - Fetch data from the API.
> - Display data from the API.

## Another App Example
And [here]() is another video.
