# GPS Tracker using ESP32

[![ESP32](https://img.shields.io/badge/Board-ESP32-blue?logo=espressif)](https://www.espressif.com/en/products/socs/esp32) 
[![Language](https://img.shields.io/badge/Language-Arduino%20C++-brightgreen?logo=arduino)](https://www.arduino.cc/reference/en/) 
[![Project](https://img.shields.io/badge/Project-CircuitDigest-orange)](https://circuitdigest.com)

---

## 📘 Tutorial Link  
👉 [GPS Tracker using ESP32](https://circuitdigest.com/microcontroller-projects/simple-gps-tracker-using-esp32-visualize-data-on-map)

## 📂 Project Type  
🔗 [ESP32 Project](https://circuitdigest.com/esp32-projects)

---

![GPS Tracker using ESP32](https://circuitdigest.com/sites/default/files/projectimage_mic/GPS-Tracker-using-ESP32-and-GeoLinker.png)

---

## 🚀 Features
- Real-time GPS tracking with ESP32 and Neo-6M GPS module  
- Cloud-based visualization using **GeoLinker API**  
- Offline data buffering when internet is unavailable  
- Automatic re-sync once connection is restored  
- Configurable update intervals for optimized performance  

---

## 🛠️ Hardware Requirements

| Component | Quantity |
|-----------|----------|
| [ESP32 Development Board](https://components101.com/microcontrollers/esp32-devkitc) | 1 |
| [Neo-6M GPS Module](https://components101.com/modules/neo-6mv2-gps-module) | 1 |
| LEDs | 2 |
| 1kΩ Resistors | 2 |
| Breadboard | 1 |
| Connecting Wires | As required |

---

## ⚙️ How It Works
1. The **Neo-6M GPS module** fetches latitude, longitude, and time data using NMEA protocol.  
2. The **ESP32** reads this data over UART (pins IO16/IO17).  
3. Data is transmitted to the **GeoLinker API** via Wi-Fi.  
4. If Wi-Fi is unavailable, the ESP32 **stores data locally** until connectivity is restored.  
5. Once reconnected, buffered data is synced to the cloud along with real-time updates.  
6. The location is plotted on the **GeoLinker map interface** for route tracking.  

---

## 🔌 Circuit Connection  

![Circuit Diagram](https://circuitdigest.com/sites/default/files/circuitdiagram_mic/GPS-Tracker-Circuit-Diagram-using-ESP32.png)

### Pin Mapping Table  

| ESP32 Pin | GPS Module Pin |
|-----------|----------------|
| 3.3V      | VCC            |
| GND       | GND            |
| IO16 (RX) | TX             |
| IO17 (TX) | RX             |

---

## 🧠 Troubleshooting  

| Issue | Possible Cause | Solution |
|-------|----------------|----------|
| No GPS Fix | Weak satellite signal | Move outdoors or use an active antenna |
| Wi-Fi not connecting | Wrong SSID/Password | Double-check credentials in code |
| Data not uploading | Invalid API key | Re-generate and update API key in code |
| Garbage output from GPS | Baud mismatch | Ensure GPS baud is set to **9600** |
| ESP32 resets | Power instability | Use stable 5V USB supply |

---

## 📱 Applications
- Vehicle tracking  
- Asset monitoring  
- Personal safety devices  
- Fleet management systems  
- Outdoor navigation experiments  

---

## 🔮 Future Enhancements
- Support for GSM/GPRS modules for remote areas  
- Integration with Google Maps for visualization  
- Data logging on SD card  
- Mobile app dashboard for live tracking  
- Multi-device fleet tracking support  

---

## 🧪 Technical Specifications

| Parameter | Value |
|-----------|-------|
| Microcontroller | ESP32 |
| GPS Module | Neo-6M |
| GPS Protocol | NMEA |
| GPS Baud Rate | 9600 |
| Connectivity | Wi-Fi (2.4 GHz) |
| Cloud API | GeoLinker (CircuitDigest Cloud) |
| Offline Buffer | Up to 20 records |
| Power Supply | 5V (USB) |

---

## 🔗 Links
- 📘 [GPS Tracker using ESP32](https://circuitdigest.com/microcontroller-projects/simple-gps-tracker-using-esp32-visualize-data-on-map)  
- 📂 [ESP32 Project Collection](https://circuitdigest.com/esp32-projects)  
- 📚 [ESP32 with NEO-6M GPS Module](https://circuitdigest.com/microcontroller-projects/interfacing-neo6m-gps-module-with-esp32)  
- 📖 [Arduino IDE](https://www.arduino.cc/en/software)  
- 📄 [ESP32 Datasheet](https://www.espressif.com/sites/default/files/documentation/esp32_datasheet_en.pdf)  
- 📄 [Neo-6M GPS Datasheet](https://www.u-blox.com/sites/default/files/products/documents/NEO-6_DataSheet_%28GPS.G6-HW-09005%29.pdf)  
- 💻 [GeoLinker GitHub Repository](https://github.com/Circuit-Digest/GeoLinker)  
- 💻 [Project GitHub Repository](https://github.com/Circuit-Digest/Simple-GPS-Tracker-using-ESP32---Visualize-Data-on-Map)  

---

## ⭐ Support
This project is published on **[CircuitDigest](https://circuitdigest.com)**.  
If you found it useful, please ⭐ star the repository and share it with others!

---

## 🔖 Keywords
`ESP32` `Neo-6M GPS` `GeoLinker API` `GPS Tracker` `IoT GPS` `ESP32 Project` `Arduino C++`
