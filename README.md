Nowadays the drunk and drive cases and the road accidents are happening in the great extent 
due to the uncontrolled driving by the driver. To control these accidents, the proposed system 
namely ‘Alcohol Detection and Engine Locking’ is developed. We have used Arduino UNO as 
a microcontroller, MQ3 sensor to detect the alcohol, Resister to control the current, DC motor, 
Battery, Transistor, LED and Buzzer as an output detection, Breadboard mini to do all the 
required connections and jumper wires to interconnect all the components with each other. 
When the driver is drunk the MQ3 sensor will detect it and the LED will starts glowing and the 
buzzer will ring up. And finally, the engine will get blocked as a result the vehicle will stop 
immediately. 
Keywords: Alcohol detection, Engine Locking, Arduino UNO, MQ3 Alcohol Sensor.
 
As we know India is one of the most populates countries in the world. Most of the percentage 
in this population is covered by youngsters and that is the strength of our country. Nowadays 
number of the drunk and drive cases and the road accidents are increased in the great extent. 
The drivers involving in these cases are mostly the youngsters. These youngsters are addicted 
by the alcohol consumption. Due to this our strength is creating the worst issue to deal with
[1]. As we peep into the records of last few years, we are finding that the death ratio in last few 
years is increased due to the road accidents and drunk and drive cases. This has become a
serious problem. The road safety is decreasing day by day [2]. 
After analysing this scenario, we decided to build up a system namely “Alcohol Detection and 
Engine Locking System”. This system is hardware and software based i.e., an embedded 
system. The main hardware we used is Arduino UNO and MQ3 sensor. For the coding part we 
have used the Arduino IDE software. The coding is done using embedded C language. As per 
the system developed by us, the drunk person is not able to drive the car because of engine 
blocking of the vehicle. Due to the buzzer and the LED the people in inside as well as outside 
the vehicle get an alert of the driver’s condition and the further crisis can be avoided. The main 
objective of this project is to reduce the road accidents as well as the drunk and drive cases. So 
that it helps to improvise the road safety.
LITERATURE REVIEW :
The focus of the paper Automatic Engine Locking System Through Alcohol Detection is on 
creating a hardware device, which detects the alcohol consumption of vehicle driver, to reduce
road accidents. Pravin Shukla et al. [1] focuses on the Alcohol Detection System in Vehicle 
Using Arduino is to represent the project which makes human driving safer and to overcome                             
accidents caused by driving vehicles with alcohol consumption. Sudharsana Vijayan et al. [2]
developed an Automatic Alcohol Detection and Engine Locking System Using Arduino 
NANO is to operate vehicle only by normal person. It provides safety of people outside and 
inside the vehicles. It helps to control accidents as well as rash driving due to alcohol. R. 
Kumudham et al. [3] proposed a system “Drunk and Drive Controller” for Vehicles which was 
used to control accident happening because of driving after consuming alcohol. Gaseous 
material in breath of driver is sense using sensing and output is implemented by sensor. P. 
Manikandan et al. developed a system namely Alcohol Detection and Vehicle Ignition 
Locking System which focuses on to develop a system to avoid accident due to concern of 
alcohol. And mainly temperature and microcontroller are used to detect and implement.
 
The system composed of the following components:
• Arduino UNO
• MQ3 Sensor
• DC Motor
• Bread Board Mini
• Resister
• Buzzer
• Battery
• Transistor
• Jumper Wire
Basically, LED and the Buzzer are the components who will give the alert, or the actual output 
and other components are used for main functioning. 
MQ3 is a sensor which we have used for detection of alcohol. Now sensor detect the presence 
of alcohol it passes signal to the main micro-controller i.e., Arduino UNO board. The microcontroller sends these signals to buzzer and transistor and further these signals are relayed to 
DC motor i.e., Engine through relay. As per the algorithm that we have implemented, that when 
alcohol is detected, the buzzer should buzz, and the DC motor or engine should stop working.
ALGORITHM USED IN THE PROPOSED SYSTEM:
Step 1: 
We have defined the digital pins of microcontroller A0, D9, D8 as sensorDigital, Motor, Buzzer 
respectively.
Step 2: 
These pins are declared as input or output.
Step 3:
Began the serial monitor using user defined function with specific delay.
Step 4:
We have used the If-else loop for the functioning of Motor and Buzzer pin. We are taking 
Boolean type values as input. if the digital==0 then the motor pin will become low, and buzzer 
will become high or else buzzer will remain low and motor will remain high.
RESULTS AND DISCUSSIONS
If the alcoholic person tries to drive the vehicles, the sensor present at the driver seat will detect 
the presence of alcohol and the circuit will get activated. Hence the buzzer will start to buzz,
and the vehicle engine will be turned off.
LIMITATIONS :
1) The driver can hide their alcohol breath will any product.
2) Alcohol sensor can be faked using different perfume which are alcohol free.
FUTURE SCOPE :
Currently, the developed system is in the initial stage. In future, we can use the touch sensor in 
the system so that when the driver will touch the steering automatically the engine will block. 
We can also add the GPS technology to fetch the location of the vehicle as well as we can 
involve IoT technology for more improvement. 
CONCLUSION :
The system “Alcohol Detection and Engine Locking” system is beneficial for the society. It 
will help to reduce the road accidents as well as the drunk and drive cases. So that the road 
safety will increase automatically. The number of deaths will decrease automatically. It’s not 
only helpful to reduce the loss of lives but also helpful to reduce the loss of the properties such 
as roads as well as vehicles. If the accidents will not happen, then the damage of roads will also 
reduce. And it will indirectly affect on the economy of the country it will grow in some manner.
On the other hand, the loss or damage of vehicle will also be stop so that the individual’s 
economic loss is also be prevented. As we know if the drunk and drive or a road accident case 
is happening then there is a legal process and fine or the punishment is also given to the driver 
or the accuse. It leads to the life destroyer also. If the engine gets automatically locked the 
further disaster or the crisis can be stopped. As a result, the life of the driver as well as the loss 
of the others’ lives can be prevented. In short, this system will be helpful to the society in many 
ways such as road safety, economic growth, etc.
