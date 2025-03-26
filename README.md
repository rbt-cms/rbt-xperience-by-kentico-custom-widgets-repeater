# Xperience by Kentico Custom Widgets - Repeater

A Repeater widget is a commonly used component in Kentico CMS. It is used to display a collection of repeating elements dynamically based on configurations from widget properties.

# Installation

Install the RBT.Kentico.Xperience.Custom.Widgets.Repeater.1.0.0 NuGet Package to your Xperience by Kentico website (>=29.4.0 with .Net 8.0). 

# Widget
This is a widget which allows you to add a Repeater Widget to your screen with certain attributes that can be configured while adding. The properties that can be configured are:

- IsVisible: Select IsVisible option to show/hide widget on page
- PageTypeClassName: Select your desired Class Name
- Path: Specifies the path of the selected pages. If you leave the path empty, the widget either loads all child pages or selects the current page(depending on the page type and configuration of the widget other properties)
- ViewName: Enter the view name you created in your code for the selected page type
- MaxItemsDisplayed: Specifies the maximum of pages to be loaded. At least as many pages as in the 'visible' value of the 'initialization script' property need to be specified. If empty, all possible pages will be selected.
- OrderBy: Sets the value (like Columnname) of the ORDER BY clause in the SELECT statement used to retrieve the content
- OrderBy Direction: Select Orderby Direction like Ascening or Descending
- ContentBefore: HTML content placed before the widget content. Can be used to display a header or add encapsulating code such as div tag
- ContentAfter: HTML content placed after the widget content. Can be used to display a header or add encapsulating code such as div tag



# Add the Repeater widget to your project after installing the NuGet package

Follow these steps to integrate the **Repeater** widget into your project after installing the NuGet package.

Step 1: Configure Dependency Injection  
Insert the following code snippet into `Program.cs` and build the solution:

```
builder.Services.AddSingleton<IRepeaterRepository, RepeaterRepository>();
```

Step 2: Create a Repeater folder under /Components/Widgets/ in the project source code.

Example: ```/Components/Widgets/Repeater```

Step 3: Copy the Articles.cshtml file from ```/Components/Widgets/Repeater ``` in this repository and paste it into your project's ```/Components/Widgets/Repeater``` folder

Step 4: If you need more views for Article or any new page type, create your own views as per your requirements

Step 5: You can specify the view name in the View name widget property,``` e.g.: View name: Articles```


# Author

This custom widget was created by @Ray Business Technologies Pvt Ltd. Last updated 26-03-2025

# License

This widget is provided under MIT license.

# Uninstall

Uninstall this from the NuGet Package Manager and rebuild the project.

# Reporting issues

Please report any issues seen, in the issue list. We will address at the earliest possibility.

# Compatibility

This widget has been tested on Xperience by Kentico version (29.4.0) and can be used on >=29.4.0 with .Net 8.0. 
