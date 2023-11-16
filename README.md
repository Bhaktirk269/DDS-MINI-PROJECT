

# ALCOHOL DETECTION WITH   VEHICAL CONTROLLING SYSTEM

# Team Details
<details> 
<summary> Details </summary> 


Semester :3rd Sem B.Tech.CSE ,
Section: S1,
Team Number:13
Team Members:
1) Bhakti Raju Karchi, 221CS116 ,bhaktirajukarchi.221cs116@nitk.edu.in
2) Hitha N,221CS130, hithan.221cs130@nitk.edu.in
3) P Devi Deepika ,221CS138, pdevideepika.221cs138@nitk.edu.in 


</details>

# Abstract
<details> 
<summary> Details </summary> 




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


# Working
<details> 
<summary> Details </summary> 



Alcohol detection and vehicle control systems are designed to enhance road safety by preventing individuals under the influence of alcohol from operating vehicles. These systems typically incorporate
breathalyzer technology to measure the driver's blood alcohol concentration (BAC). If a driver's BAC exceeds acertain threshold, the system may immobilize the vehicle or prevent it from starting, ensuring a safer driving environment. MQ-3 Alcohol Sensor: The MQ-3 sensor detects alcohol vapor concentration in the air and provides an analog output proportional to the alcohol level.Microcontroller (e.g., Arduino): This will interface with the MQ-3 sensor and process the analog output.LED or Buzzer (Optional): To indicate the status of the alcohol level (e.g., above the threshold). Here we have should use sequential logical gates (flip flops).there
a) Input –clock , alcohol level, rest. 
b) Output- Detection flag, detection counter. 
c) Alcohol level is 0 if alcohol is less than 127. 
d) Alcohol level is 1 if alcohol is greater than 127.


</details>



# Logisim
<details> 
<summary> Details </summary> 


![final logisim](![image](https://github.com/Bhaktirk269/DDS-MINI-PROJECT/assets/129278697/7c4d336e-3da9-46d9-98cf-0eeef9b101c5)



</details>

# Verilog Code
<details> 
<summary> Details </summary> 
  
                    module AlcoholDetection (
              input wire sensor_data,
                output wire alcohol_detected
    );
      // Alcohol detection logic based on sensor_data
    // Set alcohol_detected high if alcohol is detected
    endmodule

    module VehicleControl (
    input wire alcohol_detected,
    input wire ignition_request,
    input wire speed_request,
    output wire ignition_enabled,
    output wire speed_limit
      
      );
    // Vehicle control logic based on alcohol_detected, ignition_request, and speed_request
    // Control ignition_enabled and set speed_limit accordingly
  endmodule

    module AlcoholDetectionVehicleControl (
    input wire sensor_data,
    input wire ignition_request,
    input wire speed_request,
    output wire alcohol_detected,
    output wire ignition_enabled,
    output wire speed_limit

      );
       
        // Instantiate the AlcoholDetection module
        AlcoholDetection alcohol_detection_inst (
        .sensor_data(sensor_data),
        .alcohol_detected(alcohol_detected)
    );

            
            // Instantiate the VehicleControl module
            VehicleControl vehicle_control_inst (
        .alcohol_detected(alcohol_detected),
        .ignition_request(ignition_request),
        .speed_request(speed_request),
        .ignition_enabled(ignition_enabled),
        .speed_limit(speed_limit)
          );
      endmodule



          //Testbench

          `timescale 1ns/1ps

          module tb_alcohol_vehicle;

    // Instantiate the modules
    AlcoholDetection alcohol_detection_inst (
        .sensor_data(sensor_data),
        .alcohol_detected(alcohol_detected)
          );

    VehicleControl vehicle_control_inst (
        .alcohol_detected(alcohol_detected),
        .ignition_request(ignition_request),
        .speed_request(speed_request),
        .ignition_enabled(ignition_enabled),
        .speed_limit(speed_limit)
    );

    // Declare signals for the modules
    wire sensor_data;
    wire ignition_request;
    wire speed_request;
    wire alcohol_detected;
    wire ignition_enabled;
    wire speed_limit;

    // Stimulus generation
    initial begin
        // Initialize inputs
        sensor_data = 0;
        ignition_request = 0;
        speed_request = 0;

        // Apply some test cases
        // Test case 1: No alcohol detected
        // Set sensor_data accordingly
        // Assert expected values for ignition_enabled and speed_limit

        // Test case 2: Alcohol detected
        // Set sensor_data accordingly
        // Assert expected values for ignition_enabled and speed_limit

        // ... Add more test cases as needed

        // Finish simulation after some time
        $finish;
    end

    // Monitor to display outputs
    always @ (posedge alcohol_detected or posedge ignition_enabled or posedge speed_limit) begin
        $display("Alcohol Detected: %b, Ignition Enabled: %b, Speed Limit: %b",
                 alcohol_detected, ignition_enabled, speed_limit);
    end

    endmodule





</details>






