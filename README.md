### Description
# ESB 32 USB-C Development Board

The **ESB 32** is a custom-designed ESP32 development board created using **Altium Designer**, featuring a **USB Type-C** interface for reliable power delivery and programming. This board is tailored for IoT prototyping, embedded systems development, and educational use in microcontroller-based applications.


## Developer Information

- **Name:** Abdul Rahman  
- **Roll Number:** BSEE21080  
- **Department:** Electrical Engineering  
- **Institution:** Information Technology University (ITU), Lahore  
- **Course:** Bachelor of Science in Electrical Engineering  
- **Project Year:** 2025  


##  Project Objectives

- Design and fabricate a compact ESP32-based development board
- Integrate USB Type-C for modern power/data connection
- Ensure breadboard compatibility for ease of prototyping
- Provide all essential features for firmware development and debugging
- Apply PCB design knowledge using **Altium Designer**


## Technical Specifications

1 **Microcontroller:** ESP32-WROOM-32 (Dual-core Xtensa 240MHz, Wi-Fi, Bluetooth)
2 **Power Interface:** USB Type-C (5V input)
3 **Voltage Regulation:** AMS1117-3.3 (or compatible)
4 **Programming Interface:** USB to UART bridge ( CP2102 / CH340)
-5 **Onboard Components:**
  - Reset and Boot buttons
  - Power LED
  - Optional user LED (GPIO-connected)
6 **I/O Access:** Multiple GPIOs exposed via headers
7 **PCB Size:** [Specify dimensions if known]

## Tools & Environment

- **PCB Design Tool:** Altium Designer
- **Firmware Development:** Arduino IDE, PlatformIO, or ESP-IDF
- **Simulation/Test:** Multimeter, Oscilloscope, Serial Monitor

## Getting Started
### Requirements

- USB Type-C cable
- ESP32 board definitions (via Arduino Boards Manager)
- Required USB-to-Serial drivers ( CH340 / CP2102)

### Setup Instructions

1. Connect ESB 32 to your PC via USB-C.
2. Install required USB drivers.
3. Open Arduino IDE and install ESP32 board support from the Boards Manager.
4. Go to `Tools > Board > ESP32 Dev Module`.
5. Select the correct COM port.
6. Upload your sketch!

###  Example Code: Blink LED

```cpp
void setup() {
  pinMode(2, OUTPUT);  // GPIO 2 used in it
}

void loop() {
  digitalWrite(2, HIGH);
  delay(1000);
  digitalWrite(2, LOW);
  delay(1000);
}
