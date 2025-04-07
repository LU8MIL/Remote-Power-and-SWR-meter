📡 ESP32 RF Power & SWR Remote Meter
A remote RF power and SWR (ROE) monitoring system built using an ESP32 microcontroller. This project is ideal for amateur radio operators looking to monitor forward/reflected power and SWR in real time from a modern web interface.

🔧 Features
Measures forward and reflected power via analog inputs

Calculates Standing Wave Ratio (SWR) dynamically

Real-time web interface with AJAX updates (every 250ms)

Animated bar graphs for power visualization

Visual alert system: flashing red background when SWR > 3.0

ADC averaging for stable, noise-free readings

Fully self-hosted on the ESP32 — no external server needed

📶 Hardware Required
ESP32 development board

Directional coupler or RF sampling circuit

Voltage divider circuits for ADC protection

Pull-down resistors on analog inputs

WiFi access point or hotspot

🌐 How It Works
The ESP32 reads analog voltages from the directional coupler representing forward and reflected power. These readings are averaged, scaled, and converted into watts. The device calculates SWR and serves a responsive web interface showing real-time data.

When SWR exceeds 3.0, the page displays a red flashing alert warning the user of a potentially dangerous mismatch in the RF system.

📸 Web Interface Preview
(Add screenshot or gif here)

⚠️ Important Notes
Power range is scaled linearly: 0V = 0W, 3.3V = 100W

Adjust scaling if using amplifiers or external attenuation

Use proper RF shielding and filtering in your coupler design for best results

🧰 Future Ideas
MQTT integration

Logging to SD card or cloud

Email alerts for high SWR

Mobile UI improvements

📻 73 de LU8MIL 🇦🇷
If you like this project, feel free to fork it, improve it, and share it with the ham radio community!

