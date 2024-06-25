# ESP32 Tilt Sensor Project

### Project Overview
The ESP32 Tilt Sensor project demonstrates how to interface a tilt sensor with an ESP32 microcontroller to detect changes in orientation or tilt. This project is useful in applications where detecting movement or changes in position is critical, such as in security systems, robotics, or game controllers.

### Components Needed
- **ESP32 Microcontroller**: Used to read the tilt sensor input.
- **Tilt Sensor**: A simple switch that changes state when tilted.
- **Jumper Wires**: Connect the tilt sensor to the ESP32.
- **Breadboard**: Optional, for organizing circuit connections if needed.

### Circuit Setup
1. **Connecting the Tilt Sensor to ESP32:**
   - **Tilt Sensor Pin**: Connect one side of the tilt sensor to a GPIO pin on the ESP32 (e.g., GPIO 5).
   - **Power and Ground**: Connect the other side of the tilt sensor to GND. Use the internal pull-up resistor of the ESP32 to pull the pin high.

### Instructions
1. **Setup:**
   - Initialize Serial communication using `Serial.begin(9600)` for debugging purposes.
   - Set the tilt sensor pin as an input with an internal pull-up resistor using `pinMode(tiltSensorPin, INPUT_PULLUP)`.

2. **Operation:**
   - **Reading Tilt State:**
     - Use `digitalRead(tiltSensorPin)` to read the state of the tilt sensor.
     - Print the tilt state to the Serial Monitor.
   - **Detecting Tilt:**
     - Print "Tilt detected!" if the tilt sensor state is LOW (indicating it is tilted).
     - Print "No tilt detected." if the tilt sensor state is HIGH (indicating it is not tilted).

3. **Output:**
   - Continuously display the tilt state.
   - Indicate tilt detection based on the sensor reading.

4. **Considerations:**
   - **Debouncing:** Implement software debouncing if the sensor produces erratic readings.
   - **Mounting:** Ensure the tilt sensor is securely mounted to detect orientation changes accurately.
   - **Environment:** Test the sensor in the intended environment to ensure reliable operation.

### Applications
- **Security Systems:** Detect unauthorized movement or tampering.
- **Robotics:** Monitor the orientation of robotic components.
- **Game Controllers:** Create tilt-sensitive inputs for interactive gaming experiences.

### Useful Links
🌐 [ProjectsLearner - ESP32 Tilt Sensor](https://projectslearner.com/learn/esp32-tilt-sensor)  
📧 [Email](mailto:projectslearner@gmail.com)  
📸 [Instagram](https://www.instagram.com/projectslearner/)  
📘 [Facebook](https://www.facebook.com/projectslearner)  
▶️ [YouTube](https://www.youtube.com/@ProjectsLearner)  
📘 [LinkedIn](https://www.linkedin.com/in/projectslearner)

Created with ❤️ by ProjectsLearner
