
# Opencontour Project Window

What you will learn:

- [Overview](#overview)
- [Dropdown Menu](#dropdown-menu)
- [Main Menu](#main-menu)
- [Utility Menu](#utility-menu)



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

  >**NOTE: During the import, the Fix All Polygons function in the Main Menu will run automatically. The >Error layer will be used to store errors. To proceed past the error warning, click the x in the upper >right corner.**

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

>- **Dates should be entered in the Excel format m/d/yyyy.** 

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


>**NOTE : Display/3D can be utilized with virtual reality glasses if your computer is configured properly. >If you do not, a message such as "WEBVR NOT SUPPORTED" may appear in the lower section of the screen.**

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

>**NOTE: The order and positions of the layers listed in the Layer Menu can be rearranged, but any changes will not be saved.**

  

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


  >**NOTE: there is a message warning the user against repeatedly hitting the button if the CutterResult layer has not changed since the previous execution of the Discretize function.**

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

>**NOTE:  The polygon must be drawn above the CutterResult's minimum elevation as shown in the Volumetric/Summary By/Bench dropdown menu. A solution polygon will not be visible if the min z property is greater than the max z. The polygon will appear in the Solution layer at the lowest elevation of the CutterResult layer.**

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

   ![Image](/image/Figure 4 75  Dropdown Menu’s Leach-Add Options.jpg)




### Help 

To access the help documentation, visit help.opencontourXXXX.com 

  ![Image](/image/Figure 4 76 Dropdown Menu, Help Options.jpg)

-  **Cheat Sheet**: Provides an overview of the Opencontour layout and techniques.

-  **Help Guide**: Opens a new browser tab with a searchable full Help Guide page.

<hr>

## Main Menu


The Main menu provides access to tools for creating and editing projects. It enables you to view and control the context of the currently running task or workflow.


  ![Image](/image/Figure 5 1 Main Menu.jpg)


- When a button is available for selection, it is shown in light green ![Image](/image/green_button.jpg). 

- When a button is selected and currently active, it is shown in orange ![Image](/image/orange_buton.jpg). You can deactivate the button by re-selecting it. When the button is not in use, it should revert to its default light green color.

Select the layer from the **Layer Menu** to display the hidden buttons. For additional information, please refer to XXXX.


### Buttons

![Image](/image/button_list.jpg)
<hr>

- **Zoom to full extent** ![Image](/image/Zoom to full extent.jpg): This button will magnified the view to show the full scope of the project. See Help Guide section XXXX 
<hr>

- **Zoom to layer extent** ![Image](/image/Zoom to layer extent.jpg): This button will magnified the view to the active layer extent at the current elevation indicated in the Message bar. See Help Guide section XXXX.
<hr>

- **Up one Level** ![Image](/image/Up one Level.jpg): Move the Drawing Window up in elevation by the BenchHeight value in the Project Settings.  See Help Guide section XXXX to observe use.
<hr>

- **Down one Level** ![Image](/image/Down one Level.jpg): Move the Drawing Window down in elevation by the BenchHeight value in the Project Settings.  See Help Guide section XXXX.
<hr>

- **Copy Cutter Up Level** ![Image](/image/Copy Cutter Up Level.jpg): Expand the pit contour up or down to the next contour’s elevation. It is used when constructing pits, dumps, or leach pads. See Help Guide section XXXX. 
<hr>

- **Cut Contour with Cutter/Filler** ![Image](/image/Cut Contour With Cutter-Filler.jpg):  Use the **Cut Contour with Cutter/Filler** button ![Image](/image/Cut Contour With Cutter-Filler.jpg) on the respective Cutter and Filler layers in the Layer Menu to cut or filled Base topography. This populates two levels automatically: the **BaseResult** layer and the **CutterResult** layer, both of which are saved as part of the Group files. These layers are rewritten each time this button is clicked.




<hr>

- **Add Cutter Layer** : Adds another Cutter layer. Each additional layer will be sequentially numbered and the Phase Name (pn) should be edited for each.  See Help Guide section XXXX.
<hr>

- **Add Filler Layer** : Adds another Filler layer.  Each additional layer will be sequentially numbered and the Phase Name (pn) should be edited for each.  See Help Guide section XXXX.
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
     


 activate the Cutter or Filler Layer from the Layer Menu.  Each vertice will be assigned a sequential number; making it easier to spot kinks, etc.  See Help Guide section XXXX.
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

- **Add Box** : Click this button to add a border around the extents of the topography contours at a selected elevation. Available when Base layer is active.  See Help Guide section XXXX.
<hr>

- **Select feature** : This option enables selection of the desired feature when the relevant layer is selected from the Layer Menu.  See Help Guide section XXXX.
<hr>

- **Select features with a Box**![Image](/image/Select features with a Box.jpg): 

    1. Click the first box corner![Image](/image/Select features with a Box.jpg) to select a feature in the active layer.
    2. Hold the mosuse button and move the mouse to draw the box to the diagonally opposite corner
    3. All features in the active layer that are within or touch the drawn box will be seleced and highlighted in green.
<hr>

- **Add Haul/Load Features** : Click this button and specify the location with a left mouse click to insert a feature that contains an elevation, type, name, availability, utilization, efficiency, and fleet count. Loaders will be given a tnsPerHr productivity rating.  Trucks require rated speeds for gradients that are low, medium, and high & a ‘truckfactor’ (truck payload) & rank.  The units used in the speeds must match those of the project files (i.e. imperial or metric).  
<hr>

- **Add Dump Features** : Click this button and specify the location with a left mouse click to insert a feature that contains an elevation, type, capacity, tns (populated during a schedule run), and name.  Available when Schedule layer is active.  See Help Guide section XXXX.
<hr>

- **Add Phase Features** : Click this button and specify the location with a left mouse click to insert a feature (intersection) that contains an elevation (z), type, name and order.  Available when Schedule layer is active.  See Help Guide Table XXXX.
<hr>

- **Add Stockpile Features** : Click this button and specify the location with a left mouse click to insert a feature that contains an elevation, type, name, a processing order, and a owmin and owmax for determining the values of the Routing variable (data.ow) blocks accepted on that stockpile.  Available when Schedule layer is active.  See Help Guide Table XXXX.
<hr>

- **Add Leach Crush Features** : Click this button and specify the location with a left mouse click to insert a feature that contains an elevation, type, name, a processing order, and a owmin & owmax for determining the values of the Routing variable (data.ow) blocks accepted.  The that feature name must be leach; it must match the filler Phase Name (pn) name of each leach cell (Filler) created.  Available when Schedule layer is active.  Material mined reports here after stockpiling.  See Help Guide Table XXXX.
<hr>

- **Add Leach ROM Features** : Click this button and specify the location with a left mouse click to insert a feature that contains an elevation, type, name, a processing order and a owmin & owmax for determining the values of the Routing variable (data.ow) blocks accepted.  The that feature name must be leach; it must match the filler Phase Name (pn) name of each leach cell (Filler) created.  Available when Schedule layer is active.  Material mined reports directly here rather than via a stockpile.  See Help Guide Table XXXX.
<hr>

- **Add Point Features** : This will add point features to the active layer.  Only available when the Schedule (see section XXXX), Model (see section), or Import (see section XXXX) layers are active. 

<hr>

- **Add Line Features** : When the Roads layer is active, this property becomes available.  This will add lines to those selected layers.  See Help Guide section XXXX.

<hr>

- **Add Polygon Features** : To start drawing polygons or contour lines:

    1. Activate the appropriate layer.
    2. Click the **Add Polygon Features** button. 
    
      Only available when the Base, Cutter, Filler, BaseResult or CutterResult layers are active.  See Help Guide section XXXX.
<hr>

- **Modify features**![Image](/image/Modify features.jpg): 

    1. To add a vertice, click the left mouse button once on the line where the vertice is to be placed. 
    2. To delete a vertice, click the left mouse button once on the vertice to be deleted. 
    3. To move a vertice, hold down the left mouse button and drag the vertice. Release when it moves to the desired location. See Help Guide section XXXX.
<hr>

- **Snap to paths, and vertices** : Allows snapping the cursor to lines and vertices in the Drawing Window for the activated layer.  See Help Guide section XXXX.
<hr>

- **Remove features**![Image](/image/Remove Features.jpg): Delete a feature from the active layer. To delete an entire feature in an active layer:

      1. select **Remove features**![Image](/image/Remove Features.jpg) from the Main Menu.

      2. Select the feature to be removed from the drawing screen. Deselect this button when finished.
<hr>

- **Drag features** : Drag a feature to a different location (but not elevation) in the Drawing Window.  See Help Guide section XXXX.

<hr>

- **Modify Number of Feature Vertices**![Image](/image/Modify Number of Feature Vertices.jpg): If a feature has too many vertices, this will reduce the unnecessary vertices to make the feature easier to work with. To reduce the number of vertices, use the Vertice value in the **View Settings** as the distance between vertices.

      1. Select the active layer.  

      2. Press the **Modify Number of Feature Vertices button** ![Image](/image/Modify Number of Feature Vertices.jpg)

      3.	Select the feature.


<hr>

- **Create Curve**![Image](/image/Create Curve Smoothing A Feature.jpg): A curved line can be created using this tool. The function outcome will depend on the value entered for the Vertice and it is changeable through the **View Settings**.

    1. Activate the feature layer. The feature’s layer must be activated to insert vertices into the curve.

    2. Select a feature in the active layer.  

    3. Click **Create Curve** button ![Image](/image/Create Curve Smoothing A Feature.jpg). The selected feature will be replaced with a curved feature, with vertices inserted as needed. This function is active in layers with features (Base, Geotech, Cutter, Filler & Roads). This function uses the Vertice number written in the Project Settings, or View Settings.  See Help Guide section XXXX.
  

<hr>
 
- **Split Polygon** : Pick one feature, then pick a second feature. The first feature will split the second feature.  The area of the first feature selected inside the second will be maintained. The remainder of the first feature selected can be deleted.  See Help Guide section XXXX.
<hr>

- **Union Two Polygons** : Pick one feature then pick another feature, these two features will join to form a new feature.  If using ramps, the start of the ramp (denoted by the red circle) will be retained for the second feature selected.  See Help Guide section XXXX.
<hr>

- **Set First Poly Vertex** : Moves starting location for ramp (red dot) to vertice on feature specified.  
    1. Draw the feature.
    2. Click **Set First Poly Vertex** button from the Main Menu and click the new position for the inside vertice of the ramp to start from.
    3. Click the button again to exit this function.  See Help Guide section XXXX.

 
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
    
    - Wall Angle: When measuring wall angles, select the line for the 1st mid bench, then select a line for a higher or lower mid bench in the same vertical plane.  See Help Guide section XXXX.

        1. Select a wall contour line for the first mid bench.  The lighter blue line that appears acknowledges the first selection on the 1950 elevation.

        2. Move to the next mid bench using q,![Image](/image/Q.jpg), w, or ![Image](/image/W.jpg). Then select a line perpendicular at a higher or lower mid bench in the same vertical plane. The next mid bench measured here is at the 1945 level.
        3. On selection of the second line, the Message bar will display the wall angle if measured correctly.
        4. Click the **Measure** button to exit the measuring and snapping activities. 

        ![Image](/image/Figure 5 3 Measuring Wall Angle, From (Start) Elevation, 1950.jpg)

        ![Image](/image/Figure 5 4 Measuring Wall Angle, To (End) Elevation, 1945.jpg)

        ![Image](/image/Figure 5 5 Message Bar Display, Wall Angle Shown On The Far Right.jpg)
<hr>

- **View Latitude and Longitude** ![Image](/image/View Latitude And Longitude.jpg): Activates display of latitude and longitude gridlines, scale bar and north arrow. Click **View Latitude and Longitude**![Image](/image/View Latitude And Longitude.jpg) button. The settings selected will be displayed in the Drawing Window. See Help Guide section XXXX.

<hr>

- **Export CSV** : Available for CutterResult, Mineplan & Import layers only.  See Help Guide section XXXX.

<hr>



## Utility Menu

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
####	Project Settings 


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

When the checkbox is selected, the interval will produce a backup of the All (Model) group file, including the Model layer. For example, “April 11, 2019-09.41.00AM pit1 all backup.json” is an example of a file name. If a project _all.json file is loaded the file name will replace “pit1_all” .


#### Project Properties 


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


#### Create Schedule 

To open the schedule window, click **Create Schedule**![Image](/image/Utility_Create Schedule.jpg) button in the Utility Menu. Please refer to section XXXX for more details.

  ![Image](/image/Figure 6 5 Schedule Window.jpg)



#### Create Script 

To open the Script window, click **Create Script**![Image](/image/Utility_Create Script.jpg) button in the Utility Menu.

  ![Image](/image/Figure 6 6 Script Window.jpg)


Scripts can be written to run over the Mineplan before, during or after running a schedule.  The programming language used is JavaScript. To know more about script, refer to JavascriptGuide.pdf


A variable used in a script must either already exist in the layer on which it is working or be defined in the script's previous line. When an error occurs in a script, Opencontour generates error messages to assist the user in identifying the faulty line. If no errors occur, the script will execute with a message. Additionally, This message also tells you how many records are in the layer.

 ![Image](/image/Figure 6 7 Script Run Completion Message.jpg)



#### Create Charts 

To open the charts window, click **Create Charts**![Image](/image/Utility_Create Charts.jpg) button in the Utility Menu. The Mineplan layer is the primary source of data for the charts, after the Schedule has been executed. Please refer to section XXXX for more details.


  ![Image](/image/Figure 6 8 Upper Create Charts Window.jpg)



####	Report Tool


To open the report window, click **Report Tool**![Image](/image/Utility_report.jpg) button in the Utility Menu.

  ![Image](/image/Figure 6 9 Report Window, “report01.json” Loaded.jpg) 


  When executing a report, different browsers may display different export prompts (). Reports are generated over the Mineplan layer by specifying a grouping parameter, for example, "data.pm."


<hr>

## Layer Menu
