# Tires-Tubes-TPMS
This repo is built for knowledge sharing of how to build a Tire  Pressure Monitoring System (TPMS)

**Logical Diagram for this project:**
![Logical View](./Diagrams/TPMS_Architecture_Logical.svg)

**Physical Items needed for this project:**

 - TPMS Sensors: https://www.amazon.com/gp/product/B07Q2T649S/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1 

 - 433mhz Antenna: https://www.amazon.com/Electrodepot-Inches-Antenna-Magnetic-Connector/dp/B07NPX7W28/ 

 - RTL-SDR USB Radio: https://www.amazon.com/Electrodepot-Inches-Antenna-Magnetic-Connector/dp/B07NPX7W28/ 

 - Raspberry Pi 4: Amazon.com: https://www.amazon.com/Vilros-Raspberry-Fan-Cooled-Heavy-Duty-Aluminum/dp/B07XTRK8D4/ 

**Software Used for this project:**

 - Home Assistant (Operating System): https://www.home-assistant.io/

 - Mosquito Broker (MQTT):  https://github.com/home-assistant/addons/blob/master/mosquitto/DOCS.md

 - RTL_433 MQTT Auto Discovery (Entity Creation):https://github.com/bartrumb/rtl_433-hass-addons 

 - RTL_433 (Radio Controller): https://github.com/pbkhrv/rtl_433-hass-addons/tree/main/rtl_433

 - Nginx Proxy Manager (Encrypted Proxy): https://github.com/hassio-addons/addon-nginx-proxy-manager

 - Studio Code Server (Config file editor): https://github.com/hassio-addons/addon-vscode

 - MariaDB (Database): https://github.com/home-assistant/addons/tree/master/mariadb 


**Rename Entity:**
![Rename Entity](https://cdn.juicedwheels.com/content/Rename%20Entity.gif)


**Change Pressure Unit:**
![Change Pressure Unit](https://cdn.juicedwheels.com/content/Change%20Pressure%20Unit.gif)


**Add New Guagues:**
![New Guages](https://cdn.juicedwheels.com/content/Add%20new%20guages.gif)


**Modify Guage Colors**
![Modify Guage Colors](https://cdn.juicedwheels.com/content/Change%20Pressure%20Unit.gif)
https://cdn.juicedwheels.com/content/Modify%20Guage%20Colors.gif
