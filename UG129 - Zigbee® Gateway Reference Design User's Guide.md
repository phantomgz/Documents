**UG129: Zigbee® Gateway Reference Design User's Guide**

# 1. Introduciton
This section introduces RD=0001-0201: Zigbee Wi-Fi/Ethernet Gateway Reference Design and RD-0002-0201: Zigbee USB Virtual Gateway Reference Design.

The software is distributed as three software components:
* Z3Gateway Application
* NodeJS Server Application
* ReactJS Front=End Application

The Z3Gateway Application offers three transport options for inter-process and off-gateway communication:
* Telnet
* CoAP
* MQTT

The MQTT transport is used for inter-process communication with the NodeJS Server Application.

The software binaries are available using the Linux apt package manager, as described in section [2. Installation and Configuration for the Zigbee Wi-Fi/Ethernet Gateway (RD-0001-0201)]() and [3. Installation and Configuration for the Zigbee USB Virtual Gateway (RD-0002-0201)]().

The software source code for the Z3Gateway application is available as a host example application distributed with the EmberZNet PRO 6.2.0 Zigbee stack. For more information on how access the Zigbee stack please see <http://www.silabs.com/products/wireless/mesh-networking/Pages/getting-started-with-mighty-gecko-zigbee.aspx>. 

The software source code for the NodeJS Server Application and ReactJS Front-End Application is available on github at <https://github.com/SiliconLabs/gateway-management-ui> and is also installed on the target system at /opt/siliconlabs/zigbeegateway/gateway_management_ui.

The kits RD-0001-0201 and RD-0002-0201 are no longer available for purchase from Silicon Labs. Most users found it more convenient to acquire the Raspberry Pi hardware from third-party sources. Throughout this document the part numbers RD-0001-0201 and RD-0002-0201 are used to refer to the kit acquired previously from Silicon Labs or built with components from a third-party. 

The kits RD-0001-0201 and RD-0002-0201 shipped from Silicon Labs used a CEL USB dongle as the NCP. To improve ease-of-use, the CEL USB dongle is replaced with one of the three wireless starter kit mainboards available with the EFR32 Mighty Gecko Wireless SoC Starter Kit (SLWSTK6000B). Notes are made throughout this document to guide users wishing to continue using their CEL NCP USB dongle and EM35x-DEV end-devices. 

The WiFi / Ethernet Gateway runs on a Raspberry Pi 2 Model B or Raspberry Pi 3 Model B computer with Raspbian Linux and Zigbee NCP (network co-processor). A Silicon Labs EFR32 Mighty Gecko Wireless Starter Kit such as SLWSTK6000B is required as the NCP. The gateway includes a Wi-Fi soft access point and a web server that presents a user interface to a desktop or mobile web browser. The web browser can run on a device connected via Wi-Fi or wired local area network (LAN). A typical Zigbee system configuration with the Zigbee Wi-Fi/Ethernet Gateway is shown in the following figure.

