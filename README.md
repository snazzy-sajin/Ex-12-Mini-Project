# Ex-12 Mini Project

## SMART PARKING SYSTEM USING ARDUINO

## ABSTRACT

Smart parking systems are an important application of embedded systems that help manage parking spaces efficiently and reduce the time spent searching for available slots. This project presents the design and implementation of an Arduino-based smart parking system using ultrasonic sensors, LEDs, and a servo motor.

The ultrasonic sensors continuously detect whether vehicles are present in the parking slots by measuring the distance between the sensor and the vehicle. The Arduino microcontroller processes the sensor values and determines whether each parking slot is occupied or available. LEDs are used to indicate the status of the parking spaces.

When a vehicle approaches the entrance, the system checks whether parking space is available. If a slot is available, the entrance gate can be opened automatically using a servo motor. When all parking slots are occupied, the system indicates that the parking area is full.

This system reduces manual monitoring, improves parking space utilization, and provides a simple and cost-effective solution for smart parking management. The project demonstrates the integration of Arduino, ultrasonic sensors, LEDs, and servo motor control.

## CHAPTER 1 – INTRODUCTION

Smart parking is a system designed to efficiently manage available parking spaces using sensors and automation. In conventional parking systems, drivers may spend significant time searching for vacant spaces, which can result in traffic congestion and unnecessary fuel consumption.

In this project, an Arduino UNO is used as the main controller. Ultrasonic sensors are placed at individual parking slots to detect the presence of vehicles. The sensors send distance information to the Arduino, which processes the readings and determines whether a parking slot is occupied or available.

LED indicators are used to display the status of each parking slot. A green LED can indicate an available slot, while a red LED can indicate an occupied slot. A servo motor can also be used to control the entrance gate automatically.

The system provides a simple, low-cost, and efficient solution for parking management and can be used in small parking areas, colleges, offices, shopping centers, and residential buildings.

## Objectives

The main objectives of the Smart Parking System are:

* To detect the presence of vehicles in parking slots automatically.
* To identify available and occupied parking spaces.
* To provide visual indication of parking slot status.
* To automatically control the parking entrance gate.
* To reduce manual monitoring and parking search time.
* To develop a simple and low-cost smart parking system using Arduino.

## CHAPTER 2 – LITERATURE SURVEY
<img width="412" height="507" alt="image" src="https://github.com/user-attachments/assets/921372e7-0db2-4129-bb91-ebbd1d0860fa" />


Traditional parking systems require drivers to manually search for available parking spaces. This can result in increased traffic, fuel consumption, and inconvenience, especially in crowded parking areas.

Modern smart parking systems use sensors and microcontrollers to automatically monitor parking spaces. Ultrasonic sensors are commonly used because they can detect objects by measuring the distance between the sensor and the object.

Microcontrollers such as Arduino can process sensor data and control indicators or gates according to parking availability. LED indicators can provide a simple visual representation of whether a parking slot is free or occupied.

Arduino-based smart parking systems are widely suitable for educational and small-scale automation projects because they are simple, affordable, and easy to implement.

## CHAPTER 3 – PROPOSED METHODOLOGY

The proposed smart parking system consists of the following main components:

* Arduino UNO
* Ultrasonic Sensors
* Servo Motor
* Red LEDs
* Green LEDs
* Buzzer
* Jumper Wires
* Breadboard
* Power Supply

The ultrasonic sensors are positioned near the parking slots. They measure the distance to detect whether a vehicle is present. The Arduino receives the sensor readings and compares them with a predefined distance threshold.

If a vehicle is detected within the threshold distance, the corresponding parking slot is considered occupied. If no vehicle is detected, the slot is considered available.

The LEDs display the parking status, while the servo motor can be used to control the entrance gate.

## CHAPTER 4 – HARDWARE DESCRIPTION

## ARDUINO UNO

Arduino UNO is a popular microcontroller board based on the ATmega328P. It provides digital and analog input/output pins and can be programmed using the Arduino IDE.

In the smart parking system, the Arduino UNO receives distance information from the ultrasonic sensors and processes the data to determine the status of each parking slot. It also controls the LEDs, buzzer, and servo motor.

### Features:

* Arduino UNO Microcontroller
* ATmega328P processor
* 14 Digital I/O pins
* 6 Analog input pins
* USB connectivity
* Easy programming using Arduino IDE
* Low-cost and low-power operation

The Arduino UNO acts as the main controller of the smart parking system.

## ULTRASONIC SENSOR

The ultrasonic sensor is used to detect the presence of vehicles in the parking slots. It works by transmitting ultrasonic waves and measuring the time taken for the waves to return after hitting an object.

The Arduino uses the measured distance to determine whether a vehicle is present in a parking slot.

When the measured distance is below the predefined threshold, the slot is considered occupied. Otherwise, it is considered available.

## SERVO MOTOR

The servo motor is used to control the parking entrance gate. It can rotate to a specific angle based on the signal received from the Arduino.

When parking space is available, the Arduino can rotate the servo motor to open the gate. After the vehicle passes through, the servo can return to its original position.

## LED INDICATORS

LEDs are used to indicate the status of parking slots.

A green LED indicates that a parking slot is available, while a red LED indicates that the slot is occupied.

These visual indicators allow users to quickly identify available parking spaces.

## BUZZER

The buzzer provides an audio indication when required. It can be activated when all parking slots are occupied or when a vehicle attempts to enter a full parking area.

## JUMPER WIRES

Jumper wires are used to establish electrical connections between the Arduino, ultrasonic sensors, LEDs, servo motor, buzzer, and other components.

## POWER SUPPLY

A suitable power supply provides electrical power to the Arduino and other components of the smart parking system.

The power supply should provide the appropriate voltage and current required for reliable operation of the sensors, LEDs, and servo motor.

## CHAPTER 5 – SOFTWARE IMPLEMENTATION

The system is programmed using the **Arduino IDE**. The program continuously reads the distance values from the ultrasonic sensors and processes them using the Arduino UNO.

The Arduino determines whether each parking slot is occupied or available based on a predefined distance threshold.

### The program performs the following steps:

● Initialize the Arduino and connected components.

● Initialize the ultrasonic sensors.

● Read the distance measured by each sensor.

● Compare the measured distance with the predefined threshold.

● Determine whether each parking slot is occupied or available.

● Turn ON the appropriate LED indicator.

● Calculate the number of available parking slots.

● Open the entrance gate using the servo motor when space is available.

● Activate the buzzer when all parking slots are occupied.

## CHAPTER 6 – WORKING PRINCIPLE

The Smart Parking System works by using ultrasonic sensors to detect vehicles in individual parking slots.

Each ultrasonic sensor continuously measures the distance between itself and the vehicle or surrounding object. The sensor sends the measured information to the Arduino UNO.

The Arduino compares the measured distance with a predefined threshold value. If the detected distance is less than the threshold, a vehicle is considered to be present and the parking slot is marked as occupied.

The corresponding red LED is turned ON to indicate that the slot is occupied. If no vehicle is detected, the slot is considered available and the green LED is turned ON.

The Arduino also checks the overall parking availability. If at least one slot is available, the entrance gate can be opened using the servo motor. If all slots are occupied, the gate remains closed and the buzzer can be activated to indicate that the parking area is full.

Thus, the system automatically monitors parking spaces and provides real-time parking status.

## CHAPTER 7 – APPLICATIONS

The Smart Parking System can be used in various applications such as:

● Shopping malls

● College and university parking areas

● Office buildings

● Hospitals

● Residential apartments

● Hotels

● Railway stations

● Airports

● Public parking areas

● Smart city parking systems

The system can also be used as an educational project to demonstrate sensor-based automation and embedded system applications.

## CHAPTER 8 – RESULTS AND DISCUSSION

The developed Arduino-based Smart Parking System successfully detects the presence of vehicles in the parking slots using ultrasonic sensors.

When a vehicle occupies a parking slot, the corresponding ultrasonic sensor detects the vehicle and sends the distance information to the Arduino. The Arduino processes the sensor value and changes the parking status to occupied.

The red LED is activated for an occupied slot, while the green LED indicates an available slot. The system also determines the total number of available parking spaces.

When parking space is available, the servo motor can be used to open the entrance gate. When all parking slots are occupied, the system indicates that the parking area is full using the buzzer.

The results demonstrate the successful integration of Arduino UNO, ultrasonic sensors, LEDs, servo motor, and buzzer to create a simple and efficient smart parking system.

## CHAPTER 9 – CONCLUSION AND FUTURE SCOPE

## Conclusion

The Arduino-based Smart Parking System was successfully designed and implemented. The system automatically detects the presence of vehicles and determines the availability of parking spaces using ultrasonic sensors.

The project helped in understanding the working of ultrasonic sensors, Arduino UNO, LEDs, servo motors, buzzers, and embedded system programming.

The system provides a simple, reliable, and cost-effective solution for monitoring parking spaces and reducing the time required to find available parking.

## Future Scope

The system can be further improved by adding IoT features for remote monitoring of parking spaces. A mobile application can be developed to display real-time parking availability.

RFID or QR-code-based vehicle identification can also be integrated to automate vehicle entry and exit. An LCD display can be added to show the number of available parking slots.

Cloud-based monitoring, automatic payment systems, number plate recognition, and multiple parking levels can also be incorporated in future versions to create a more advanced smart parking management system.

## OUTPUT

<img width="603" height="381" alt="image" src="https://github.com/user-attachments/assets/bace8bd4-5903-4b31-94dc-6dd9f5d87092" />


The Smart Parking System successfully detects the availability of parking slots using ultrasonic sensors. When a vehicle is detected, the corresponding slot is marked as occupied and the red LED is activated.

Available slots are indicated using green LEDs. The Arduino continuously monitors the parking area and updates the status of each slot.

When parking space is available, the servo motor can open the entrance gate. When all slots are occupied, the system indicates that the parking area is full.

Thus, the system successfully provides automatic parking slot monitoring, reduces manual effort, and improves the efficiency of parking management.
