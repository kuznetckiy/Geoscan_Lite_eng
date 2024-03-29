Charger and battery
=========================

.. csv-table:: **Parameters of battery**
   
   "Guaranteed number of charge-discharge cycles", "50"
   "Max charge limit", "16.8 V"
   "Min discharge limit", "13.2 V"
   "Charging current", "<10 А"
   "Number of cells", "4"
   "Capacity", "10 000 mAh"


Safety requirements
----------------------

**Battery**

* Avoid depressurization and deformation of battery elements (don't drop, don't pierce).
* Do not allow the battery to heat more than 60 degrees.
* Avoid overcharging the battery (over 16.8V). Do not allow the battery discharge below 12V.
* Do not store the battery in a discharged state. For long-term storage of the battery (more than a month) it must be transferred to the **Storage** mode by the battery charger.
* Do not charge with currents exceeding the load capacity (not more than 100% of the capacity, it is recommended to charge 50% of the capacity to extend the service life). Exceeding the permissible charge current will heat the battery over 60 degrees.

.. attention:: Failure to comply with the above instructions may result in fire or complete failure of the battery.


**Charger**

* The charger must be switched on before connecting the battery to the charger.
* Cables and connectors must be inspected for damage before each use.
* Do not operate the charger in direct sunlight.
* Do not leave the charger unsupervised.

The charger is set up from the factory. If the settings are different, follow the instructions to config preset.

Preset of the battery charger
---------------------------------

Use the charger's touchscreen to configure it. The start screen looks like:

.. figure:: _static/_images/charge1.png
   :align: center
   :width: 400
   :alt: Main menu

**Setting battery charging parameters:**

In section **Type** select **LiPo**:

.. figure:: _static/_images/charge2.png
   :align: center
   :width: 400
   :alt: Type 

In section **Cells** select **4Cells** **14.8V**:

.. figure:: _static/_images/charge3.png
   :align: center
   :width: 400
   :alt: Cells

In section **Mode** select:

* **Balance only** for the battery charge.

* **Storage** to transfer the battery to storage mode.

* **Charge** to charge the battery without balancing the voltage on the elements (not recommended to charge in this mode).

* **Discharge** for battery discharge.

* **Quick Charge** for charging with high currents (not recommended to charge in this mode).

* **Checker** to check battery status.

.. figure:: _static/_images/charge4.png
   :align: center
   :width: 400
   :alt: Mode

In section **Current** choose **Charge: 5.0А**, **Discharge: 3.0А**:

.. figure:: _static/_images/charge5.png
   :align: center
   :width: 400
   :alt: Current

Choose the section **Uset**:

.. figure:: _static/_images/charge7.png
   :align: center
   :width: 400
   :alt: Settings

In section **Uset** set **Cutoff Time** *200 Minute*:

.. figure:: _static/_images/charge6.png
   :align: center
   :width: 400
   :alt: Cutoff Time

In section **Uset** set **Cutoff Capacity** *10.0 Ah*:

.. figure:: _static/_images/charge8.png
   :align: center
   :width: 400
   :alt: Cutoff Time

Battery charging
---------------------
* Connect the AC power cable to the charger.

* Plug the power cord into an outlet.

* Connect the balancing cable to the battery being charged.

* Connect the power cable connector to the battery being charged.

* Check the settings of the charger and start the charge process by long (3 seconds) clicking on the icon **Start**.

* After charging is complete, turn off the battery in the reverse order.

.. figure:: _static/_images/charge9.png
   :align: center
   :width: 400
   :alt: Charging start

Recommendations for lithium polymer (LiPo) battery use 
---------------------------------------------------------------------

**Battery operation rules**

In order to avoid emergency situations related to the abnormal operation of the battery, these rules must be followed:

If the flights are performed at temperatures below 0 degrees, the battery must be stored in a warm place before the flight and avoid being cooled. It should be remembered that lithium polymer batteries can lose up to 30% of its capacity in cold conditions, this fact must be taken into account when preparing the flight task;

If the flights are performed at temperatures above 25 degrees, the battery must be stored in a cool place, protected from direct sunlight before the flight. After the flight, you can not immediately charge the battery, you need to let it cool down. It is also necessary to charge in a cool place, protected from direct sunlight.

Battery check
---------------------------------
To check the battery, it is recommended to perform a full charge/discharge cycle for the battery.

1) Charge the battery.
2) Discharge the battery to 13.5 V by select **Discharge** mode.
3) Re-charge the battery.


Storage and discharge
--------------------------------------------
The storage mode is necessary if you do not intend to use the battery for more than 14 days.

To transfer the battery to the storage mode, you need to change the mode **Balance** to the mode **Storage**, checking the correct number of cells on the screen (4 Cells) and start it with a long press of the button **Start**.

Store in a cool dry place, excluding exposure to direct sunlight, at a temperature of 5 to 25 °C and a relative humidity of not more than 80%, without condensation.

The optimum temperature is from 5 to 10 °C.

Optimal battery voltage level for storing: 15.12 V.

Battery life cycle - 1 year.


Battery recycling
--------------------

.. attention:: Do not dispose of LiPo batteries in household waste containers. 
 Improper disposal of used power sources can be hazardous to the environment.
 Dispose of LiPo batteries in accordance with local regulations and take them to the nearest recycling points.