🏠 TECHXCELERATE – Smart Home Automation using Arduino & IoT

This end-to-end smart home system leverages an Arduino-based setup and modern web technologies to monitor and control indoor environments—designed to be more affordable and user-friendly than traditional solutions.

🌡️ Core Functionality

Temperature & Humidity Monitoring via DHT11/DHT22 sensors.

Ambient Light Detection using LDR sensors.

Automated Appliance Control:

Triggers lights or fans using relay modules based on sensor readings.

Real-time Remote Access:

Connects to Wi‑Fi (ESP8266/NodeMCU)

Offers a web interface (built with HTML, JS, Node.js/Express) for users to monitor and operate devices.

⚙️ Architecture & Tech Stack

Hardware:

Arduino UNO or ESP8266‑based NodeMCU for sensing and control

DHT11/DHT22 & LDR sensors

Relay modules for switching AC appliances

Software:

Frontend: index.html, detail.html for dashboard and control

Backend: index.js server using Node.js/Express

MQTT protocol (with mosquitto.conf) for lightweight IoT messaging

Configurations stored in config/, modular controllers, routes, and services for scalability

📡 How It Works

Arduino/NodeMCU collects environment data, then publishes sensor data via MQTT.

Node.js server subscribes to MQTT topics, processes data, and relays commands.

Web dashboard displays live readings and allows users to manually toggle appliances.

Automation logic: e.g., if the room gets too warm → fan auto‑switches ON.

✅ Advantages & Improvements over Traditional Systems
Low-cost DIY components instead of expensive proprietary systems

Modular code architecture—easy to maintain and extend

Easy self-installation with public Wi‑Fi and web UIs—no professional setup required

🎯 Suggested Enhancements
Add push notifications or email alerts when thresholds are crossed.

Integrate data logging/charting using a database or IoT service.

Enhance security: JWT-based authentication and HTTPS on the dashboard.

Add voice control support via Alexa or Google Assistant.

Expand with additional sensors (e.g., gas, motion) or automate more devices.
