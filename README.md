# TaskTrackerFrontEnd
Frontend development new version for SAP Task Tracker Application (TechSchool 3rd Edition)

# Useful links

UI5 Documentation
https://sapui5.hana.ondemand.com/sdk/#content/Overview.html

UI5 mobile library explored
https://sapui5.hana.ondemand.com/sdk/explored.html

UI5 icons explorer
https://openui5.hana.ondemand.com/iconExplorer.html

BACKEND URL - Updated at 28.05.2017
https://testefortrainingi843890trial.hanatrial.ondemand.com/tasktrackertest/rest/task

SAP Cloud Platform
https://account.hanatrial.ondemand.com/cockpit#/acc/iXXXXXXtrial/accountdashboard -> XXXXXX (User ID)

# FRONT-END DEVELOPMENT
Access the SCP Cockpit > Subscriptions > SAP Web IDE > Open SAP Web IDE

# Creating a new UI5 project
-	File > New > Project from Template > SAPUI5 Application
-	Select the initial view to be XML and name it Tasks

# Developing the main view
-	Open the file Tasks.view.xml
-	Change the page title
-	Add a List with a CustomListItem containing a CheckBox
-	Add a footer with a toolbar and a button to add new tasks

# Developing the creation view
-	Right click on view folder > new > SAPUI5 View
-	Name it TaskCreation and select view type XML
-	Open the index.html > add an id pro the App > instantiate a new View and add it to the App
-	Open the TaskCreation.view.xml > add a Label and an Input > Add a footer with a button

# Navigating between views
-	Open the Tasks controller and implement the button press
-	Open the TaskCreation view and add the back button to the page
-	Open the TaskCreation controller and implement the back button press

# Creating a destination
-	Go to the Cockpit > Destinations > New Destination
-	Fill the name field >Fill the URL field with your backend URL > Save
-	In the webide, go to the neo-app.json and declare the destination

# Binding the list
-	Open the Tasks controller 
-	Declare a JSON model and the destination name
-	Go to the onInit method > set the model data > set the model to the view

# Creating tasks
-	Open the TaskCreation controller
-	Implement the save button press to get the value of the input field
-	Implement a function to make an ajax call to the backend in order to create a new Task
-	Call the ajax function from the button press function, passing the input value


# Loading the tasks from the backend
# Updating the tasks
# Deleting the tasks

# Refresh the list
