# 🚗 Android Joystick Controller for ESP8266

## 🎮 Overview
This project provides an Android-based virtual joystick that communicates with an ESP8266 over Wi-Fi to control movement. The joystick sends directional commands to the ESP8266 based on user input.

## ✨ Features
- Smooth joystick movement 🕹️
- Supports both 4-direction and 8-direction control 🎯
- Adjustable sensitivity and transparency 🎛️
- Sends HTTP requests to ESP8266 for movement control 🌐

## 🛠️ How It Works
1. The joystick detects user input and calculates the direction and angle. 📏
2. Based on the input, the joystick sends an HTTP request to the ESP8266. 📡
3. The ESP8266 receives and processes movement commands (e.g., forward, backward, left, right). 🔄
4. The joystick updates dynamically based on user interactions. ⚡

## 🔗 Connection to ESP8266
Replace `http://192.168.4.1` with your ESP8266's IP address.

## 📜 Code Breakdown
### 🎨 UI Components
- Uses `ViewGroup` to handle joystick layout.
- Draws a joystick bitmap on the screen.
- Detects touch movements and updates the joystick position dynamically.

### 🚀 Movement Processing
- Determines the joystick's angle and distance.
- Converts input into directional movement.
- Sends HTTP requests to control ESP8266 movement:
  - `http://ESP-IP/forward` 🚗➡️
  - `http://ESP-IP/backward` 🚗⬅️
  - `http://ESP-IP/left` 🔄
  - `http://ESP-IP/right` 🔃
  - `http://ESP-IP/stop` 🛑

### ⚙️ Customization Options
- Adjust joystick size, transparency, and sensitivity.
- Modify the ESP8266 endpoints as needed.


## 🏗️ Installation
1. Clone this repository: 
   ```sh
   https://github.com/Samkelo908/maqueen_joystick.git
   ```
2. Open the project in Android Studio.
3. Modify `esp8266Ip` to match your device's IP.
4. Run the app on an Android device. 📱✅

## 🔥 Future Improvements
- Add Bluetooth support for offline mode. 🎧
- Implement vibration feedback for better user experience. 🎮
- Enhance UI design with animations. ✨

## 🤝 Contributions
Feel free to fork and contribute to this project! 🚀

## 📜 License
This project is open-source and available under the MIT License. 📄

Happy coding! 🚀🎮
