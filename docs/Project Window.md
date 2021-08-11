
# Chapter 4 Mine Design Core Module

What you will learn:

- [Overview](#41-overview)
- [Dropdown Menu](#42-dropdown-menu)
- [Main Menu](#43-main-menu)
- [Utility Menu](#44-utility-menu)
- [Layer Menu](#45-layer-menu)
- [Screen Menu](#46-screen-menu)
- [Message Bar](#47-message-bar)





<hr style="height:2px;border-width:0;color:gray;background-color:grey">



## 4.1 Overview


The Project window is used to create and manipulate various Opencontour projects using various elements, such as panels, bars, windows, etc. After finalizing the **Project Settings**, the new project will be created. The project's name and version number are displayed in the upper right-hand corner of the **Project Window**.

![Image](/image/proejct_window_dashboard.jpg)

In the project window, you can access the following menus:

- Dropdown Menu
- Main Menu
- Drawing Window
- Utility Menu
- Layer Menu
- Message bar

**Dropdown Menu:** A Dropdown Menu is located below the browser address bar. This menu is used to save and open files, configure display parameters, access design features, and access the Help Guide directly. Refer to section [Dropdown Menu](#dropdown-menu) for more details.

**Main Menu:** When a project is opened, the Main Menu appears at the top of the display window. A project can be built using the layer drawing and editing tools available in this menu and running functions.

**Drawing Window:** When a project is open, the Drawing Window is the top area of the display window and the location of the CAD design work. When a project is opened, this section is initially empty until layers are added.

**Utility Menu:** The Utility Menu enables users to make changes to **Project Settings**, **Project Properties**, **Scheduling**, **Scripts**, **Charts**, and **Reports**. These topics are described throughout this document in the order in which they occur procedurally.

**Layer Menu:** The Layer Menu is used to edit individual layers.

**Message bar:** The message bar is used to convey information such as coordinates, elevations, strike angles, wall angles, and distances to the user.

**Additional Option:**

- **Zoom in:** Press **+** button to zoom in. This has the same effect as turning the mouse wheel.

- **Zoom out:** Press **-** button to zoom out. This has the same effect as turning the mouse wheel.

- **Zoom bar:** This bar allows you to zoom in and out by sliding it up and down.

  ![Image](/image/Additional_option.jpg)

<hr>

### Other Operations

**Panning**

The user is also able to pan, by holding down the left mouse key in the **Drawing Window** and dragging it to a new location. Panning can also be used to view the entire contents of the Properties display window while viewing a feature's properties.

**Schedule Fill Down in the Schedule Window**

To fill the remining schedule periods with a value, type the value in a blank entry box (for either the **Mine Constraint** or **Process Limit**). Select the value, right-click and choose either Copy Up or Copy Down.

**Rotate View**

Holding down the **Alt** + **Shift** keys on the keyboard and panning with the mouse will rotate the view displayed in the **Drawing Window**. 

**Copy a Selected Feature in the Drawing Window**

Use the **Select Feature** button to select a single feature in the active layer. Right-click in the **Drawing Window** to copy. You can also copy an entire layer by selecting the **Design > Copy All To** Dropdown Menu,

Features may be copied from an active layer to inactive layer. To copy from an active layer to an inactive layer, follow the steps mentioned below.

1.	Activate the layer you wish to copy a feature from.

2.	Use the **Select Feature** button, to select the item. The selected item will change to a light green color.

3.	Right-click the mouse and select a layer from the dropdown. The layers listed will contain all available layers in the current project. The selected item will be copied to the selected layer, at the same elevation as in the originating layer. 

    **NOTE:**

    - **If a layer (for example, Filler5) does not appear, you must first add the Filler layer.**
    - **The Mineplan and Schedule layers can not be copied.**

&nbsp;
4. Verify that the copy procedure worked properly by unchecking the originating layer of the feature and turning on and activating the destination layer.


**Remove A Selected Feature in The Drawing Window**

An active layer's features may be removed. Use the **Select Feature** button to select a feature, then right-click. A **Remove** option will appear in the Drawing Window.

The available options are:

- **Current** – removes the currently selected contour.
- **All** – removes all contours in the layer.
- **Above** – removes all contours in the layer vertically above the currently selected contour.
- **Below** – removes all contours in the layer vertically below the currently selected contour.

     ![Image](/image/Remove_A_Selected_Feature.jpg)

<hr style="height:2px;border-width:0;color:gray;background-color:grey">

## 4.2 Dropdown Menu

A Dropdown Menu is located below the browser address bar. This menu is used to save and open files, configure display parameters, access design features, and access the Help Guide directly. 

  ![Image](/image/drop_down1.jpg)

<hr>

### 4.2.1 Project

The Project option is located in the top-left corner of the screen in the Dropdown Menu. Click on the term **Project**. The extended Dashboard will appear.

  ![Image](/image/project_dashboard.jpg)

The dashboard displays:

- A list of current projects. Click the **New Project** button to initiate a new project. Additionally, you can reopen a previous project by clicking the project name given underneath the **New Project** option.

- **UserName** at the top of the window.

- Version release information is located in the top-right corner of this screen (date of last software update).  

- **Logout** (press either of the Logout words).  You can change users by going back to the login credentials screen.  
<hr>

### 4.2.2 File

The file menu is used to handle files and project activities. Click on the term **File**. The extended Dashboard will appear.

  ![Image](/image/File_extended.jpg)


##### File > Open Project Tab

This option will launch a new browser tab pre-loaded with Opencontour. The page will serve as a welcome page for selecting or creating projects.

##### File > Clear Project

When selected, the current project will be closed and all layers in the **Layer Menu** will be cleared. The same project will remain open, with no layers loaded.


##### File > Open

This option inserts a layer into a project and assigns it to the provided location in the file. Click **Open** from the file menu and select the file. This option can be used in place of the **drag and drop** feature in the Dropdown Menu. The file location is specified by the **la** property in the JSON file when it is stored.


##### File > Save Layer

A layer can be exported from Opencontour as a JSON file once it is created and active in the **Layer Menu**. 

  1. From the Layer Menu, select the desired layer. 
  2. Click **File > Save Layer**.

    Depending on the active layer, the file name will automatically include the layer's default extension.

##### File > Clear Layer

To clear an activated layer, select the **Clear Layer** from the dropdown. 

##### File > Save Group

The Save Group will display the four available group file options. 

- All (Model)
- All (most commonly used)
- Contour Group
- Mineplan Group

  Saving the group file will save the inputs in the [Leach/Stacking](#leach) Module, Grid tab, the Legend, Grid Settings and Charts. 

##### File > Save DXF

From the Layer Menu, select the desired layer and click **Save DXF**. The following layers can be saved as DXF files:

  - Base
  - Geotech
  - Cutter
  - Filler
  - BaseResult
  - CutterResult
  - Roads

##### File > Import DXF

To import a DXF file, 

1. Select the **Import DXF** option from the dropdown. A popup window will appear.

  ![Image](/image/import_dxf.jpg)

&nbsp;
2. Click **DXF Layers**.  The DXF's layers will be listed. 

  ![Image](/image/DFX_layaer_list.jpg)

&nbsp;
3. Select the layer. DXF files may be imported into one of five Opencontour layers; Import, Base, Geotech, Cutters, or Fillers.

&nbsp;
4. Click **Import DXF**.

  >**NOTE: During the import, the user can run the Fix All Polygons (Fix) on the imported features. The Error layer will be used to store errors. To proceed past the error warning, click the x in the upper right corner**

![Image](/image/polygon_error.jpg)


##### File > Open Model

The Open Model function is used to import **models** and **mineplans** into a project. 
After selection, the user is required to specify the directory and file location for the Model. The supported file formats are: 

- JSON
- CSV
- TAM (Typed Array Model)
- Save TAM


>**NOTE**

>- **It is important that all CSV files used for data import are in the 'generic' format (for example, 43914 with no decimals for the pm property). Commas should not be used as thousand delimiters in data records (including grades).**

>- **Dates should be entered in the Excel serial format: m/d/yyyy.** 

To import a CSV file:

1. Click **File > Open Model > CSV** and import the Model or Mineplan layer.

  ![Image](/image/CSV_IMPORT.jpg)
&nbsp;
2. Enter the following details.

  ![Image](/image/CSV__element_details.jpg)

&nbsp;
3. After addressing each entry, click **Import**.


##### File > Save As PDF

This function is used to create a PDF file for plotting. Everything that is presented in the Drawing Window will be captured and saved. Objects should be centered to be included in the popup prompt's scale.

1. Click **File > Save As PDF**. The Print PDF window appears.

  ![Image](/image/save_as_PDF.jpg)

&nbsp;
2. Each entry in this template is configurable, including the Size and Scale options.

&nbsp;
3. Click **Print** to save the file as a PDF.

<hr>

### 4.2.3 Display

The display menu is used to summarize specific views and data information.

  ![Image](/image/Display.jpg)


##### Display > Volumetric 

The data represents a summary of the attributes of the features in the CutterResult layer. The Volumetric feature provides two options for filtering:

- Detail
- Summary By 

**Detail View **

1. Click **Display > Volumetric > Detail**. The Volumetric Summary window appears.

  ![Image](/image/Volumetric_summary.jpg)  

&nbsp;
2. For more information on each field, see the following table.

  ![Image](/image/Details_table.jpg) 


**Summary By**

These summaries are used to query pit volumes, design dumps, and construct leach pads. t is applied to any shapes that are present in the CutterResult layer. The mass data is independent of the Mineplan

The **Summary By** provides three options to filter:

- Filler/Cutter

- Phase Name 

- Bench 

**Filler/Cutter**: It summarizes the cut and fill areas, volumes, and mass and generates a file with a calculation for each cut fill number.

  ![Image](/image/Volumeteric summary_1.jpg) 


**Phase Name**: It functions similarly to the **Filler/Cutter** option, except that each line of data will include the Phase Name (pn). The similarities between cut fill num and pn can be noticed in the detail report.

  ![Image](/image/Volumeteric summary_2.jpg) 


**Bench**: The Bench option makes use of elevation (z) but does not provide information about the initial cut fill num or pn.

  ![Image](/image/Volumeteric summary_3.jpg) 


##### Display > Contour By PM

This function can be used to populate the baseResult layer with period map contours after a schedule is run.

1. Click **Display > Contour By PM**. The Contour By Period Mined window appears.

    ![Image](/image/ContourByPM.jpg) 

You can enter a period number (for example: 5) or a date in the **Period Mined (pm)** entry box. The single down arrow displays a calendar, while the other increments the current date.

Fillers can obstruct Cutters if they are positioned on top of each other.  Hence, there is a choice for their display.  This is apparent in pits where backfilling practices are used.

When the Filler and Cutter layers' checkboxes are checked, this function creates contours in the BaseResult layer for them.


##### Display > Grid Settings

Grid settings are used to include grids in the project.

1. To select the grid interval, Click the **Display > Grid Settings**. 

  ![Image](/image/Grid_settngs.jpg) 

&nbsp;
2. Click the **Save** button.  The View Latitude and Longitude button on the Main Menu will be activated. To bring the display to a halt, push the **View Latitude** and **Longitude** button until it turns green. The following sections cover each option in the **Gridline Settings** box.


**Scale Bar** 

If the Scale Bar is enabled, it will be displayed in the Drawing Window's lower left corner. The value displayed in the bar and the spacing between the gridlines are adjusted by zooming in and out with the mouse.

  ![Image](/image/grid_settings_scale_bar.jpg) 


**Compass** 

If the compass is shown, it will appear in the upper right corner of the Drawing Window.  The arrow vertices towards the North.

  ![Image](/image/grid_settings_compass.jpg) 


**Labels**

Northing and Easting intervals are displayed by ticking the Labels box in **Display/Grid** Settings

  ![Image](/image/grid_settings_label.jpg) 


##### Display > 3D

The Drawing Window's layers are displayed three-dimensionally in a new browser tab. Click **Display > 3D**. 


The 3D view options are:

- **Contour Lines** – for viewing the contours as 3D strings. It has the capability of showing the layers in a Spin mode, with a variable Speed bar.  

-	**Surface** – displays the contours as an opaque overlay.

-	**Section** – shows a sliced view from a selected vantage point. It allows the user to change the view by using the Change View option from the Display menu.

-	**Timeline** – animation of the project for the project life.


These tools are detailed in the 3D View Tools section.

  ![Image](/image/3D_new_browser_tab.jpg) 


  ![Image](/image/3D_newtab_elementDetails.jpg)

<hr>

### 4.2.4 Design

The following options are available in the design menu:

- Copy All To

- Reorder Fillers

- Organize Fillers


##### Design > Copy All To

This option enables you to copy all features from one layer to another. To copy a layer to another, follow the steps below:

1. Activate the layer from which you'd like to copy features.

2. Click **Design > Copy All To** to access to the list of layers in the project.

  ![Image](/image/Figure 4 43 Dropdown Menu, Design-CopyAllTo Options.jpg)

&nbsp;
3. Select a layer. A notification message will appear.

  ![Image](/image/Figure 4 42 Copy All To Notification.jpg)

&nbsp;
4. Press **Ok**. In the **Drawing Window**, the copied features will be displayed. Each feature will be colored blue, giving the appearance that the function is being used.


##### Design > Reorder Fillers

The **Reorder Fillers** option in the Dropdown Menu can be used to reorder filler layers that were built out of order for a particular project.

   ![Image](/image/Figure 4 44 Dropdown Menu, Design Options.jpg)

To reorder the filler layer, follow the below steps:

1. Click **Design > Reorder Fillers**. Reorder Filler Layers window will appear, listing all the Filler layers in the project along with their original cut fill number.

    ![Image](/image/Figure 4 45 Initial Reorder Filler Layers Window.jpg)


2. Each Filler listed in the **Reorder Filler Layers** window can be dragged to a different listing position in the **Reorder Filler Layers** window. To move the Filler to a new location in the list, hold down the left mouse button and drag the Filler.

    ![Image](/image/Figure 4 46 Reorder Filler Layers Window; Filler Order Listing Changed.jpg)&


3. Click **Reorder** button. The original position of the layers in the **Layer Menu** will not change, but their cut fill num will. The cut_fill_num will be assigned to the Filler layers so they are numbered sequentially


4. An advisory notification will appear before approving the change. Click **Ok**.

    ![Image](/image/Figure 4 49 Reorder Filler Layers Change Notification Window.jpg)

>**NOTE: The order and positions of the layers listed in the Layer Menu can be rearranged, but any changes will not be saved.**


<hr>

### 4.2.5 Help 

To access the help documentation, visit help.opencontourXXXX.com 

  ![Image](/image/Figure 4 76 Dropdown Menu, Help Options.jpg)

-  **Cheat Sheet**: Provides an overview of the Opencontour layout and techniques.

-  **Help Guide**: Opens a new browser tab with a searchable full Help Guide page.

<hr style="height:2px;border-width:0;color:gray;background-color:grey">

## 4.3 Main Menu


The Main menu provides access to tools for creating and editing projects. It enables you to view and control the context of the currently running task or workflow.


  ![Image](/image/Figure 5 1 Main Menu.jpg)


- When a button is available for selection, it is shown in light green ![Image](/image/green_button.jpg). 

- When a button is selected and currently active, it is shown in orange ![Image](/image/orange_buton.jpg). You can deactivate the button by re-selecting it. When the button is not in use, it should revert to its default light green color.

Select the layer from the **Layer Menu** to display the hidden buttons.


### 4.3.1 Buttons

![Image](/image/button_list.jpg)


- **Zoom to full extent** ![Image](/image/Zoom to full extent.jpg): This button will magnified the view to show the full scope of the project.
<hr>

- **Zoom to layer extent** ![Image](/image/Zoom to layer extent.jpg): This button will magnified the view to the active layer extent at the current elevation indicated in the Message bar.
<hr>

- **Up one Level** ![Image](/image/Up one Level.jpg): Move the Drawing Window up in elevation by the BenchHeight value in the Project Settings.
<hr>

- **Down one Level** ![Image](/image/Down one Level.jpg): Move the Drawing Window down in elevation by the BenchHeight value in the Project Settings.
<hr>

- **Copy Cutter Up Level** ![Image](/image/Copy Cutter Up Level.jpg): Expand the pit contour up or down to the next contour’s elevation. It is used when constructing pits, dumps, or leach pads.
<hr>

- **Cut Contour with Cutter/Filler** ![Image](/image/Cut Contour With Cutter-Filler.jpg):  Use the **Cut Contour with Cutter/Filler** button ![Image](/image/Cut Contour With Cutter-Filler.jpg) on the respective Cutter and Filler layers in the Layer Menu to cut or filled Base topography. This populates two levels automatically: the **BaseResult** layer and the **CutterResult** layer, both of which are saved as part of the Group files. These layers are rewritten each time this button is clicked.




<hr>

- **Add Cutter Layer** : Adds another Cutter layer. Each additional layer will be sequentially numbered and the Phase Name (pn) should be edited for each.
<hr>

- **Add Filler Layer** : Adds another Filler layer.  Each additional layer will be sequentially numbered and the Phase Name (pn) should be edited for each.
<hr>

- **Non Bench** ![Image](/image/Non Bench.jpg): Non Bench will remove all features if it does not lie on a project’s mid bench interval elevation. To use:

    1. Activate the Layer from the **Layer Menu** that contains features that are not at project elevation levels.

    2. Click the Non Bench ![Image](/image/Non Bench.jpg) button to remove them all from the layer at each erroneous elevation. This option is very useful when importing a DXF file with horizontal slicing every 3 feet and significant curves every 9 feet. This is not necessary for contours of 3 and 6 feet.
<hr>

- **Fix All Polygons**![Image](/image/Fix All Polygons.jpg): Use of the Fix The All Polygons function ensures that the displayed features contain beginning and ending vertices.To use:

    1. activate the Layer from the Layer Menu.
    2. Click the Fix All Polygons button ![Image](/image/Fix All Polygons.jpg) from the Main Menu. Select a contour at the current elevation displayed in the Message bar  to prepare the features for editing.
    3. Select **OK** in the notification message. The notification message will convey th fixes made.

  - The function removes and checks for the following things:
      - The total number of features
      - The existence of multi polygons or features
      - If the first coordinate is the same as the last in the features, i.e. closing of a polygon
      - Feature duplication and removal
      - Areas of less than five, to discard minute features
      - Features with less than two coordinates
      - Kinks 
  


<hr>

- **Display Vertice Number** : The Display Vertice Number function is useful for displaying the point order in a contour.  It is possible to see kinks in the numbers presented when they overlap each other.To use:
    
    1. Activate the Cutter or Filler layer from the Layer Menu. 
    2. Select the feature tool ![Image](/image/feature tool.jpg), and select a contour to be labelled.
    3. Click the Display Vertice Number button ![Image](/image/Display Vertice Number.jpg). Each vertice on the selected contour will be assigned a sequential number, making it easier to spot kinks, etc., where the numbers overlap.

    ![Image](/image/Figure 5 7 Numbered Vertices.jpg)
     


 activate the Cutter or Filler Layer from the Layer Menu.  Each vertice will be assigned a sequential number; making it easier to spot kinks, etc.  
<hr>

- **Add Toe Crest**![Image](/image/Add Toe Crest.jpg): Opencontour can add toe and crest lines for projects that require extra detail. To add these lines at the appropriate elevations  (0.5 x BenchHeight):

    1. activate the Cutter or Filler layer in the Layer Menu that needs toe and crest lines.

    2. Click the **Toe Crest button** ![Image](/image/Add Toe Crest.jpg).

The contours designed and viewed are at mid bench elevations. Bench elevation contours may be inserted and viewed, but they are not part of the major design process steps.

<hr>

- **Clear Toe Crest**![Image](/image/Add Toe Crest.jpg): Opencontour can remove added toe and crest lines in a layer. Only available when the Cutter, Filler or BaseResult layer is active. 
    
    1. Activate the Cutter layer that needs toe and crest lines removed.
    2. Click the **Clear Toe Crest**![Image](/image/Add Toe Crest.jpg) button.


<hr>

- **Add Box** : Click this button to add a border around the extents of the topography contours at a selected elevation. Available when Base layer is active.  
<hr>

- **Select feature** : This option enables selection of the desired feature when the relevant layer is selected from the Layer Menu.  
<hr>

- **Select features with a Box**![Image](/image/Select features with a Box.jpg): 

    1. Click the first box corner![Image](/image/Select features with a Box.jpg) to select a feature in the active layer.
    2. Hold the mosuse button and move the mouse to draw the box to the diagonally opposite corner
    3. All features in the active layer that are within or touch the drawn box will be seleced and highlighted in green.
<hr>

- **Add Haul/Load Features** : Click this button and specify the location with a left mouse click to insert a feature that contains an elevation, type, name, availability, utilization, efficiency, and fleet count. Loaders will be given a tnsPerHr productivity rating.  Trucks require rated speeds for gradients that are low, medium, and high & a ‘truckfactor’ (truck payload) & rank.  The units used in the speeds must match those of the project files (i.e. imperial or metric).  
<hr>

- **Add Dump Features** : Click this button and specify the location with a left mouse click to insert a feature that contains an elevation, type, capacity, tns (populated during a schedule run), and name.  Available when Schedule layer is active.  
<hr>

- **Add Phase Features** : Click this button and specify the location with a left mouse click to insert a feature (intersection) that contains an elevation (z), type, name and order.  Available when Schedule layer is active.
<hr>

- **Add Stockpile Features** : Click this button and specify the location with a left mouse click to insert a feature that contains an elevation, type, name, a processing order, and a owmin and owmax for determining the values of the Routing variable (data.ow) blocks accepted on that stockpile.  Available when Schedule layer is active.
<hr>

- **Add Leach Crush Features** : Click this button and specify the location with a left mouse click to insert a feature that contains an elevation, type, name, a processing order, and a owmin & owmax for determining the values of the Routing variable (data.ow) blocks accepted.  The that feature name must be leach; it must match the filler Phase Name (pn) name of each leach cell (Filler) created.  Available when Schedule layer is active.  Material mined reports here after stockpiling.
<hr>

- **Add Leach ROM Features** : Click this button and specify the location with a left mouse click to insert a feature that contains an elevation, type, name, a processing order and a owmin & owmax for determining the values of the Routing variable (data.ow) blocks accepted.  The that feature name must be leach; it must match the filler Phase Name (pn) name of each leach cell (Filler) created.  Available when Schedule layer is active.  Material mined reports directly here rather than via a stockpile.

- **Add Point Features** : This will add point features to the active layer.  Only available when the Schedule layers are active. 

<hr>

- **Add Line Features** : When the Roads layer is active, this property becomes available.  This will add lines to those selected layers.  

<hr>

- **Add Polygon Features** : To start drawing polygons or contour lines:

    1. Activate the appropriate layer.
    2. Click the **Add Polygon Features** button. 
    
      Only available when the Base, Cutter, Filler, BaseResult or CutterResult layers are active.  
<hr>

- **Modify features**![Image](/image/Modify features.jpg): 

    1. To add a vertice, click the left mouse button once on the line where the vertice is to be placed. 
    2. To delete a vertice, click the left mouse button once on the vertice to be deleted. 
    3. To move a vertice, hold down the left mouse button and drag the vertice. Release when it moves to the desired location. 
<hr>

- **Snap to paths, and vertices** : Allows snapping the cursor to lines and vertices in the Drawing Window for the activated layer.  
<hr>

- **Remove features**![Image](/image/Remove Features.jpg): Delete a feature from the active layer. To delete an entire feature in an active layer:

      1. select **Remove features**![Image](/image/Remove Features.jpg) from the Main Menu.

      2. Select the feature to be removed from the drawing screen. Deselect this button when finished.
<hr>

- **Drag features** : Drag a feature to a different location (but not elevation) in the Drawing Window.  

<hr>

- **Modify Number of Feature Vertices**![Image](/image/Modify Number of Feature Vertices.jpg): If a feature has too many vertices, this will reduce the unnecessary vertices to make the feature easier to work with. To reduce the number of vertices, use the Vertice value in the **View Settings** as the distance between vertices.

      1. Select the active layer.  

      2. Press the **Modify Number of Feature Vertices button** ![Image](/image/Modify Number of Feature Vertices.jpg)

      3.	Select the feature.


<hr>

- **Create Curve**![Image](/image/Create Curve Smoothing A Feature.jpg): A curved line can be created using this tool. The function outcome will depend on the value entered for the Vertice and it is changeable through the **View Settings**.

    1. Activate the feature layer. The feature’s layer must be activated to insert vertices into the curve.

    2. Select a feature in the active layer.  

    3. Click **Create Curve** button ![Image](/image/Create Curve Smoothing A Feature.jpg). The selected feature will be replaced with a curved feature, with vertices inserted as needed. This function is active in layers with features (Base, Geotech, Cutter, Filler & Roads). This function uses the Vertice number written in the Project Settings, or View Settings.  
  

<hr>
 
- **Split Polygon** : Pick one feature, then pick a second feature. The first feature will split the second feature.  The area of the first feature selected inside the second will be maintained. The remainder of the first feature selected can be deleted.  
<hr>

- **Union Two Polygons** : Pick one feature then pick another feature, these two features will join to form a new feature.  If using ramps, the start of the ramp (denoted by the red circle) will be retained for the second feature selected.  
<hr>

- **Set First Poly Vertex** : Moves starting location for ramp (red dot) to vertice on feature specified.  
    1. Draw the feature.
    2. Click **Set First Poly Vertex** button from the Main Menu and click the new position for the inside vertice of the ramp to start from.
    3. Click the button again to exit this function.  

 
<hr>

- **Properties** : Displays the table of layer or feature Properties (the layer should be active in the Layer Menu) in the Drawing Window.  To select this display box, left-click the Properties button or hit the **p** key on the keyboard.
    
    - Click the **+** button to add parameters to the Properties table.
    - Clcik the **x** button to delete parameters from the Properties table.
    - Click the save button to save the changes.
 
<hr>

- **Measure**![Image](/image/Measure.jpg): 
    - Distance: To determine the distance, use the **Measure** tool ![Image](/image/Measure.jpg). Left-click on the first vertex in the Drawing Window, followed by the second vertex to be measured. The result will appear in the Message bar.  
       
          ![Image](/image/Figure 5 2 Measured segment displays in the Message bar.jpg)
       
    
    - Strike: This describes the angle between the North vector and the line direction. For strike, select the two contour vertices in the direction they were drawn (clockwise or counterclockwise).  
    
    - Wall Angle: When measuring wall angles, select the line for the 1st mid bench, then select a line for a higher or lower mid bench in the same vertical plane.  

        1. Select a wall contour line for the first mid bench.  The lighter blue line that appears acknowledges the first selection on the 1950 elevation.

        2. Move to the next mid bench using q,![Image](/image/Q.jpg), w, or ![Image](/image/W.jpg). Then select a line perpendicular at a higher or lower mid bench in the same vertical plane. The next mid bench measured here is at the 1945 level.
        3. On selection of the second line, the Message bar will display the wall angle if measured correctly.
        4. Click the **Measure** button to exit the measuring and snapping activities. 

        ![Image](/image/Figure 5 3 Measuring Wall Angle, From (Start) Elevation, 1950.jpg)

        ![Image](/image/Figure 5 4 Measuring Wall Angle, To (End) Elevation, 1945.jpg)

        ![Image](/image/Figure 5 5 Message Bar Display, Wall Angle Shown On The Far Right.jpg)
<hr>

- **View Latitude and Longitude** ![Image](/image/View Latitude And Longitude.jpg): Activates display of latitude and longitude gridlines, scale bar and north arrow. Click **View Latitude and Longitude**![Image](/image/View Latitude And Longitude.jpg) button. The settings selected will be displayed in the Drawing Window. 

<hr>

- **Export CSV** : Available for CutterResult, Mineplan & Import layers only.  

<hr style="height:2px;border-width:0;color:gray;background-color:grey">

## 4.4 Utility Menu

The utility menu enables you to customize the standard interface by providing access to secondary actions and tools such as project properties, create schedule, create script, report etc.

The Utility Menu is located to the right of the Drawing Window, above the Layer Menu, 


  ![Image](/image/Figure 6 1 Utility Menu.jpg)

### Buttons

  | Button    | Description |
  | ----------- | ----------- |
  | ![Image](/image/Utility_project_settings.jpg) | Project Settings, recalls the saved Project Settings. Click [here](#project-settings) for more information.|
  | ![Image](/image/Utility_project_properties.jpg)   |Project Properties, amending feature properties. Click [here](#project-properties) for more information. |
  | ![Image](/image/Utility_Create Schedule.jpg)   |Create Schedule, opens the scheduled mining & processing tonnages for each phase. Click here for more information.|
  | ![Image](/image/Utility_Create Script.jpg)  | Create Script, Mineplan property creation & manipulation tool. Click here for more information.|
  | ![Image](/image/Utility_Create Charts.jpg)   | Create Charts, charting facility for Mineplan & model properties display. Click here for more information.|
  | ![Image](/image/Utility_report.jpg)   | Report, report CSV builder facility for the Mineplan data. Click here for more information.|


&nbsp;

<hr>

####  4.4.1 Project Settings 


Each project listed in Opencontour has its own set of Project Settings parameters. These parameters can be exported and imported as required.

The project settings can be accessed by clicking the Project Settings button![Image](/image/Utility_project_settings.jpg) in the Utility Menu.  

The project window is divided into three distinct settings windows.

- [Drawing Window Settings](#drawing-window-settings)

- [Schedule Settings](#schedule-settings)

- [buildMineplan Settings](#buildMineplan-settings)


After making any changes, click the **Save** button. These settings are stored in an online database and can be viewed from any computer connected to the internet. The user is redirected to the Drawing Window at the most recently viewed elevation.

  ![Image](/image/Figure 6 2 Project Settings Window.jpg)


##### Drawing Window Settings

The Drawing Window Settings section controls what is visible and designed in the Drawing Window.


##### Schedule Settings

The Schedule Settings portion help to define the Filler’s Density - mass/volume (ton/ft3 or t/m3) and Swell.


##### buildMineplan Settings. 


The buildMineplan Settings portion of the window is used to set site-specific Model values in Opencontour to be written to the Mineplan. These properties are also used when the Schedule is run and will also be stored in the Mineplan layer. For instance, if the site makes use of the terms "specific gravity" or "relative density" rather than "density," this variable may be specified here.


##### Auto Save (in minutes)


This feature will not be available until the box is checked. The default saving interval is ten minutes, with a minimum of one minute between each saving interval.

When the checkbox is selected, the interval will produce a backup of the All (Model) group file, including the Model layer. For example, “April 11, 2019-09.41.00AM pit1 all backup.json” is an example of a file name. If a project _all.json file is loaded the file name will replace “pit1_all”.

<hr>

#### 4.4.2 Project Properties 


To open the Project Properties screen, click **Project Properties**![Image](/image/Utility_project_properties.jpg) button in the Utility Menu.

 ![Image](/image/Figure 6 3 Project Properties Window.jpg)


The properties window is divided into three distinct windows and Each of the three windows has its own function.

- Layer Properties

- buildMineplan Properties 

- Legend


##### Layer Properties

The Layer Properties section at the top of this window is used to add a property to the currently selected layers. Properties can be added to a selected layer by typing the name of the property in the Property field in the Layer Properties dialog box.

Typically, the Mineplan characteristics are modified. The shown list will contain all of the project's layers.

 ![Image](/image/Figure 6 4 Project Properties Choose Layer List.jpg)

To add a property to the **Mineplan layer**:

1. Click the **Choose Layer** dropdown window in **Project Properties** portion. 

    ![Image](/image/Project_properties.jpg)


2. Select the layer **Mineplan**.

3. Enter the name of the new property and the formula to calculate the property. The format of any formulae entered in the Property Value section should have the true and false values inside curly brackets.

4. Click **Populate Property** button.

5. Click **Save** buton to store the information entered in the project.  

#####  Property and Property Values

When referring to a Property in the **Mineplan** layer, the property is referred to without “data.” written before the property.  For example, if the property is data.au, a Property entry is written “au”.  

  | If Statement    | Formatted Written Example |
    | :-----------: | :-----------: |
    | if(logical test){value if true}{value if false}| if(data.au>0.3){1}else{0} |

&nbsp;&nbsp;

Here is an example of a property formula entered for the Property Value.  Values and codes can be assigned in the **Property Value** field using text (“TEXT”), integers, and “If Statements”.If statements must contain the Else part of the equation; the value if false.  More script examples are in the document “JavascriptGuide.pdf”.


If the values are reported with too many significant figures, use the formulae below (specifically, the “.toFixed(3)”) to refine your formula to three decimals

  | Formatted Written Example   | Calculated Value | New value |
  | :-----------: | :-----------: | :-----------: |
  | +(data.dens*data.vol).toFixed(3)|56842.88861132361 | 56842.889 |

&nbsp;&nbsp;

#####	buildMineplan Properties

The buildMineplan Properties section of the window builds the Mineplan using the entries in the **buildMineplan Settings** section of the **Project Settings** window. The **Mineplan layer** is built using the **CutterResult** shapes and the **buildMinepla**n function


The blocks within the Model layer will estimate their tonnage using the density value, data.dens, specified in the Density (dens): field in the Project Settings, buildMineplan Settings. Outside the Model layer, the Density - mass/volume (ton/ft3 or t/m3): value in the Schedule Settings section will be used to estimate the tonnage.


**justOre Checkbox**: a Mineplan that retains ore blocks but groups null (empty) waste blocks inside the CutterResult with grouped null waste records for each elevation shape.

#####	Legend

The Legend enables you to view a property that is shaded by color, even if it is not the active layer.

<hr>

#### 4.4.3 Create Schedule 

To open the schedule window, click **Create Schedule**![Image](/image/Utility_Create Schedule.jpg) button in the Utility Menu. Please

  ![Image](/image/Figure 6 5 Schedule Window.jpg)

<hr>

#### 4.4.4 Create Script 

To open the Script window, click **Create Script**![Image](/image/Utility_Create Script.jpg) button in the Utility Menu.

  ![Image](/image/Figure 6 6 Script Window.jpg)


Scripts can be written to run over the Mineplan before, during or after running a schedule.  The programming language used is JavaScript. To know more about script, refer to JavascriptGuide.pdf


A variable used in a script must either already exist in the layer on which it is working or be defined in the script's previous line. When an error occurs in a script, Opencontour generates error messages to assist the user in identifying the faulty line. If no errors occur, the script will execute with a message. Additionally, This message also tells you how many records are in the layer.

 ![Image](/image/Figure 6 7 Script Run Completion Message.jpg)

<hr>

#### 4.4.5 Create Charts 

To open the charts window, click **Create Charts**![Image](/image/Utility_Create Charts.jpg) button in the Utility Menu. The Mineplan layer is the primary source of data for the charts, after the Schedule has been executed. Please


  ![Image](/image/Figure 6 8 Upper Create Charts Window.jpg)

<hr>

####	4.4.6 Report Tool


To open the report window, click **Report Tool**![Image](/image/Utility_report.jpg) button in the Utility Menu.

  ![Image](/image/Figure 6 9 Report Window, “report01.json” Loaded.jpg) 


  When executing a report, different browsers may display different export prompts (). Reports are generated over the Mineplan layer by specifying a grouping parameter, for example, "data.pm."


<hr style="height:2px;border-width:0;color:gray;background-color:grey">

## 4.5 Layer Menu

The **Layers Menu** is usually located on the right side of the project window. To activate a layer, click on the layer name in the **Layer Menu**. The layer will expand with a bold orange border. If the layer is active and the associated data is provided, the layer's parameters can be viewed and edited.

  ![Image](/image/layer_Menu.jpg)


- The horizontal scroll bar directly below the layer name in the **Layer Menu** can be used to adjust the darkness of each layer. Drag the bar left or right to adjust the darkness.

- The three QuickButtons at the top of the Layer Menu, **All/None**, **Schedule** and **Drawing**, are used to efficiently turn the display of multiple layers in the Layer Menu on and off in a project. Click the **QuickButton** to turn on or off any layer in the **Layer Menu**.

  ![Image](/image/Table 7 1 Layer Menu QuickButtons.jpg)
<hr>

### 4.5.1 Layer Geometry Types

The following layer option is available from the Layers menu. To learn more about it, click on each layer.

  | Layer  | &nbsp;&nbsp;la Property&nbsp;&nbsp; |
  | :-----------: | :-----------: | 
  | [Base](#base-layer) | ba | 
  | Geotech | ge | 
  | Cutter | cu | 
  | Filler | fi | 
  | BaseResult | rb | 
  | CutterResult | cr | 
  | Mineplan | mp | 
  | Schedule | mo | 
  | Model | ba | 
  | Roads | ro | 
  | Import | im | 

&nbsp;&nbsp;

<hr>

### 4.5.2 Functions

When a file is loaded into a Project, if the layer includes data, the layer's original file name appears beside the layer. Additionally, the number of files added to a layer will also display in brackets. **Cutter** and **Filler** layers will display the Phase Name (pn) given to the layer.

  ![Image](/image/Figure 7 1 Layer Menu display, Showing Layer File Name Origin & Number Of Files.jpg)

In the above example, The origin file name was “Tutorial3.2_ph1,2&Dump_all.json”, containing the layers shown.  Cutter1 was named ph1, Cutter2, ph2.  Filler3 was dump 1.  A second file was dragged in to the Filler3 layer.  See the Filler3 – dump1 (2) entry.  The (2) is the count of the number of files added to the layer.

If the Layer Menu indicates that a layer has several files (as shown by the bracketed number), the layer should be checked for duplicate contours at each elevation. The menu can be expanded and collapsed. The order of the layers listed in the Layer Menu can be changed by dragging each layer to the desired location.

  ![Image](/image/Figure 7 2 Layer Menu.jpg)

<hr>

### 4.5.3 Drag and Drop Files

The drag and drop capability enables the user to drag a Group file or a single layer file into another layer.

To drag & drop a file into a layer, first activate the layer. For example, dragging the Cutter file to the Base layer will add the Cutter file to the Base layer. To undo this, either perform a **ClearLayer** or restart the project. When a file is dragged onto an active layer that already includes data, the data from the dragged file is added to the existing data rather than being overwritten.

  ![Image](/image/Figure 7 3 irma_base.json file Dragging To The Project Drawing Window.jpg)

 **NOTE : When dragging a Group file or a single layer file, if no layer from the Layer Menu is selected as active, the layer will be added to the corresponding layers based on the file contents in the la property. When you save, the la property is written to a file. If you don't activate a layer, you'll get the same result as if you use the Dropdown Menu method. File/Open**
<hr>

### 4.5.4 Layer Geometry Types

Each defined layer has a unique geometry type:

  ![Image](/image/Table 7 3 Layer Geometry Types.jpg)


**Base Layer**: The Base layer represents the original surface as closed contour polygons.  The closed polygons or features can include ‘holes’ that represent voids in the solid contour.  For the features to be viewed in 3D, contour features cannot exist outside contour lines at lower elevations.

**Cutter Layer**: Cutter layers represent contour lines that will create voids (pits) in the base layer.  For cutter layers to be viewed in 3D, contour features must encompass features at lower elevations.  Cutter layer features do not include ‘holes’.  


**Filler Layer**: Filler layers represent contour lines that will add (fill) to the base layer.  For Filler layers to be viewed in 3D, contour features cannot exist outside contour lines at lower elevations.  Filler layer features do not include ‘holes’.

**CutterResult**: include the result cuts when the Cut Contour with Cutter/Filler function is run.  This layer is overwritten each time the Cut Contour with Cutter/Filler function is run.

**BaseResult**: the BaseResult layer is the resulting surface after the Cut Contour with Cutter/Filler function is run.  The BaseResult layer is overwritten each time the Cut Contour with Cutter/Filler function is run.
<hr>

### 4.5.5 Layers

#### Base Layer


The Base layer includes the surface topography before any shapes are cut or filled. The features and shadings of the base layer are highlighted in red. The current elevation causes that contour to change to a solid feature with editable vertices. That contour is changed to a solid feature with editable vertices as the elevation changes.


  ![Image](/image/Figure 7 6 Layer Options, Base Layer Tools.jpg)

  ![Image](/image/Figure 7 5 Base layer Red Coloring.jpg)


Importing a DXF file is a common method of creating base layers.


#### Geotech Layer

The features of the Geotech layer are blue with grey shading. These features do not change appearance with elevation changes.

  ![Image](/image/Figure 7 7 Geotech Layer Coloring.jpg)

To add Geotech:

1. Click on the **Geotech** layer in the **Layer Menu**.
2. From the dropdown menu, choose any of the label options.

    ![Image](/image/Figure 7 8 Layer Options, Geotech Layer.jpg)

    - Geotech Layer, Name Option

    ![Image](/image/Figure 7 9 Geotech Layer, Name Option.jpg)

    - Geotech Layer, **IRA_BFA** Option

    ![Image](/image/Figure 7 10 Geotech Layer, IRA_BFA Option.jpg)


3. To reload the page, press the **q** or **w** keys. The Drawing Window will update the display after refreshing.

4. Click the **addGeotech** button in the Layer Menu's Geotech section to add a new domain shape with the extents of the **Project Settings** coordinates at the current elevation indicated in the Message bar. Domains can also be added using the **Add Polygon** Features tool, in the Main Menu.


#### Cutter Layer

The current elevation displayed in the Message bar causes the Cutter contour to change to a solid feature with editable vertices and internal shading if there is data on the elevation in the Cutter layer. Using the **Cutter Color** option, you can color multiple Cutter layers separately. 

The first Cutter layer features are dark blue, with lighter blue shading. Each cutter layer is colored by default, however the colors can be customized using the Cutter Color option. By default, the first Cutter is royal blue, the second is red, the third is fuchsia, etc.

  ![Image](/image/Figure 7 11 Cutter Layer Coloring & Contours-Points On Current Elevation, Base Layer Loaded (Pink).jpg)


The Cutter layer number is incremented as **Cutters** and **Fillers** are added, and is recorded in the cut fill num property. By dragging files onto active Cutter or Filler layers, you can work around these assigned **Cutter** and **Filler** layer numbers. For example, to assign an exported JSON file from the **Cutter6** layer to the **Cutter3** layer, activate the **Cutter3** layer in the Layer Menu and drag the exported **Cutter6** JSON export file into the Drawing Window. Then, using the Dropdown Menu File/Clear Layer, delete the contents of the **Cutter6** layer.

  ![Image](/image/Figure 7 12 Layer Options, Cutter Layer.jpg)

- Each Cutter layer can have a **Phase Name (pn)**, such as phase1, pit2, etc. When you press **Cut Contour using Cutter/Filler**, the **Phase Name (pn)** is written to the layer. This means that until the button **Cut Contour with Cutter/Filler** is pressed, the **Phase Name (pn)** will not be visible in the Drawing Window as a Label display.

- The **Direction (dir)** property entry is located beneath the **Phase Name (pn)** entry area.  This is used to specify a strike cutting direction from 0-360 degrees (90 degrees represents East).  If this value is 0, the **Panel Window** direction entries  will be ignored.

When drawing the Cutter, the **Cutter InterRampAngle (IRA)** and **Cutter Bench Face Angle (BFA)** from the **Project Settings** are applied. This is because the ramp widths and wall angles of Cutter material can be different for disturbed/mined material properties.

If a DXF file is to be imported into a **Cutter** layer, it must be imported individually into an empty Cutter layer (see Dropdown Menu File/Clear Layer). It can then be saved as a Cutter JSON file. 


  ![Image](/image/Figure 7 14 Drawing Window Cutter Layer Properties After Cut Contours With CutterFiller.jpg)


#### Filler Layer

Filler layers are used for constructing dumps and leach pads. As with Cutters, if there is data on the elevation in the **Filler** layer, the current elevation displayed in the Message bar causes that contour to change to a solid feature with editable vertices and internal shading.

The **Filler** layer numbers (cut fill num) are assigned automatically based on the number of existing Cutter and Filler layers and order of creation.

  ![Image](/image/Figure 7 15 Layer Options, Filler Layer.jpg)

- Each **Filler** layer can have a unique **Phase Name (pn)**, for example, leach01 and dump5. When you press Cut Contour with Cutter/Filler (section 10.5), the **Phase Name (pn)** is written on the layer and the **CutterResult** layer. This means that until the button **Cut Contour with Cutter/Filler** is pressed, the **Phase Name (pn)** will not be visible as a Label display for the Filler in the Drawing Window.

- The stack Direction (dir) property entry is located beneath the **Phase Name (pn)** entry area. This is used to indicate the direction of filling from 0-360 degrees (90 degrees represents East).

- The layers are also assigned default colors, editable by changing the **Filler Color** in the Layer Menu. Multiple **Filler** layers can be colored separately by choosing different colors, but they are by default assigned different shades.

- When drawing the Filler, the **Filler InterRampAngle (IRA)** and **Filler Bench Face Angle (BFA)** from the **Project Settings** are used. Ramp widths and slope angles for **Filler** material can be different to in situ (Cutter) material properties.  When drawing the **Filler**, the slope of the stack can be determined using the **Project Settings' Filler InterRampAngle (IRA)** and **Filler Bench Face Angle (BFA)**, or the **Geotech** layer IRA and BFA.

![Image](/image/Figure 7 16 Drawing Window Filler Layer Properties Before Cut Contours With Cutter-Filler.jpg)

![Image](/image/Figure 7 17 Drawing Window Filler Layer Properties After Cut Contours With Cutter-Filler.jpg)


- In the **Drawing Window**, you can edit the **Filler** layer's properties. After clicking the button **Cut Contour** using **Cutter/Filler Main Menu**, the Cutter layer's properties cut fill num, **Phase Name (pn)**, **Drection (dir)**, **Min ow**, and **Max ow** are written. The **Phase Name (pn)** for each shape is assigned to the **CutterResult** layer, which will be a 'Fill' type record using the Filler material density and swell specified in the **Schedule Settings** section of the **Project Settings** window.


- If a DXF file is to be imported into a **Cutter** layer, it must be imported individually into an empty Cutter layer (see **Dropdown Menu File/Clear Layer**). It can then be saved as a Cutter JSON file.



#### BaseResult Layer

BaseResult layer features are orange, with lighter orange shading.  The current elevation causes that contour to change to a solid feature with editable vertices and internal shading.

 ![Image](/image/Figure 7 18 BaseResult Layer Coloring.jpg)


 The **BaseResult** layer shows the project surface contours after the pit has been cut (mined), and/or the waste dump and leach pads have been filled. This is the final topography once mining activity is completed, which can be accessed by hitting the keyboard shortcut key, **a**, or by selecting the **All Contours** radio button in **View Settings**.

 By clicking the **Legend** box in the **Legend** portion of the **View Settings** menu, all contours of the **Base** or **BaseResult** layer can be displayed continuously in an overlay when changing elevations (by pressing either **q** or **w**). Press the **a** key to activate the Base or **BaseResult** layer. The **Cut Contour** with **Cutter/Filler** operation populates the **BaseResult** layer.

 **Display/Contour By PM** function is used to create period maps for a given period of mining.  These contours are populated in the **BaseResult** layer for viewing and export.


#### CutterResult Layer

CutterResult layer features are lime colored.

 ![Image](/image/Figure 7 21 CutterResult Layer Cut Coloring.jpg)


The shape shown in the **CutterResult** layer is the result cut polygon representing the material cut (mined) or filled (dumped).  This layer is populated by using the Cut Contour with **Cutter/Filler** operation.  This information is also used in the **Volumetric/Summary** function of the **Dropdown Menu**.

When the Cut Contour function is called, **CutterResult** will be build for the layers selected in the Layer Menu. The **CutterResult** layer is frequently used to stack leachpads.


 ![Image](/image/Figure 7 25 Drawing Window CutterResult Layer Properties For A Filler Type Contour.jpg)


#### Mineplan Layer

The Mineplan layer is used to store a subset of the block model data that exists within the **cutterResult** layer shapes.  The **Schedule / Build** function is used to populate this layer.

Additional properties can also be added/edited in the **Mineplan** layer by clicking the **Project Properties** button in the Main Menu. For more details for the mineplan layer, refer to the Schedule instruction.


 ![Image](/image/Mineplan layer grades and legend color.jpg)


#### Schedule Layer

This layer includes all of the features required for the Schedule. (fleets, location icons, etc.) 
Each schedule Feature can be dragged to its preferred horizontal plane location using the **Main Menu's** Drag features button. While doing this operation, it may be useful to hide other layers to avoid dragging them to undesirable positions. When features are inserted at an elevation indicated in the **Drawing Window**, that elevation is allocated to all features.


## 4.6 Screen Menu

The actions performed on the screen menu have an effect on the content displayed in the Drawing Window. The Screen Menu options are initially retrieved from the Project Settings panel. The button on the far left of the Message bar can be used to collapse or extend this menu.

**NOTE: The Screen Menu settings are temporary and will be lost upon saving and restarting a project. To ensure continuity in a project, the values and options selected/entered will only be retained in the project if they are entered in the Project Settings window button in the Utility Menu.**

![Image](/image/Screen_Menu.jpg)

![Image](/image/Screen_Menu_table_1.jpg)

![Image](/image/Screen_Menu_table_2.jpg)



#### Labels

To make the selected property visible in the **Drawing Window**, select the layer from the dropdown menu and turn it on in the **Layer Menu**.  Layers can contain the same properties, such as data.pn, and all layers that are checked in the **Layer Menu** will display this label.


#### Legend

The Legend allows you to customize the display colors and bins. One legend, with six property options is available.  Individual rows cannot be imported or exported into an existing legend. There is a limit of one Legend Name per project. Legends that are imported and exported should encompass the entire legend for the project.

![Image](/image/Legend.jpg)

To access the legend, click the **Utility Menu > Project Properties** option. The Project Properties screen, which contains the Legend section, will be displayed.

To create a legend in a project, use the following instructions:

1. Click the **Project Properties** button.

2. Enter the Legend name in the **Legend Name** section.

3. Enter the desired shaded property, overwriting the entry in the Property column. The property entry must match the property case and syntax as contained in the Mineplan or Model layer.

4. Enter the numerical bins and shading colors in the **Project Properties** window.

5. Click **Add Legend** button to import a previously exported legend by browsing to the file. Click **Delete** button to remove the imported legend.

6. To save this to the Project, click the **Save Legend** button. Click the **Export** checkbox if you wish to create a saved export file of the Legend for use in another project. You will be prompted to save the Legend with the filename “legend.json”, rename this to “Au_legend.json”. The saved Legend will appear in the dropdown list of saved legends for the project.



7. Check the **Legend** box in the **Screen Menu** of the Drawing Window (or press the keyboard shortcut, **'l'**). Select the Layer containing the desired Property and then select it in the Legend section of the **Screen Menu**.



## 4.7 Message Bar

The Message bar is located between the **Drawing Window** and the **Screen Menu**. 

![Image](/image/message_bar.jpg)


The Message bar displays the follwing information:

- Strike

- Wall angles

- Distances (when the measuring tool is used)

- The easting and northing coordinates, elevation, and position of the bench.

The elevation position indicates whether the contour is at the MidBench, Bench, or NonBench elevation level.

