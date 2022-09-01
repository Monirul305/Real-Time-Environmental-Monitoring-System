# Environmental Monitoring System

**Creators: <br />
Monirul Islam, Dept of EEE, BUET <br />
Fariza Siddiqua, Dept of EEE, BUET <br />
A F M Mahfuzul Kabir, Dept of EEE, BUET <br />
Shuvro Chowdhury, Dept of EEE, BUET <br />**

**This project is for academic evaluation for EEE 416 course in Bangladesh University of Engineering and Technology (BUET).**

Environmental monitoring system using Arduino UNO. The system can sense air quality and temperature and humidly of a location and upload data to thingspeak. 
The system is charged automatically using solar power. The GSM network system uploads live data to server in real time.

The system uses Arduino UNO as the main controlling microprocessor. Three batteries are used for powering up the whole system. 
Two batteries are working in series to power the GSM module and sensors. The last battery is used to power up Arduino.
The GSM module draws high current while connecting to the network. A single battery can't suffice the current need for this system. So, batteeries are connected in
series to provide enough current.
Two charding modules are used to charge three batteries. Relays are used to switch the pararrel batteries to parallel when in charging mode. While discharging, the 
batteries are in series to provide enough power to the GSM. Since the battery output voltage is used while in series, voltage regulator is used so that the modules
are not harmed.

While in work, the system code defines the delay after which the system automatically goes into charging mode. For example, the system can be set to 5 minutes of charging
and then 5 minutes of discharging in loop. During discharging, the system sends data from the sensors to the cloud.
