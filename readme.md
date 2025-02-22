# Instructions for calculating water access area and meter reading route by QGIS3
I created some customized modeler of QGIS3 for calculating water access area and meter reading route by using QGIS routing functions.
The some data inside geopackage belong to WASAC, Ltd. in Rwanda.

## Extract ZIP file of Geopackage under project folder.

![how to extract zip of geopackage](./images/how%20to%20extract%20zip%20of%20geopackage.gif)

## Install .model3 and .qml file for graphic modeler of QGIS3

First, you need to copy .model3 and .qml file to QGIS's modeler folder. The default path of modeler folder is as follow.

```
%userprofile%\AppData\Roaming\QGIS\QGIS3\profiles\default\processing\models
```

![how to copy model file to folder](./images/how%20to%20copy%20model%20file%20to%20folder.gif)

------

## How to calculate water access area from water points

Second, you need to install QNEAT3 plugin on QGIS3.

![how to install QNEAT3 plugin](./images/how%20to%20install%20QNEAT3%20plugin.gif)

Calculate water access area from water points by modeler.

1. Select target area.
2. Processing --> Toolbox --> Models --> Water --> Create Driving Distance from Water Points
3. Run after selecting road layer and water points layer!

![how to calculate water access area](./images/how%20to%20calculate%20water%20access%20area.gif)

The following figure is the result of calculation.

![water access area result explanation](./images/water%20access%20area%20result%20explanation.png)

The following figure describes how the modeler was built.

![water access area model explanation](./images/water%20access%20area%20model%20explanation.png)

------

## How to create meter reading route by TSP algorithm

First, please open QGIS Desktop 3.10.0 with GRASS 7.6.1.

Don't use QGIS Desktop without GRASS tool.

1. Select target area from WSS layer (Polygon layer).

   ![select_target_area](./images/select_target_area.png)

2. Run Processing --> Toolbox --> Models --> Water --> Create meter reading route by TSP.

   ![select_target_area](./images/run%20modeler%20of%20creating%20meter%20reading%20route.png)

3. Styling network salesman layer to make it be beautiful after completing to run the modeler.

   ![how to styling network salesman layer](./images/how%20to%20styling%20network%20salesman%20layer.gif)

The following figure describes how the modeler was built.

![meter reading route model explanation](./images/meter%20reading%20route%20model%20explanation.png)

------
This tools were developed by ````Jin IGARASHI, JICA Expert```` from ````The Project for Strengthening Operation and Maintenance of Rural Water Supply Systems in Rwanda- RWASOM````.
