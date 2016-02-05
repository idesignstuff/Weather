# Weather

I'm a beginner, and this is where I'll be keeping my code as I figure out some things.

The plan:
-outdoor weather station consisting of
  -Gikfun Pro Mini A328 3v3 @ 8MHz
  -DIYmall BME280 I2C temp/humidity/pressure sensor
    -measure outdoor temp/hum/pressure
  -nRF24L01+ 2.4GHz network card w/PCB antenna
     -send/receive data
  
-indoor HVAC controller
  -Gikfun Pro Mini A328 3v3 @ 8MHz
  -DHT-11 oneWire temp/humidity sensor
    -monitor HVAC performance at return duct
  -nRF24L01+ 2.4GHz network card w/PCB antenna
     -send/receive data
  -Sainsmart 4 channel relay to interface with:
    -HVAC blower @24VAC
    -Heater switch @24VAC
    -A/C compressor switch @24VAC
    -Humidfier switch @24VAC
  -LED or LCD mode/health indicators
  -I2C 2004 LCD?
    -Display mode/setpoint/current state
    
-indoor weather station/ HVAC control module
  -Gikfun Pro Mini A328 3v3 @ 8MHz
  -DHT-11 oneWire temp/humidity sensor
    -monitor living space temp/hum
  -nRF24L01+ 2.4GHz network card w/PCB antenna
    -send/receive data
  -Sainsmart 2004 I2C LCD
    -Display outdoor Temp/Hum/Pressure/Heat index/Dewpoint/etc. (maybe trends to indicate weather changes)
    -Display HVAC setpoint
    -Display indoor temp/Hum
  -Encoder with pushbutton for user inputs
    -Send control inputs for setpoint/modes/power states
      -blower on/off/auto
      -Heat/Cool/Auto
      -set target temp, (maybe weighted for other sensors in other rooms?)
      -set target humidity(based on outside temp logic) Max 45% target, lower when outside is <20F
      
