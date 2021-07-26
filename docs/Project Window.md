
# Opencontour Project Window

What you will learn:

- [Overview](#overview)
- [Dropdown Menu](#dropdown-menu)


____________________________________________________________________


## Overview

The Project window is used to create and manipulate various opencontour projects using various elements, such as panels, bars, windows, etc. After finalizing the **Project Settings**, the new project will be created. The project's name and version number are displayed in the upper right-hand corner of the **Project Window**.

![Image](/image/proejct_window_dashboard.jpg)

In the project window, you can access the following menus:

- Dropdown Menu
- Main Menu
- Drawing Window
- Utility Menu
- Layer Menu
- Message bar

**Dropdown Menu:** A Dropdown Menu is located below the browser address bar. This menu is used to save and open files, configure display parameters, access design features, and access the Help Guide directly. Refer to section [Dropdown Menu](#dropdown-menu) for more details.

**Main Menu:** When a project is opened, the Main Menu appears at the top of the display window. A project can be built using the layer drawing and editing tools available in this menu and running functions. Refer to section XXXX for more details.

**Drawing Window:** When a project is open, the Drawing Window is the top area of the display window and the location of the CAD design work. When a project is opened, this section is initially empty until layers are added. Refer to section XXXX for more details.

**Utility Menu:** The Utility Menu enables users to make changes to **Project Settings**, **Project Properties**, **Scheduling**, **Scripts**, **Charts**, and **Reports**. These topics are described throughout this document in the order in which they occur procedurally. Refer to section XXXX for more details.

**Layer Menu:** The Layer Menu is used to edit individual layers. Refer to section XXXX for more details.

**Message bar:** The message bar is used to convey information such as coordinates, elevations, strike angles, wall angles, and distances to the user. Refer to section XXXX for more details.

**Additional Option:**

- **Zoom in:** Press **+** button to zoom in. This has the same effect as turning the mouse wheel.

- **Zoom out:** Press **-** button to zoom out. This has the same effect as turning the mouse wheel.

- **Zoom bar:** This bar allows you to zoom in and out by sliding it up and down.

  ![Image](/image/Additional_option.jpg)


### Operations Without Buttons

**Panning**

The user is also able to pan, by holding down the mouse key in the **Drawing Window** and dragging it to a new location. Panning can also be used to view the entire contents of the Properties display window while viewing a feature's properties.

**Schedule Fill Down in the Schedule Window**

To fill the remining schedule periods with a value, type the value in a blank entry box (for either the **Mine Constraint** or **Process Limit**). Select the value, right-click and choose either Copy Up or Copy Down.

**Rotate View**

Holding down the **Alt** + **Shift** keys on the keyboard and panning with the mouse will rotate the view displayed in the **Drawing Window**. 

**Copy a Selected Feature in the Drawing Window**

Use the **Select Feature** button to select a single feature in the active layer. Right-click in the **Drawing Window** to copy. You can also copy an entire layer by selecting the **Design > Copy All To** Dropdown Menu, Refer to section XXXX for more details.

Features may be copied from an active layer to inactive layer. To copy from an active layer to an inactive layer, follow the steps mentioned below.

1.	Activate the layer you wish to copy a feature from.

2.	Use the **Select Feature** button, to select the item. The selected item will change to a light green colour.

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

## Dropdown Menu

A Dropdown Menu is located below the browser address bar. This menu is used to save and open files, configure display parameters, access design features, and access the Help Guide directly. 

  ![Image](/image/drop_down1.jpg)


### Project

The Project option is located in the top-left corner of the screen in the Dropdown Menu. Click on the term **Project**. The extended Dashboard will appear.

  ![Image](/image/project_dashboard.jpg)

The dashoboard displays:

- A list of current projects. Click the **New Project** button to initiate a new project. Additionally, you can reopen a previous project by clicking the project name given underneath the **New Project** option.

- **User Name** at the top of the window.

- Version release information is located in the top-right corner of this screen (date of last software update).  

- **Logout** (press either of the Logout words).  You can change users by going back to the login credentials screen.  


### File

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

  Saving the group file will save the inputs in the [**Leach/Stacking**](#leach) Module, Grid tab, the Legend, Grid Settings and Charts. 

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

**NOTE: During the import, the Fix All Polygons function in the Main Menu will run automatically. The Error layer will be used to store errors. To proceed past the error warning, click the x in the upper right corner.**

![Image](/image/polygon_error.jpg)


##### File > Open Model

The Open Model function is used to import **models** and **mineplans** into a project. 
After selection, the user is required to specify the directory and file location for the Model. The supported file formats are: 

- JSON
- CSV
- TAM (Typed Array Model)
- Save TAM


**NOTE**

- **It is important that all CSV files used for data import are in the 'generic' format (for example, 43914 with no decimals for the pm property). Commas should not be used as thousand delimiters in data records (including grades).**

- **Dates should be entered in the Excel format m/d/yyyy.** 

To import a CSV file:

1. Click **File > Open Model > CSV** and import the Model or Mineplan layer.

  ![Image](/image/CSV_IMPORT.jpg)
&nbsp;
2. Enter the following details.

  ![Image](/image/CSV__element_details.jpg)

&nbsp;
3. After addressing each entry, click **Import**.


##### File > Save As PDF

This function is used to create a PDF file for plotting. Everything that is presented in the Drawing Window will be captured and saved. Objects should be centred to be included in the popup prompt's scale.

1. Click **File > Save As PDF**. The Print PDF window appears.

  ![Image](/image/save_as_PDF.jpg)

&nbsp;
2. Each entry in this template is configurable, including the Size and Scale options.

&nbsp;
3. Click **Print** to save the file as a PDF.



### Display

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

The **Summary By** provides three option to filter:

- Filler/Cutter

- Phase Name 

- Bench 

**Filler/Cutter**: It summarises the cut and fill areas, volumes, and mass and generates a file with a calculation for each cut fill number.

  ![Image](/image/Volumeteric summary_1.jpg) 


**Phase Name**: It functions similarly to the **Filler/Cutter** option, except that each line of data will include the Phase Name (pn). The similarities between cut fill num and pn can be noticed in the detail report.

  ![Image](/image/Volumeteric summary_2.jpg) 


**Bench**: The Bench option makes use of elevation (z), but does not provide information about the initial cut fill num or pn.

  ![Image](/image/Volumeteric summary_3.jpg) 


##### Display > Contour By PM

This function can be used after a schedule run for a project with pits. 

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

  ![Image](/image/3D_Option.jpg) 

The 3D view options are:

- **Contour Lines** – for viewing the contours as 3D strings. It has the capability of showing the layers in a Spin mode, with a variable Speed bar.  

-	**Surface** – displays the contours as an opaque overlay.

-	**Section** – shows a sliced view from a selected vantage point. It allows the user to change the view by using the Change View option from the Display menu.

-	**Timeline** – animation of the project for the project life.


The new browser tab displays the menu items in the screen's top-left corner.

  ![Image](/image/3D_new_browser_tab.jpg) 


  ![Image](/image/3D_newtab_elementDetails.jpg)


**NOTE : Display/3D can be utilized with virtual reality glasses if your computer is configured properly. If you do not, a message such as "WEBVR NOT SUPPORTED" may appear in the lower section of the screen.**

**Sample 3D Images:**

- Display/3D Browser Tab Displaying Contour Lines

  ![Image](/image/3D_sampleImage_1.jpg)
  
- Display Tab Options

  ![Image](/image/3D_sampleImage_2.jpg)

- Display/3D Browser Tab Displaying Surface

  ![Image](/image/3D_sampleImage_3.jpg)

- Display/3D Browser Tab Displaying Section

  ![Image](/image/3D_sampleImage_4.jpg)

- Display/3D Browser Tab Displaying Timeline

  ![Image](/image/3D_sampleImage_5.jpg)




### Design

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

**NOTE: The order and positions of the layers listed in the Layer Menu can be rearranged, but any changes will not be saved.**

  

##### Design > Organize Fillers

in-progess....



### Leach

The **Leach** in the Dropdown Menu enables access to the Stacking Module, Cell Model, and Lab Plots options.

  ![Image](/image/Figure 4 50 Dropdown Menu, Leach Options.jpg)


##### Leach > Stacking Module  

Stacking Module is used to assign leach panels to the CutterResult, Model, and Mineplan layers. Leach pads are first designed as Filler layers. These are designed as separate fingers and vertical lifts (each in their own cutter shape). After that, the Cut Contour with Cutter/Filler function is called. Once complete, the fingers are allocated panel and cell numbers via the **Leach > Stacking Module**.

The Stacking Module provide two configuration tab option:

- Home Tab

- Grid Tab

###### Stacking Module > Home Tab

1. Click **Leach > Stacking Module**. The Stacking Module home tab will appears.

  ![Image](/image/Figure 4 51 Dropdown Menu, LeachStacking Module, Home Tab.jpg)


The Home tab displays a status indicator for completed process stages. To learn more about the Leach Stacking Module Guide & Procedures documentation, click on the **?** button to the right of the text Leach Stacking at the top of the window.



The Stacking Module Home tab contains the following button:


- Discretize 

- Populate Mineplan 

- Dispatch 

- Solution 

- Cancel 


######  Color Status

  ![Image](/image/Color status.jpg)


######  Discretize Button

1. The Discretize button separates the CutterResult shapes using the Model layer's grid and adds the block panel properties for each panel to the CutterResult layer. Click [here](#grid-properties) for CutterResult Layer Grid Properties.

    ![Image](/image/Figure 4 52 CutterResult Display Of pn After Running The Build & Discretize Function.jpg)


2. After the Discretize process is complete, a confirmation message will appear, indicating the amount of new blocks created. Select the **OK** option. The Discretize function failed if this message indicates that no blocks were created. If failed, the Model layer and Leach Panel tab entries should be rechecked and the function re-run.  

    ![Image](/image/Figure 4 53 Confimation After Discretize Function Is Run.jpg)


  **NOTE: there is a message warning the user against repeatedly hitting the button if the CutterResult layer has not changed since the previous execution of the Discretize function.**

  ![Image](/image/Figure 4 54 Re-run Warning Message.jpg)



###### Grid Properties

  ![Image](/image/Table 4 2 CutterResult Layer Grid Properties After Pressing Discretize.jpg)



###### Populate Mineplan Button

Discretize will clear the Mineplan layer. To reload the layer: 

1. Click **File > Open Model> CSV** or **JSON**. Select previously saved CSV or JSON file.
2. Click **Populate Mineplan** button. Write the data.dest property to the Mineplan layer from the CutterResult layer to the Mineplan data to be stacked.  For example, data.dest = panel cid from CutterResult layer = d10x5. This function uses stacking order and material type (data.ow). The midx, midy and midz properties will be written to the Mineplan layer when the Populate Mineplan button is pressed.  
3. The Mineplan properties may be plotted in Charts. They are not always visible in the Drawing Window in these coordinate locations.

    ![Image](/image/Figure 4 56  Chart Input Entries Of AuMetal & Otns By Dest After Populate Mineplan Function Run.jpg)

    ![Image](/image/Figure 4 57 Chart AuMetal & Otns By Dest After Populate Mineplan Function Run.jpg)


###### Dispatch Button – used for Month End procedures

The Dispatch button will read the coordinates and quantities from the **CutterResult** layer panels and populate the Mineplan data with the ‘dest’ property.  Any Mineplan data outside the CutterResult shape will not contain an assigned ‘dest’.

The **Contour By PM** function is invoked during the running of the Dispatch function. This function is used to populate period stacked in **CutterResult** for the “Timeline” view .  It writes the pm field from the Mineplan to the CutterResult layer. The Drawing Window allows you to view and reconcile this information.


###### Solution Button

The Solution button will create a Solution layer at the top of the Layer Menu. This layer represents the functionality in turning solution on (on1) and off (off1).

Polygon shapes can be built using the **Add Polygon Features** button, on any elevation of the CutterResult layer, by displaying the CutterResult layer and making the Solution layer active.

  ![Image](/image/Figure 4 58 Active Solution Layer Polygon.jpg)

The polygon and it’s properties will be visible at lower elevations coinciding with the CutterResult layer. The Solution layer will populate the Mineplan layer's on1/off1 properties with a numeric value for each record contained within the **Solution** layer polygon and **CutterResult** shape.  

  ![Image](/image/Figure 4 59 Solution Layer Polygon Properties In Figure 4 58.jpg)

  ![Image](/image/Solution_layer_properties.jpg)

**NOTE:  The polygon must be drawn above the CutterResult's minimum elevation as shown in the Volumetric/Summary By/Bench dropdown menu. A solution polygon will not be visible if the min z property is greater than the max z. The polygon will appear in the Solution layer at the lowest elevation of the CutterResult layer.**

The **Add Polygon** Features button allows you to create a polygon containing the centroids of CutterResult panels. To complete the drawing, double-click the mouse button. You can adjust and save the on1 and off1 dates. They will appear as labels in the Drawing Window if the layer is selected using the on1 or off1 property. These dates for the on1 and off1 properties will be written as a number (general format in Excel, >40000) in the Mineplan layer at the same elevation. if there is Mineplan layer data present at that elevation.

  ![Image](/image/Figure 4 60 Mineplan Layer From Figure 4 59, Displaying Off1 Property.jpg)



###### Cancel Button

Click **Cancel** button to close the Leach Stacking window. The entries will remain in the Leach Stacking window even if the window is closed.



###### Stacking Module > Grid Tab

1. Click **Leach > Stacking Module > Grid Tab**. The Stacking Module grid tab will appears.

    ![Image](/image/Figure 4 61 Dropdown Menu, Leach-Stacking Module, Grid Tab.jpg)

    **NOTE: When a project is saved, the grid tab entries are not retained. All inputs for this tab are saved as part of the Group file. It is recommended to create a new project with distinct Project Settings for designing and scheduling the Leach Module panels.**


2. The **Grid** tab includes a number of project configuration options. Enter the following parmaters from the menu.


    | Project Settings Property               | Grid Tab Parameter Populated                                                              |
    |-----------------------------------------|-------------------------------------------------------------------------------------------|
    | MidBench                                | Z Origin. Click [here](#z-origin) for more details.                                       |
    | BenchHeight                             | Lift Height. Click [here](#lift-height) for more details.                                 |
    | Direction                            | X-,Y-. Click [here](#direction) for more details.



###### Z Origin

The origin specified here should be the lowest elevation of your leach pad necessary to keep the entire pad above the topography. The **Volumetric/Summary By Bench** option in the Dropdown Menu will display the lowest elevation of the shape. This elevation should be selected as the Z Origin. The MidBench entry in the Project Settings will populate the Z Origin initially can be overwritten in this Grid tab.

Example: The minimum Z elevation is 4,100 in the Dropdown Menu’s **Volumetric/Summary By Bench**, write this elevation in your project, 4,100, if the BenchHeight from Project Settings is 15.


###### Lift Height

The BenchHeight parameter in the Project Settings will determine the lift height. This can be changed by overwriting the value in the Grid tab. The grid will appear at every elevation, even if the chosen lift height is 5 times the project's BenchHeight entry.


######	Direction

The **Direction** specifies the direction in which the panel numbers are ordered. Select the direction option from the **X Direction** or **Y Direction** dropdown menu and and then click the radio button to set the dominant direction.
    ![Image](/image/Figure 4 63 Grid Direction Tab X Direction Options.jpg)
    ![Image](/image/Figure 4 64 Grid Direction Tab Y Direction Options.jpg)
    ![Image](/image/Figure 4 65 Grid Tab Direction Portion With X Direction Dominant.jpg)
    ![Image](/image/Figure 4 66 Resultant Panel Numbering, Using Figure 4 65 Inputs..jpg)

&nbsp;
3. You can choose either **Manual Grid** or **Provided Grid** Radio Button . If you selected the Manual Grid radio choice, Enter the following details. For more information regading the **Provided Grid**, refer to [**Provided Grid**](#provided-grid-radio-button) section..



| Project Settings Property               | Grid Tab Parameter Populated                                                              |
|-----------------------------------------|-------------------------------------------------------------------------------------------|
| Block Rotate (degrees clockwise)    | Angle Offset (degrees). For more details, click [here](#angle-offset).                                                     |
| viewExtentMinx                          | X Origin. For more details, click [here](#x-origin-and-y-origin).                                                              |
| viewExtentMiny                          | Y Origin. For more details, click [here](#x-origin-and-y-origin).                                                                             |
| viewExtentMaxx                          | Used in conjunction with the X panel size & X Origin: to calculate the X number of Panels |
| viewExtentMiny                          | Used in conjunction with the Y panel size & Y Origin: to calculate the Y number of Panels |
| Block X                                 | X Panel Size. For more details, click [here](#x-panel-size).                                                                          |
| Block Y                                 | Y Panel Size. For more details, click [here](#y-panel-size).                                                                           |
|                                         | X Number of Panels: = (viewExtentMaxx - viewExtentMinx)/X Panel Size. For more details, click [here](#x-number-of-panels).                      |
|                                         | Y Number of Panels: = (viewExtentMaxy - viewExtentMiny)/Y Panel Size. For more details, click [here](#y-number-of-panels).            |

&nbsp;
######	Angle Offset (degrees)

The Angle Offset (degrees) is used to rotate the alignment of the specified grid when cutting the CutterResult layer.  By measuring the strike of the CutterResult panels this angle entry can be deduced.  An entry of zero represents North used for unrotated leach pad projects. This is initially populated by the **Project Settings**, **Block Rotate** (degrees clockwise).

Example:  A project’s leach panels are rotated such that the measured strike along the Northernmost extent boundary is 121.3. The entry required to align the panels in degrees will be 121.3 – 90 = 31.3.

  ![Image](/image/Figure 4 70 Grid Tab Example Inputs.jpg)

  ![Image](/image/Figure 4 71 Grid Tab Example Results.jpg)




###### X Origin and Y Origin

The X Origin and Y Origin is located in the bottom-left (Southwest) corner of the panels. The Preview button can be used to confirm and relocate this position.


![Image](/image/Figure 4 69 Positioning Of The Grid With All Contours Of The CutterResult Displayed.jpg)

If the **Fix** box is checked, the origin entries will be maintained in the **Preview**.  Unticking this box allows repositioning in the Drawing Window. The **X Origin** and **Y Origin** will be initially populated by the Project Settings; **viewExtentMinx** and **viewExtentMiny**.

Example: Using the **All Contours** display of the CutterResult layer, a **Preview** of the grid position ensures the entire heap leach pad is contained.  Without the Fix box ticked, when the desired position is found simply click the left mouse button to have the entries saved in the Grid tab, which will then reappear.  The X and Y Panel Size, as well as the **X** and **Y Number of Panels** can be reviewed using this tool.



###### X Panel Size


The X Panel Size is initially determined by the entries in the Project Settings for Block X, but may be overwritten.


###### X Number of Panels

X Panel Size and X Number of Panels determines the X direction extent of panels created. The **Preview** tool can be used to determine the combined magnitude of the X Panel Size and the X Panels.

Below is the equation used to determine the X Number of Panels. If this does not equal an integer, the value is rounded to the nearest integer. This integer is susceptible to being overwritten.


        X Number of Panels: = (viewExtentMaxx - X Origin:)/X Panel Size


Example:  Using the All Contours display of the CutterResult layer, a **Preview** of the grid size can be selected to ensure the entire heap leach pad is contained. Each panel written in the X Number of Panels will not be displayed, but the multiplication of the panel size and number will adjust the extents in the X direction.


######	Y Panel Size 

The Y Panel Size is initially determined by the entries in the Project Settings for Block Y, but may be overwritten.


######	Y Number of Panels

Y Panel Size and Y Number of Panels determines the Y direction range of panels. The **Preview** tool can be used to determine the range of the panels in the Y direction.

Below is the equation used to determine the X Number of Panels. If this does not equal an integer, the value is rounded to the nearest integer. This integer is susceptible to being overwritten.

    Y Number of Panels = (viewExtentMaxy - Y Origin)/Y Panel Size


Example:  Each panel written in the Y Number of Panels will not be displayed in the Preview.  The panel size multiplied by the number of panels will adjust the range in the Y direction.  Using the **Preview** tool to confirm the extents.    


######	Preview Button


The Preview button enables the user to view the defined grid's boundaries relative to the CutterResult position of the designed leach pad.  The CutterResult should be displayed in the Drawing Window first, usually displaying All Contours to ensure the entire CutterResult layer is captured.

If the Fix box is checked, the origin will be those written in the Grid tab in the Preview displayed.  Unticking this Fix box allows repositioning in the Drawing Window.

Once the grid is positioned correctly and the left mouse button is pressed, the Grid tab's coordinates will update to reflect the new **X Origin (SW Corner)** and **Y Origin (SW Corner)**. The X and Y Number of Panels, and X and Y Panel Size entries will remain unchanged.



######	Save Button 

Click the **Save** button to save the Grid tab entries to the project. The entries will be recalled with the opening of a saved group file (All (Model), All, Contour Group, Mineplan Group).


######	Build Button

This grid dataset will be used to represent the leach stacking model, which will be written to the Model layer when the **Build** button is pressed. It will be composed of visible points (rather than square polygons) at all elevations. However, the Drawing Window will display grid squares. If constructed manually, each leach elevation will have a grid. It can be saved as a JSON file and reused. Otherwise, it will be saved as a group file All (Model).

  ![Image](/image/Figure 4 72 Model Layer Display After Running Build Function.jpg)





During this process, several properties are written to the Model layer.

  ![Image](/image/Table 4 5 Model Layer Grid Properties After Pressing Build.jpg)


The default nomenclature for the property ‘gid’ is x x y, or 2x10.  If the user would like 'y' to be first for the gid, the **Project Properties** can be used to re-write the gid for the Model layer: 

    gid = data.gy+"x"+data.gx

The mid_x and mid_y are the center points of the grid location and are created in the CutterResult when we discretize. When we run Populate Minelan, these coordinates are assigned to the Mineplan records so that they are viewable    



###### Provided Grid Radio Button


Select the **Provided Grid** radio button to populate the entire grid with data from the imported DXF grid. When the **Provided Grid** radio button is selected, the Inputs Portion entries will be removed from the Grid tab. Manual entry is still required for the **Lift Height**, **Z Origin**, and **Direction Portion**.

  ![Image](/image/Figure 4 73 Example DXF Grid Stored In The Import Layer.jpg)

  ![Image](/image/Figure 4 74 Inputs Entries Will Disappear From The Grid Input Tab When Selecting Provided Grid.jpg)



##### Leach > Cell Model

###### Ore Loading Plan

  ![Image](/image/One_loading_Paln.jpg)


###### Hydrodynamic Characteristics


  ![Image](/image/Hydrodynamic-Characteristics.jpg)



###### Hydrodynamic Characteristics

  ![Image](/image/Extraction-Kinetics.jpg)


##### Leach > Lab Plots

  ![Image](/image/Lab-Plots.jpg)


##### Leach > Add

   ![Image](/image/Figure 4 75  Dropdown MenuÆs Leach-Add Options.jpg)




### Help 

To access the help documentation, visit help.opencontourXXXX.com 

  ![Image](/image/Figure 4 76 Dropdown Menu, Help Options.jpg)

-  **Cheat Sheet**: Provides an overview of the Opencontour layout and techniques.

-  **Help Guide**: Opens a new browser tab with a searchable full Help Guide page.


