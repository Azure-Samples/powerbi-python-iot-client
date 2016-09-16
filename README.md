---
services: power-bi
platforms: raspberry-pi
author: sirui-sun
---

# Building a Real-time IoT Dashboard with Power BI: A Step-by-Step Tutorial
This sample code will read from a DHT22 sensor wired to a Raspberry Pi running Raspbian, and send data to a Power BI dashboard for display. Full walkthrough [here](https://powerbi.microsoft.com/blog/using-power-bi-real-time-dashboards-to-display-iot-sensor-data-a-step-by-step-tutorial).


## Running this sample locally on Raspbian 
### Clone the repository
```
git clone https://github.com/Azure-Samples/powerbi-python-iot-client
```

### Install dependencies
```
sudo apt-get install build-essential python-dev
git clone https://github.com/adafruit/Adafruit_Python_DHT.git && cd Adafruit_Python_DHT && sudo python setup.py install
```

### Update uploadDHT22Data.py with your REST API push URL
```
REST_API_URL = " *** Your Push API URL goes here *** "
```

### Run script
```
python uploadDHT22Data.py
```