# TCarTrackerSim

This project is a haxx code, shared to let others easily write their own tracker based on it.

It uses LILYGO TTGO T-SIM7000G for the GPS + 4G for positioning and communication. If it is in wifi range, use it instead.
For the Wifi it uses the SWifi lib. Most of the time it is in deep sleep, waiting for an interrupt to wake it. The interrupt comes from the ADXL345 module when the car is moved.
Also wakes up multiple times a day, and sends its battery info.

The tracker sends the data to Traccar

## These are fully functional, but mostly for demonstration. I use it as a smart car alarm system, but the code is not pretty. It's separated into multiple files, to prevent using a single big unreadable file.

Libraries needed:
- ADXL345: https://github.com/adafruit/Adafruit_ADXL345
- SWifi: https://github.com/htotoo/SWifi
- TinyGSM
- Adafruit_SSD1306
- ArduinoHttpClient
