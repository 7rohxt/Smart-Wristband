# Smart Wristband

## Key Features
- **Fall Detection**: Using an accelerometer and gyroscope (MPU6050) to detect falls.
- **Heart Rate Monitoring**: Tracks heart rate for basic health monitoring.
- **Emergency SOS Button**: Alerts caregivers or family members in case of an emergency.
- **Long Battery Life**: Ensures reduced charging frequency for ease of use.

## Hardware Requirements
### Microcontroller Options (Any 1):
- **ESP32**: Affordable and equipped with built-in Wi-Fi and Bluetooth for easy connectivity.
- **STM32**: Low-cost and energy-efficient, suitable for long battery life.
- **Arduino Nano**: Very affordable but limited in features.

### Sensors:
- **Accelerometer/Gyroscope**: MPU6050 (used for fall detection and step counting).
- **Heart Rate Sensor**: MAX (for heart rate and SpO2 monitoring).
  
### Power:
- **Battery**: Li-Po battery with integrated charging circuit to provide long battery life.

## Methodology
1. **Software Development**: The system is built using bare-metal programming tailored for the selected microcontroller.
2. **Fall Detection Algorithm**: The fall detection model is trained using data and deployed on the microcontroller using **TensorFlow Lite** for real-time processing.
3. **Health Monitoring Algorithms**: The heart rate and SpO2 levels are calculated using existing libraries tailored for the chosen sensors.
4. **Emergency SOS Button Integration**: The microcontroller is programmed to detect a button press and instantly trigger an alert to caregivers or family members.

## Future Enhancements
- **Step Counter**: Adds basic activity tracking using accelerometer data.
- **Simple Interface**: Large, easy-to-use buttons or a minimal display for user convenience.
- **Blood Sugar Monitoring**: Ability to monitor and track glucose levels for diabetic users.

