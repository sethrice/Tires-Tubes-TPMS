# Tires-Tubes-TPMS
This repo is built for knowledge sharing of how to build a Tire  Pressure Monitoring System (TPMS) for a fleet of E-Bikes.  

This project was created out of the need to track tire pressure on several types of e-bikes of various of specifications. Utilizing cheap sensors and open source software the desired outcome was acheived. This project has the following features:

 - Tracking of Tire Pressure and Tempature of several tires
 - A dashboard that presents the collected data in easy to understand low/nominal/high guages
 - Ability to set the low/nominal/high thresholds on a per tire basis
 - A historic graph of the collected data which could be helpful in finding slow leaks
 - A list of when the tire pressure data was last collected 

Utilizing a wireless digital sensor on each tire allows for the reading of the tire pressure without needing to physically interact with the tire. The data from the Tire Pressure Monitor Sensors (TPMS) are collected using a software defined radio (SDR) that is tuned to capturing 433mhz frequencies. The data collected from the SDR is sent to a database that is then later quriered to provide the visual dashboard. All of the software used in this project is open source and the only investment needed is the phsyical hardware and time. 

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
![Modify Guage Colors](https://cdn.juicedwheels.com/content/Modify%20Guage%20Colors.gif)

