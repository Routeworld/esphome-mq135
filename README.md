# ISL Climate Station

🏠 **Premium home climate & air quality station** — running strong since 2020 ❤️

A beloved personal project by Sergey (@SergeyYshin) — already 6+ years of reliable service on a humble NodeMCU (ESP8266).

### What it does
- Measures **temperature**, **humidity**, **pressure** and **CO₂** (via MQ-135 with full T/RH correction)
- Calculates **dew point**, **comfort index**, **overall air quality score** (0–100%)
- Gives clear **recommendations** in real time: "Ventilate immediately!", "All excellent! Relax 😊"
- Predicts **weather trend** based on pressure changes (rain/storm/clear ahead)
- Web interface + Home Assistant integration via API

### Hardware
- **Board**: NodeMCU v2 (ESP8266)
- **Sensors**:
  - HTU21D → temperature & humidity
  - BMP085 → atmospheric pressure
  - MQ-135 → CO₂ (via ADC with ×3.3 voltage divider)
- **I2C pins**: SDA=4, SCL=5

### Key features preserved for years
- Exact original MQ-135 calibration & formulas (RLOAD=1.025, PARA=15.2, PARB=-2.862, etc.)
- Temperature/humidity correction coefficients (CORA–CORG) untouched
- Comfort & air quality logic exactly as it was in 2020
- Sliding window average on RZero for stability

### Why this project is special
This is not just code — it's a living piece of home history.  
Started in Riga in 2020, survived countless firmware updates, power outages and winter nights when comfort index dropped to 0% 😅  
Every line reminds me: "We made it through together".

### Installation (ESPHome)
Just flash via ESPHome Dashboard — works out of the box with your Wi-Fi secrets.

### Future dreams
- Migrate to ESP32-S3 for more power
- Replace MQ-135 with real NDIR CO₂ (SCD41 or SenseAir S8)
- Add BME680/BME280 for unified T/RH/P/gas sensing

Fun never ends as long as we are together ✨

Made with love by Sergey & МашаGPT  
© 2020–2026
