# Weather

I'm a beginner, and this is where I'll be keeping my code as I figure out some things.

The plan:<br>
-outdoor weather station consisting of<br>
  -Gikfun Pro Mini A328 3v3 @ 8MHz<br>
  -DIYmall BME280 I2C temp/humidity/pressure sensor<br>
    -measure outdoor temp/hum/pressure<br>
  -nRF24L01+ 2.4GHz network card w/PCB antenna<br>
     -send/receive data<br>
  
-indoor HVAC controller<br>
  -Gikfun Pro Mini A328 3v3 @ 8MHz<br>
  -DHT-11 oneWire temp/humidity sensor<br>
    -monitor HVAC performance at return duct<br>
  -nRF24L01+ 2.4GHz network card w/PCB antenna<br>
     -send/receive data<br>
  -Sainsmart 4 channel relay to interface with:<br>
    -HVAC blower @24VAC<br>
    -Heater switch @24VAC<br>
    -A/C compressor switch @24VAC<br>
    -Humidfier switch @24VAC<br>
  -LED or LCD mode/health indicators<br>
  -I2C 2004 LCD?<br>
    -Display mode/setpoint/current state<br>
    
-indoor weather station/ HVAC control module<br>
  -Gikfun Pro Mini A328 3v3 @ 8MHz<br>
  -DHT-11 oneWire temp/humidity sensor<br>
    -monitor living space temp/hum<br>
  -nRF24L01+ 2.4GHz network card w/PCB antenna<br>
    -send/receive data<br>
  -Sainsmart 2004 I2C LCD<br>
    -Display outdoor Temp/Hum/Pressure/Heat index/Dewpoint/etc. (maybe trends to indicate weather changes)<br>
    -Display HVAC setpoint<br>
    -Display indoor temp/Hum<br>
  -Encoder with pushbutton for user inputs<br>
    -Send control inputs for setpoint/modes/power states<br>
      -blower on/off/auto<br>
      -Heat/Cool/Auto<br>
      -set target temp, (maybe weighted for other sensors in other rooms?)<br>
      -set target humidity(based on outside temp logic) Max 45% target, lower when outside is <20F<br>
      
