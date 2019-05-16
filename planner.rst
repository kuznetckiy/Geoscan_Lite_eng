Geoscan Planner
==============================

Preset
-----------------------------------

1) Connect RCL modem to the notebook.
2) Turn on UAV power.
3) Run application **MdmDisp**.

In the lower right corner of the screen, the antenna icon and the number of connected aircrafts are displayed.

.. figure:: _static/_images/planner1.png
   :align: center
   :width: 100

   MdmDisp program indicator

3.1 At the first time you need to configure connection with UAV. 

Run **NetTopology**:

* Click on the icon **Search**.

.. figure:: _static/_images/planner29.png
   :align: center
   :width: 200

   Search icon


The program shows a list of detected modems.

.. note:: The button is fixable, so it should be pressed again to stop searching.

* Choose UAV №xxx and click on the icon **Add device**.

.. figure:: _static/_images/planner30.png
   :align: center
   :width: 300

   Add device

The program saves the list of added devices.

When re-flying, just run **MdmDisp** and make sure that the connection is successful.

If UAV is not detected, you can reconnect the RCL modem by clicking **Reconnect** in context menu.

.. figure:: _static/_images/planner2.png
   :align: center
   :width: 150

   Context menu MdmDisp

4) Run program **Geoscan Planner**.
5) Enter your login and password.
6) For UAV connection select the drop-down menu **Flight – Connect to the UAV – Search...**.

.. figure:: _static/_images/planner3.png
   :align: center
   :width: 500

   Connect UAV

7) Select type of connection **MdmDisp**. Set **IP-address** *localhost*. In **Vehicle** list set **UAV - Port 6**.

.. figure:: _static/_images/pl4.png
   :align: center
   :width: 500

   Connect UAV

.. note:: It is enough to set the parameters once. Next time when you connect your UAV click **Connect the UA** on the toolbar. The receiver will automatically detect the coordinates and display the UAV location on the map. The telemetry panel (left) and the instrument panel (right) appear in the program window.

.. figure:: _static/_images/pl5.png
   :align: center
   :width: 300

   Connect UAV


Creating a flight task
----------------------------------------

1) Create**New project**.

.. figure:: _static/_images/planner5.png
   :align: center
   :width: 400

   New project creation

2) Set project name, shooting parameters, UAV and camera.

.. figure:: _static/_images/planner6.png
   :align: center
   :width: 500

   Project parameters


Areal surveying
-------------------------------------------

Areal surveying is an aerial photography of polygons. Polygon is an area, bounded by polygon. The operator sets the vertices of the polygon, and the program automatically calculates the route for UAV.

1) Click on the icon **Create areal surveying** on the toolbar.

.. figure:: _static/_images/planner8.png
   :align: center
   :width: 300

   Areal surveying creation

2) By single mouse clicking specify the angular points of the research site. The program automatically calculates the route for bypassing the polygon.
It is enough for the operator to create a polygon directly along the boundaries of the investigated area, the program will increase the length of the overfights and their number in accordance with the survey conditions by itself.
When constructing a route, a rising and a lowering of UAV is displayed as the cylinders if the difference in heights of neighboring points is not less than 30 meters.

.. figure:: _static/_images/planner9.png
   :align: center
   :width: 500

   Цилиндры набора высоты и снижения

Adding and removing polygon vertices.
__________________________________________

You can add vertices to the completed polygon.

1) Hold the left mouse button and move the middle point of the polygon side.

.. figure:: _static/_images/planner10.png
   :align: center
   :width: 500

   Adding the vertex

The vertex will be created automatically.
In a floating window near the vertex will display its coordinates.


.. figure:: _static/_images/planner34.png
   :align: center
   :width: 500

   Result of adding a vertex

To remove vertex:

1) Click right button on vertex.
2) In menu select **Remove vertex**.

.. figure:: _static/_images/planner33.png
   :align: center
   :width: 500

   Remove vertex

Changing the direction of the route lines.
_____________________________________________

The necessary of optimizing polygon "by the direction" occurs quite often, for example, if the force and direction of the wind are unfavorable at the site of work (strong wind along the lines of the overflight above the polygon).
To change the type of optimization, right-click on the polygon and select the option **Optimization by “direction”** in the context menu.

1) Right-click on the polygon area.
2) Select **Optimization by “direction”**.

.. figure:: _static/_images/planner11.png
   :align: center
   :width: 500

   Optimization by direction

One of the vertices of the polygon will be highlighted and a rotation marker will appear on it to set the direction.

.. figure:: _static/_images/planner12.png
   :align: center
   :width: 500

   Корректировка направления облета

As a Result, there will be a new route to fly around the area in the specified direction.

.. figure:: _static/_images/planner13.png
   :align: center
   :width: 500

   New flight route

Change start point
_________________________________

To change the polygon entry point, follow these steps:

1) Select polygon

.. figure:: _static/_images/planner14.png
   :align: center
   :width: 500

   Selected polygon

2) Right-click to select the point where you want to start circling the area.
3) In menu select **Start here**.

.. figure:: _static/_images/planner15.png
   :align: center
   :width: 500

   Change the polygon entry point

.. |flag| image:: _static/_images/flag.png
    :width: 50

A marker |flag| appears at the selected entry point.



Linear surveying
---------------------------
Linear aerial photography is performed in order to survey linear extended objects, such as: rivers, roads, power lines, oil pipelines.

1) Click on the icon **Create linear surveying** on the toolbar.

.. figure:: _static/_images/planner16.png
   :align: center
   :width: 300

   Linear surveying creation

2) Single-click to specify the route of traversing the extended object by turning points. The program will automatically draw lines of flight.

.. figure:: _static/_images/planner17.png
   :align: center
   :width: 500

   Example of linear surveying


Hop
----------------
Fight by pre-set route with a set altitude. It is mainly used for passing around point objects (i.e. high objects) and topographic inequality.

1) Click on the icon **Create hop** on the toolbar.

.. figure:: _static/_images/planner19.png
   :align: center
   :width: 300

   Hop creation

2) Specify the flight route by single-clicking. To build a hop at different altitudes, select **Optimization - Custom altitude** in “Properties” window.

.. figure:: _static/_images/planner20.png
   :align: center
   :width: 500

   Hop creation

** Non zero photo step** function activates the camera.

You can change the step of photo in meters is specified in the corresponding field.
Values of the Alt. AGL column are the differences between the absolute height of the flight task point and the relief below it. Thus, the height of the relief must be taken into account. The absolute heights of the points are also available for editing through the column Alt. WGS84. Besides, height can be changed by visual editing (drag mouse with Shift key pressed).

Hop route between two flight elements is built according to the following rules: 

1) If the flight elements have the same height, then the flight will be performed at the same height.
2) If the fight elements have different heights, then the flight will be performed at the highest of them.

.. attention:: If conditions do not allow to reach the height of the second point by a straight trajectory (for example, due to small distance between points, but a large difference in altitude), the aircraft will fly with the maximum allowable pitch by a straight trajectory in order to reach a point by the coordinates, after which it will rise/descend in a spiral.

Waiting point
------------------------
Waiting point serves to hold the indicated point at the specified altitude during
the specified time interval. Also, waiting point allows to measure the direction
and force of the wind at a specified altitude.

1) Click the button **Create waiting point** on the toolbar.

.. figure:: _static/_images/planner22.png
   :align: center
   :width: 300

   Waiting point creation

2) Click and specify the point, where a waiting should take place.

In expert mode properties may be changed:
setting an altitude of the waiting point, the waiting time and activation of the
wind measurement function.

.. figure:: _static/_images/planner23.png
   :align: center
   :width: 500

   Waiting point options

The UAV will hold the point for the specified time (300 seconds by default) at the specified height, and then go along the planned route.

When ** Wind measure ** is activated, the duration is automatically set to 0. The last point will turn yellow. The UAV flies in a circle, taking into account wind measurements.

.. figure:: _static/_images/planner24.png
   :align: center
   :width: 500

   Точка измерения ветра

Функция бесконечного ожидания служит для постоянного удержания точки (пока не сработает отказ по низкому заряду АКБ, приводящий к автоматическому возврату). При этом цвет точки ожидания сменяется на темно-синий.

.. figure:: _static/_images/planner25.png
   :align: center
   :width: 500

   Точка бесконечного ожидания

.. attention:: It is recommended to set a point of waiting with the wind measurement before each flight element at an altitude of the flight element. Taking into account the wind measurement data, UAV will go smoother along the route.

Landing route
--------------------------------
Command **Create landing** is used to make a landing route.

Building a landing route is an indispensable action at the stage of preparing a flight task.

On arrival at the survey area, determine the wind direction, correct if necessary
the zone of 
ight and select the landing site.
For landing should be chosen an open space without water bodies, trees and other obstacles. The landing site should be  at, preferably with a grass cover.

1) Click on **Create landing** icon on the toolbar.

.. figure:: _static/_images/planner31.png
   :align: center
   :width: 300

   Landing route creation

2) By single-clicking select the landing point first, and then the point of landing approach.

Program automatically creates the landing route, which consists of 3 points (the middle point is created automatically).

.. figure:: _static/_images/planner32.png
   :align: center
   :width: 500

   Example of landing

.. attention:: It is necessary that the landing is being performed against the wind. Otherwise, a hard landing is possible, leading to the aircraft damaging.


Pre-launch preparation
----------------------------

1) Launch **Start preparing Wizard**.

.. figure:: _static/_images/planner26.png
   :align: center
   :width: 300

   Start preparing Wizard launch

Follow the instructions of the Start preparing Wizard (most tests are runned automatically).
Set the radius of the automatic parachute detaching and время автономного полета (time in flight without the connection between the GCS and UAV).
After fight preparation completion, place UAV on the launcher.

Flight
----------------------------

1) Click on the icon **Start**.

.. figure:: _static/_images/planner27.png
   :align: center
   :width: 300

   Start

The telemetry panel displays **CATAPULT** mode.


.. figure:: _static/_images/planner28.png
   :align: center
   :width: 400

   CATAPULT mode

.. attention:: It is necessary to switch the UAV to a start mode only after placing it on the launcher. It is forbidden to take and move the UAV after switching to **CATAPULT** mode.

.. attention:: To cancel the switching to Catapult mode, press the cancel button **Cancel**. UAV will be switched to the **Preparation** mode. It will require to go through the flight preparation again.

2) Turn the safety off and activate the launch device, pulling the launching cord.



UAV will take off.


