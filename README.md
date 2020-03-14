
# Installation
## Adding Mi Box S to Home Assistant:
#### 1)  Enabled USB Debugging on Android TV/Mi Box S
      - Settings, Debugging Options, Enable USB Debugging. 

#### 2) Enable Wireless ADB Debugging 
    • Plug a USB A to USB A into your computer. 
    • Run 'adb devices' to ensure it's connected
    • Run 'adb tcpip 5555' (any port number not in use)
    • Run 'adb connect [ip]:5555'

#### 3) Add the following commands to your home assistant configuration.yaml. 

#### Home assistant Configuration
    # IoT Devices
    media_player:
      - platform: androidtv
        name: MiBox 4S
        host: 192.168.0.111
More options can be found [here](https://www.home-assistant.io/integrations/androidtv/).        
        
