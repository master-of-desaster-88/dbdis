# dbdis
Full screen telemetry window for Jeti Transmitter to display all kind of sensors for helis, aeroplanes and drones  
Latest Version: **2.0**

It bases on the Jlog script  from nichtgedacht: https://github.com/nichtgedacht/JLog-Heli 
  
The dbdis app is specially designed for the jeti transmitters with a coloured display.  
For example the min. values are green, max. values are blue and the alarm values are red, but you can easily change it, how you like them.  
  
* Translations in German and in English available
* Multible Sensors from different devices selectable  
* Free selection of Device ( JLog2.6, S32 and compatible ) 
* Very easy and fast configuration, most of it is self explaining
* The order of the display values can be changed with arrow keys very easily
* Just values are displayed where you have set a sensor value
* A small design helps to display a lot of values in one window
* You can use a template design to configure the the full screen window of all models similar
* One switch for permanent percent capacitiy announcement  
* One switch for permanent voltage announcement  
* One switch starts/stops software clock  
* One switch resets software clock  
* One audio file for capacity alarm selectable  
* One audio file for voltage alarm selectable  
* Adjustable capacity of main battery  
* Adjustable voltage of main battery  
* Adjustable cell count of main battery 
* Adjustable voltage alarm theshold  
* Adjustable percent capacity alarm theshold  
* Calculates initial charge condition  
* Displays Tail-Gyro values for Vstabi 
* Displays voltage per cell
* Displays flight time and engine time
* Displays and counts the total amount of flights and total flight time
* Displays the turbine status from the TStatus app: https://github.com/ribid1/TStatus
* Displays the value of Calculated Capacity 4.1 for Gas or Electric, if you don't have a sensor installed:  
http://swiss-aerodesign.com/calculated-capacity.html

### Video Links:
[Helicopters](https://youtu.be/Zso-oRc5-Y8)  
[Aeroplane with combustion engine](https://youtu.be/Qo8YZW3CySw)  


### Examples:  
![TDF](https://github.com/ribid1/dbdis/blob/master/TDF.jpg)
![QC650](https://github.com/ribid1/dbdis/blob/master/QC650.jpg)
![Predator](https://github.com/ribid1/dbdis/blob/master/Predator.jpg)
![Polikarpov](https://github.com/ribid1/dbdis/blob/master/Polikarpov.png)

### Installation:
* Copy the dbdis.lua or the dbdis.lc and the folder dbdis in the folder: \Apps
* If you don't want to make any changes in the program code then take the .lc files.
* Maybe you will edit the code sometime then take the .lua files.
  
### Configuration:  

Select Sensor:  
![Select Category](https://github.com/ribid1/dbdis/blob/master/Select%20Sensor.png)

Select Category:  
![Select Category](https://github.com/ribid1/dbdis/blob/master/Select%20Category.png)

Select Sensor Values:  
![Select Sensor Values 1](https://github.com/ribid1/dbdis/blob/master/Select%20Sensor%20Values%201.png)
![Select Sensor Values 2](https://github.com/ribid1/dbdis/blob/master/Select%20Sensor%20Values%202.png)
![Select Sensor Values 3](https://github.com/ribid1/dbdis/blob/master/Select%20Sensor%20Values%203.png)

Setup Announcements:  
(The capacity and percent announcements are used either for the battery as for the fuel)
![Setup Announcements](https://github.com/ribid1/dbdis/blob/master/Setup%20Announcements.png)

Setup Battery:  
![Setup Battery](https://github.com/ribid1/dbdis/blob/master/Setup%20Battery.png)

Setup Time Switches:  
![Setup Time Switches](https://github.com/ribid1/dbdis/blob/master/Setup%20Time%20Switches.png)

Setup History:  
![Setup History](https://github.com/ribid1/dbdis/blob/master/Setup%20History.png)

Design the Layout (use the arrow keys to change the order):  
- Sep.: determine the thickness of the seperator line (0 = no seperator)  

![Layout 1](https://github.com/ribid1/dbdis/blob/master/Layout_1.png)
![Layout 2](https://github.com/ribid1/dbdis/blob/master/Layout_2.png)
![Layout 3](https://github.com/ribid1/dbdis/blob/master/Layout_3.png)

### History:  
  
V1.0 initial release  
V1.1 Turbine status and turbine telemetry added  
V1.2 improvement of the timer function:
- if you activate the reset switch during the timer runs:  
    The actual flight will not count and the timer starts at zero again.    
- if you activate the reset switch during the timer stops, and you have already reached the time limit:  
    The actual flight will be count and the timer starts at zero again an other flight.  
    
- impliment of the CalCa- Gas and the CalCa-Elec App: If you get values from the app they will be used. 

V1.3 select sensors from different devices  
- save the History (fight counts and total flight time in a file) 
  
V1.4 Rx values of 2nd Receiver and Backup Receiver added  
V1.5 2nd Battery added  
V1.6 moved the drawfunctions in the screen modul  
V1.7 Central box added  
V2.0 Second Form to change the order of the boxes added  
