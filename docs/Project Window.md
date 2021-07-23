
# Opencontour Project Window

What you will learn:

- [Overview](#overview)
- [Dropdown Menu](#dropdown-menu)


____________________________________________________________________


## Overview

The Project window is used to create and manipulate opencontour projects using various elements, such as panels, bars, windows, etc. After the project setting is complete, the new project will be created. The project's name and version number are displayed in the upper right-hand corner of the Project Window.

![Image](/image/proejct_window_dashboard.jpg)

In the project window, you can access the following menus:

- Dropdown Menu
- Main Menu
- Drawing Window
- Utility Menu
- Layer Menu
- Message bar

**Dropdown Menu:** A Dropdown Menu is located below the browser address bar. This menu is used to save and open files, configure display parameters, access design features, and access the Help Guide directly. Refer to section XXXX for more details.

**Main Menu:** When a project is opened, the Main Menu appears at the top of the display window. A project can be built using the layer drawing and editing tools available in this menu and running functions.

**Drawing Window:** When a project is open, the Drawing Window is the top area of the display window and the location of the CAD design work. When a project is opened, this section is initially empty until layers are added.

**Utility Menu:** The Utility Menu enables users to make changes to Project Settings, Project Properties, Scheduling, Scripts, Charts, and Reports. These topics are described throughout this document in the order in which they occur procedurally.

**Layer Menu:** The Layer Menu is used to edit individual layers.

**Message bar:** The message bar is used to convey information such as coordinates, elevations, strike angles, wall angles, and distances to the user.

**Additional Option:**

- **Zoom in:** Press **+** button to zoom in. This has the same effect as turning the mouse wheel.

- **Zoom out:** Press **-** button to zoom out. This has the same effect as turning the mouse wheel.

- **Zoom bar:** Dragging this bar up zooms in, dragging down zooms out, dragging up zooms in.

  ![Image](/image/Additional_option.jpg)


### Operations Without Buttons

**Panning**

The user is also able to pan, by holding down the mouse key in the Drawing Window and dragging it to a new location. Panning can also be used to view the entire contents of the Properties display window while viewing a feature's properties.

**Schedule Fill Down in the Schedule Window**

To fill the remining schedule periods with a value, type the value in a blank entry box (for either the Mine Constraint or Process Limit).Select the value, right-click and choose either Copy Up or Copy Down.

**Rotate View**

Holding down the **Alt** and **Shift** keys on the keyboard and panning with the mouse will rotate the view displayed in the Drawing Window. 

**Copy a Selected Feature in the Drawing Window**

Use the **Select Feature** button to select a single feature in the active layer. Right-click in the **Drawing Window** to copy. You can also copy an entire layer by selecting the **Copy All To** from Design Dropdown Menu, Refer to section XXXX for more details.

Features may be copied from an active layer to inactive layer. To do this, first select the feature and then right-click on it.

Follow the below method:

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

- A list of current projects. Click the **New Project** button to initiate a new project. Additionally, you can reopen a previous project by clicking the project name given underneath the New Project option.

- User Name at the top of the window.

- Version release information is located in the top-right corner of this screen (date of last software update).  

- Logout (press either of the Logout words).  You can change users by going back to the login credentials screen.  


### File

The file menu is used to handle files and project activities. Click on the term **File**. The extended Dashboard will appear.

  ![Image](/image/File_extended.jpg)


##### File > Open Project Tab

This option will launch a new browser tab pre-loaded with Opencontour. The page will serve as a welcome page for selecting or creating projects.

##### File > Clear Project

When selected, the current project will be closed and all layers in the Layer Menu will be cleared. The same project will remain open, with no layers loaded.


##### File > Open

This option inserts a layer into a project and assigns it to the provided location in the file. Click **Open** from the file menu and select the file. This option can be used in place of the 'drag and drop' feature in the Dropdown Menu. The file location is specified by the **la** property in the JSON file when it is stored.


##### File > Save Layer

A layer can be exported from Opencontour as a JSON file once it is created and active in the Layer Menu. 

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

  Saving the group file will save the inputs in the Leach/Stacking Module, Grid tab, the Legend, Grid Settings and Charts. 

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


**Phase Name**: It functions similarly to the Filler/Cutter option, except that each line of data will include the Phase Name (pn). The similarities between cut fill num and pn can be noticed in the detail report.

  ![Image](/image/Volumeteric summary_2.jpg) 


**Bench**: The Bench option makes use of elevation (z), but does not provide information about the initial cut fill num or pn.

  ![Image](/image/Volumeteric summary_3.jpg) 


##### Display > Contour By PM

This function can be used after a schedule run for a project with pits. 

1. Click **Display > Contour By PM**. The Contour By Period Mined window appears.

    ![Image](/image/ContourByPM.jpg) 

You can enter a period number (e.g. 5) or a date in the Period Mined (pm) entry box. The single down arrow displays a calendar, while the other increments the current date.

Fillers can obstruct Cutters if they are positioned on top of each other.  Hence, there is a choice for their display.  This is apparent in pits where backfilling practices are used.

When the Filler and Cutter layers' checkboxes are checked, this function creates contours in the BaseResult layer for them.


##### Display > Grid Settings

Grid settings are used to include grids in the project.

1. To select the grid interval, Click the **Display > Grid Settings**. 

  ![Image](/image/Grid_settngs.jpg) 

&nbsp;
2. Click the **Save** button.  The View Latitude and Longitude button on the Main Menu will be activated. To bring the display to a halt, push the View Latitude and Longitude button until it turns green. The following sections cover each option in the Gridline Settings box.


**Scale Bar** 

If the Scale Bar is enabled, it will be displayed in the Drawing Window's lower left corner. The value displayed in the bar and the spacing between the gridlines are adjusted by zooming in and out with the mouse.

  ![Image](/image/grid_settings_scale_bar.jpg) 


**Compass** 

If the compass is shown, it will appear in the upper right corner of the Drawing Window.  The arrow vertices towards the North.

  ![Image](/image/grid_settings_compass.jpg) 


**Labels**

Northing and Easting intervals are displayed by ticking the Labels: box in Display/Grid Settings

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


**NOTE : Display/3D can be utilised with virtual reality glasses if your computer is configured properly. If you do not, a message such as "WEBVR NOT SUPPORTED" may appear in the lower section of the screen.**

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
