-----------------------------------------------------------------------------
Version: 20191124
-----------------------------------------------------------------------------
+Implement hardware led control support
*Captive portal now open WiFi settings
*Disable reboot comfir for AP mode
*Fix color_temp state for generic lamp/light controllers
*Implement color state for generic RGB lamp/controllers
*Add position state for Xiaomi curtains
*Fix Danalock setup
*Optimize MQTT subscriptions
+Support for Ksentry Zigbee OnOff Controller (KS-SM001)
+Support for Xiaomi Aqara B1 curtain motor (ZNCLDJ12LM)
+Support for Xiaomi Mi power plug ZigBee EU (ZNCZ04LM)
+Support for DIY DIYRuZ relay switch power meter (DYRuZ_rspm)
-----------------------------------------------------------------------------
Version: 20191117
-----------------------------------------------------------------------------
+Implement log caching (thx dmitriy_sannikov)
+Implement Zigbee channel setting
+Add pull up support for mode button
+Model name trimming for incorrect models (thx Devoff)
*Fix battery percentage calculation for DIYRuZ devices
+Support for Xiaomi Aqara double key wired wall switch without neutral wire (QBKG03LM)
-----------------------------------------------------------------------------
Version: 20191115
-----------------------------------------------------------------------------
*Fix stack overflow on parsing Xiaomi ZCL struct
*Fix device list packet (thx dmitriy_sannikov)
*Fix click state for devices (thx dmitriy_sannikov)
*Remove password for AP mode
+Add hardware button mode (press 2sec for enable/disable joining)
+Add hardware led (red - flashing on packet receive, green - display joining status)
+Add hardware configuration Web page
+Basic support Green Power devices
+Support for Philips Hue Tap
+Support for LifeControl Temperature, Humidity, eCO2, VOC sensor (MCLH-08) (thx lapatoc)
-----------------------------------------------------------------------------
Version: 20191107
-----------------------------------------------------------------------------
+Processing SimpleBind conditions (>, <, =, !, >=, <=, !=, <>)
*Fix TOGGLE state command for Xiaomi devices
+Support for Trust Smart tunable LED bulb (ZLED-TUNE9)
-----------------------------------------------------------------------------
Version: 20191101
-----------------------------------------------------------------------------
+Basic devices configuring feature
+Implemented SimpleBind feature - simple rules for internal binding
+Support for Itead Sonoff Zigbee DIY Smart Switch (BASICZBR3)
-----------------------------------------------------------------------------
Version: 20191031
-----------------------------------------------------------------------------
*Fix ZCL FrameType decoding
*Fix TI cc2538 init procedure
*Disable energy saving
+Support for Konke Motion Sensor (2AJZ4KPBS)
-----------------------------------------------------------------------------
Version: 20191024
-----------------------------------------------------------------------------
*Fix memory allocation (38KB RAM more free)
+Add name duplication check with group add
+Implement Captive Portal support
+Support for eWeLink Zigbee OnOff Controller (DZ4743-00B)
-----------------------------------------------------------------------------
Version: 20191022
-----------------------------------------------------------------------------
+Implemented device specific options, e.g. transition for brightness
+Setting device multi state via JSON
+Periodic report for Xiaomi MiJia temperature & humidity sensor (WSDCGQ01LM)
+Support for Xiaomi Aqara socket Zigbee (QBCZ11LM)
+Support for Danalock BT/ZB smartlock (V3-BTZB)
-----------------------------------------------------------------------------
Version: 20191021
-----------------------------------------------------------------------------
+Setting states via Web interface
+See more information about device in Web interface
+Show PowerSource & Battery level in Web interface
+Show routes in Web interface
+If the command sent successfully updates the LastSeen field
+permit_join state is now send on MQTT heartbeat
+permit_join state automatic disable via 255 seconds
-----------------------------------------------------------------------------
Version: 20191017
-----------------------------------------------------------------------------
+MQTT reset (zigbeeGW/bridge/config/reset)
+MQTT get device list (zigbeeGW/bridge/config/devices)
+MQTT & Web get device list (zigbeeGW/config/groups)
+MQTT & Web add group (zigbeeGW/config/add_group)
+MQTT & Web remove group (zigbeeGW/config/remove_group)
+Restore previous state/brightness on device announce
+Support for Sparx Single-channel relay switch (X2RM01)
+Support for Sparx Double-channel relay switch (X2RM02)
+Support for Sparx Triple-channel relay switch (X2RM03)
-----------------------------------------------------------------------------
Version: 20191016
-----------------------------------------------------------------------------
*Fix init zigbee network (thx Denis)
+Reset zigbee nvram & device config button in Web Interface
+Retain states option in MQTT settings
-----------------------------------------------------------------------------
Version: 20191015
-----------------------------------------------------------------------------
*Fix boot loop for clean zigbee module
*Fix crush on receive unsupported attribute
+Device annouce now published in MQTT
+When device leave from network they publish status in MQTT
+Experimental binding to gateway feature in Web Interface
+Support for Terncy Awareness switch (TERNCY-PP01)
-----------------------------------------------------------------------------
Version: 20191014
-----------------------------------------------------------------------------
*Reimplemented mechanism receiving messages from coordinator
*Redused count save devices actions
+Experimental feedback for Router devices
+Implement extended interview for devices
+Restart interview in Web interface
+Support for Trust RGB Tunable LED Bulb (ZLED-RGB9)
-----------------------------------------------------------------------------
Version: 20191010
-----------------------------------------------------------------------------
+Renaming devices in Web interface
+Removing devices in Web interface and MQTT
+Implement parsing ZCL_DATATYPE_STRUCT
*Fix TZ state for Xiaomi Aqara wireless relay controller (LLKZMK11LM)
+Support for Xiaomi MiJia Honeywell smoke detector (JTYJ-GD-01LM/BW)
+Support for Xiaomi MiJia gas leak detector (JTQJ-BF-01LM/BW)  
-----------------------------------------------------------------------------
Version: 20191005
-----------------------------------------------------------------------------
+Log console in Web interface
+Update firmware Over-The-Air in Web interface
+Support for Trust Smart Dimmable LED Bulb (ZLED-2709)
-----------------------------------------------------------------------------
Version: 20191002
-----------------------------------------------------------------------------
*Fixed redirect for reboot web page
*Disabling mDNS feature if domain is blank
+Support for Xiaomi Aqara wireless relay controller (LLKZMK11LM)
+Support for Xiaomi Aqara smart home cube (MFKZQ01LM)
+Support for IKEA TRADFRI motion sensor (E1525)
+Support for IKEA TRADFRI signal repeater (E1746)
+Support for IKEA TRADFRI LED bulb E26/E27 980 lumen, dimmable, white spectrum, opal white (LED1545G12)
-----------------------------------------------------------------------------
Version: 20190930
-----------------------------------------------------------------------------
+mDNS responder ( locate: http://zgwXXXX.local )
*Some fixes in Web interface
+Support for Xiaomi Aqara single key wired wall switch (QBKG11LM)
+Support for Xiaomi Aqara single key wired wall switch without neutral wire (QBKG04LM)
+Support for Xiaomi Aqara S2 Lock (ZNMS12LM)
+Support for Xiaomi Aqara S2 Lock Pro (ZNMS13LM)
+Support for Xiaomi Vima Smart Lock (A6121)
+Support for IKEA TRADFRI LED bulb E14/E26/E27 600 lumen, dimmable, color, opal white (LED1624G9)         
+Support for IKEA TRADFRI LED bulb E12/E14/E17 400 lumen, dimmable warm white, chandelier opal (LED1649C5)
-----------------------------------------------------------------------------
Version: 20190927
-----------------------------------------------------------------------------
+Saving devices on gateway reset
*Some fixes in Web interface
*Some fixes when starting coordinator
*Fix power & consumption value for Xiaomi plug (ZNCZ02LM)
*Fix battery voltage for Xiaomi devices - now in volts
+Support for DiY 4 Relays + 4 switches + 1 buzzer (DIYRuZ_R4_5)
+Support for DiY 20 button keypad (DIYRuZ_KEYPAD20)
+Support for DiY door/window open sensor (DIYRuZ_magnet)
+Support for Xiaomi Aqara wireless switch with gyroscope (WXKG12LM)
+Support for Xiaomi Aqara single key wireless wall switch (WXKG03LM)
-----------------------------------------------------------------------------
Version: 20190925
-----------------------------------------------------------------------------
*Disabled autostart joining on boot for more security
+Automatic restart gateway if zigbee module start failed
+Web interface for see zigbee devices list
+Web interface for see zigbee device states
+Web interface Start/Stop join button.
+Support for IKEA TRADFRI wireless dimmer (ICTC-G-1)
+Support for Xiaomi Aqara double key wired wall switch (QBKG12LM)
-----------------------------------------------------------------------------
Version: 20190923
-----------------------------------------------------------------------------
*Fix parsing ZCL commands from client clusters
*Fix Zigbee module reset indication
*Fix second ModelId for sensor WSDCGQ01LM
*Fix periodic pressure values from WSDCGQ11LM (thx Danikov Oleg)
+When new device is added to network it send event to MQTT and Log
+Renaming devices via MQTT
+Support for IKEA TRADFRI remote control (E1524)
-----------------------------------------------------------------------------
Version: 20190922
-----------------------------------------------------------------------------
*Fix MQTT reconnect
*Some fixes for web interface
*Fix negative temperature values for Xiaomi sensors (thx Danikov Oleg)
*Fix retrieve NTP time
+Support for Nue / 3A Smart light controller (LXZB-02A)
+Support for Xiaomi Aqara curtain motor (ZNCLDJ11LM)
+Support for IKEA TRADFRI bulb E27 W opal 1000lm (LED1623G12)
-----------------------------------------------------------------------------
