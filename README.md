## 🌿 Smart Plant Watering System using ESP32 & Blynk

This project is a smart plant watering system using ESP32 and the Blynk IoT platform. It monitors soil moisture and controls a water pump either automatically or manually, depending on the plant type selected by the user.

### 📦 Features

* Monitors soil moisture in real-time using an analog sensor.
* Controls a water pump automatically based on moisture level or manually via the Blynk app.
* Allows selection from 5 common plants: Aloe Vera, Mint, Spider Plant, Tulsi, and Money Plant.
* Adjusts moisture threshold based on selected plant type.
* Sends custom fertilizer and care tips for the selected plant.
* Displays real-time soil moisture health messages on the Blynk app.
* Updates data every 10 seconds.

### 📱 Blynk App Widget Mapping

* V1: Button to manually turn the pump ON or OFF.
* V2: Dropdown menu to select plant type (index 0 to 4).
* V3: Label to show soil moisture status (e.g., dry or healthy).
* V4: Label to show plant-specific fertilizer tips.

### 🛠️ Hardware Required

* ESP32 development board
* Soil moisture sensor (analog)
* 1-channel relay module
* Small water pump (5V or 12V based on setup)
* External power supply for pump (battery or adapter)
* Jumper wires for connections

### 🔌 Pin Assignments

* Moisture sensor connected to GPIO 33
* Relay (for pump control) connected to GPIO 4

### ⚙️ Software Requirements

* Arduino IDE with ESP32 board support installed
* Blynk library installed (`BlynkSimpleEsp32.h`)
* WiFi connection and Blynk credentials (template ID, auth token, etc.)

### 🔧 Setup Steps

1. Replace placeholders in the code with your actual WiFi SSID, password, and Blynk credentials.
2. Upload the code to your ESP32 using Arduino IDE.
3. Set up the Blynk app with the appropriate widgets on virtual pins V1 to V4.
4. Power up the hardware and open the Blynk app to start monitoring and controlling.

### 🔒 Safety Tips

* Use an external power source for the pump to avoid overloading the ESP32.
* Ensure the relay module is rated for your pump's voltage and current.

