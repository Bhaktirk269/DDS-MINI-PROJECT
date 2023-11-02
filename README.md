

                                          ALCOHOL DETECTION WITH   VEHICAL CONTROLLING SYSTEM

<details> 
<summary> Team Details </summary> 


Semester :3rd Sem B.Tech.CSE ,
Section: S1,
Team Number:13
Team Members:
1) Bhakti Raju Karchi, 221CS116 ,bhaktirajukarchi.221cs116@nitk.edu.in
2) Hitha N,221CS130, hithan.221cs130@nitk.edu.in
3) P Devi Deepika ,221CS138, pdevideepika.221cs138@nitk.edu.in 


</details>


<details> 
<summary> Abstract </summary> 




This project is one of the important Sensor based project ideas. The main unit of this project is an “Alcohol sensor”. If the person inside the car has consumed alcohol then it is alcohol detection is done by the sensor. The sensor gives this signal to a comparator IC. The output of the comparator is connected to the microcontroller.

The microcontroller is the heart of this project. It is the CPU of the complete circuit. The microcontroller gives a high pulse to the buzzer circuit and the buzzer is turned on. At the same time, a relay is turned off. Due to this, the ignition of the car is deactivated. Alcohol Detection System with Buzzer Indication project is extended by adding an ignition key at the input and a DC motor at the output. The input Ignition key is given to the microcontroller. It is used to find out that the car is started. Whenever a key is inserted into the ignition lock at that time the alcohol detection process is started.

Applications of Alcohol Detector in Car:

“Alcohol Detector project” can be used in various vehicles for detecting whether the driver has consumed alcohol or not.
Breathing analyzer projects can also be used in various companies or organizations to detect the alcohol consumption of employees. An alcohol detection system in an automobile is a must feature that every cab or bus should have.

Advantages of the Alcohol Detector project:

“Alcohol Detection System in Cars” provides an automatic safety system for cars and other vehicles as well.

Future Development of the project:

We can implement GSM technology with an alcohol detector. So Alcohol detection & vehicle controlling through text SMS will inform the relatives or owners of the vehicle about the alcohol consumption.

We can implement GPS technology so that once alcohol detection is done, the system will find out the location of the vehicle. This project is called GPS tracker and alcohol detector with engine locking system using GSM.


</details>


<details> 
<summary> Working </summary> 



Alcohol detection and vehicle control systems are designed to enhance road safety by preventing individuals under the influence of alcohol from operating vehicles. These systems typically incorporate
breathalyzer technology to measure the driver's blood alcohol concentration (BAC). If a driver's BAC exceeds acertain threshold, the system may immobilize the vehicle or prevent it from starting, ensuring a safer driving environment. MQ-3 Alcohol Sensor: The MQ-3 sensor detects alcohol vapor concentration in the air and provides an analog output proportional to the alcohol level.Microcontroller (e.g., Arduino): This will interface with the MQ-3 sensor and process the analog output.LED or Buzzer (Optional): To indicate the status of the alcohol level (e.g., above the threshold). Here we have should use sequential logical gates (flip flops).there
a) Input –clock , alcohol level, rest. 
b) Output- Detection flag, detection counter. 
c) Alcohol level is 0 if alcohol is less than 127. 
d) Alcohol level is 1 if alcohol is greater than 127.


</details>




<details> 
<summary> Logism </summary> 


![final logisim](https://github.com/Bhaktirk269/DDS-MINI-PROJECT/assets/129278697/3b65f589-8f1a-462c-8ce7-5da056f97ef3)


</details>


<details> 
<summary> Verilog Code </summary> 





1) [alc.v.txt](https://github.com/Bhaktirk269/DDS-MINI-PROJECT/files/13239353/alc.v.txt)
2) [alc_tb.v.txt](https://github.com/Bhaktirk269/DDS-MINI-PROJECT/files/13239357/alc_tb.v.txt)


</details>






