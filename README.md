# RISC-V Talent development program

the project is based on the RISC V talent development program.

<details>
  <summary> TASK 0- INSTALLATION</summary>
</details>
<details>
  <summary>
    TASK 1 -DEVELOPMENT OF C PROGRAM
  </summary>

  ### step 1: fire up the terminal 
  ```bash 
  vsduser@vsduser-VirtualBox:~$
  ```

  ### step 2: direction to home bash
  ```bash
  cd
  ```

  ### step 3: open leafpad bash
  ```bash
  leafpad sum1ton.c &
  ```

  ### step 4: write the code
  ```c
  #include<stdio.h>
  int main(){
    int sum = 0, n = 80, i;
    for(i=0; i<=n; i++){
        sum+=i;
        printf("The sum from 1 to 80: %d \n", sum);
    }
    return 0;
}
  ```

  ### step 5: compile and run the code
  ```bash
  gcc sum1ton.c
  ./a.out
  ```


  
</details>
<details> 
 <summary>
 Task 5 - design of model 
  </summary>
  Biomedical Monitoring System

This project demonstrates a simple biomedical monitoring system using a VSDSquadron Mini development board, an NTC thermistor, and a MAX30102 pulse oximeter and heart rate sensor.

Features:

Temperature Monitoring: Measures and displays temperature using an NTC thermistor.
Heart Rate Monitoring: Measures and displays heart rate using the MAX30102 sensor.
Blood Oxygen Saturation (SpO2) Monitoring: Measures and displays SpO2 using the MAX30102 sensor.
Real-time Data Display: Displays real-time readings of temperature, heart rate, and SpO2 on an LCD or through serial communication.
Alarm Functionality: Optionally triggers an alarm (e.g., LED, buzzer) if readings fall outside of predefined thresholds.
Hardware:

VSDSquadron Mini development board
NTC Thermistor module
MAX30102 pulse oximeter and heart rate sensor
Breadboard (optional)
Jumper wires
Resistors
LED (optional)
Buzzer (optional)
LCD or serial communication module (optional)
Software:

RISC-V GCC compiler
PlatformIO IDE (recommended)
Libraries:
VSDSquadron Mini peripheral libraries (GPIO, ADC, I2C)
MAX30102 library (e.g., Adafruit MAX30102 library)
Circuit Diagram:

[Include a schematic diagram of the circuit connections here]

Software Structure:

main.c: Main program file, handles initialization, data acquisition, processing, and display.
sensors.c/sensors.h: Functions for reading data from the NTC Thermistor and MAX30102.
display.c/display.h: Functions for displaying data on the LCD or through serial communication.
alarm.c/alarm.h: (Optional) Functions for triggering alarms.

</details
