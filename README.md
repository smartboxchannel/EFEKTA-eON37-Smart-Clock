# EFEKTA eON37 Smart Clock Zigbee

My new zigbee project. Wireless Smart Clock with temperature, humidity and light sensors and of course with electronic ink display 3.7 inches. Automatic time and date setting via Zigbee network. Low power consumption, compact size, enclosure with magnets. The device use HTU21D T&H sensor, MAX44009 Light sensor, chip CC2530, battery 2хАА. Support in Zigbee2MQTT, not sure about ZHA yet.

### It is forbidden to manufacture devices for commercial sale, only for personal use.

### You can buy a ready-made device by writing to the mail hello@efektalab.com

### Delivery is carried out worldwide.

## You can make your own pcb here - https://www.pcbway.com/setinvite.aspx?inviteid=550959


#### Video: https://youtu.be/5huTVfVpZgs

#### zigbee2mqtt.io/supported-devices: https://www.zigbee2mqtt.io/supported-devices/#s=efekta

#### Telegram DiyDev - https://t.me/diy_devices

More info at http://efektalab.com/eON37SmartClock




## V1_R1

![EFEKTA eON37 Smart Clock Zigbee](https://github.com/smartboxchannel/EFEKTA-eON37-Smart-Clock/blob/main/IMAGES/000.png) 


![Indoor climate sensor EFEKTA eON213 Zigbee](https://github.com/smartboxchannel/EFEKTA_eON213z/blob/main/IMAGES/EFEKTA_eON213z.jpg) 


### How to flash the device

1. Download the Smart RF Flash Programmer V1 https://www.ti.com/tool/FLASH-PROGRAMMER

2. Open the application select the HEX firmware file

3. Connect the device with wires to CCDebugger, first erase the chip, then flash it.

---

### How to install IAR

https://github.com/ZigDevWiki/zigdevwiki.github.io/blob/main/docs/Begin/IAR_install.md

https://github.com/sigma7i/zigbee-wiki/wiki/zigbee-firmware-install (RU)

---

### How to join:
#### If device in FN(factory new) state:
##### one way
1. Open z2m, make sure that joining is prohibited
2. Insert the battery into the device
3. Click on the icon in z2m - allow joining (you have 180 seconds to add the device)
4. Go to the LOGS tab
5. Press the reset button on the device (the join procedure will begin, еhe device starts flashing the LED repeatedly)
6. Wait, in case of successfull join, device will flash led 5 times, if join failed, device will flash led 2 times

##### another way
1. Open z2m, make sure that joining is prohibited
2. Insert the battery into the device
3. Click on the icon in z2m - allow joining (you have 180 seconds to add the device)
4. Go to the LOGS tab
5. Press and hold button (1) for 2-3 seconds, until device start flashing the LED repeatedly
6. Wait, in case of successfull join, device will flash led 5 times, if join failed, device will flash led 2 times


#### If device in a network:
##### one way 
1. Hold button (1) for 10 seconds, this will reset device to FN(factory new) status 
2. Click on the icon in z2m - allow joining (you have 180 seconds to add the device)
3. Go to the LOGS tab
5. Press and hold button (1) for 2-3 seconds, until device start flashing the LED repeatedly
6. Wait, in case of successfull join, device will flash led 5 times, if join failed, device will flash led 2 times

##### another way
1.Find the device in the list of z2m devices and delete it by applying force remove
2. Click on the icon in z2m - allow joining (you have 180 seconds to add the device)
3. Go to the LOGS tab
4. Press the reset button on the device (the join procedure will begin, еhe device starts flashing the LED repeatedly)
5. Wait, in case of successfull join, device will flash led 5 times, if join failed, device will flash led 2 times

![Efekta THP_LR \ THP](https://github.com/smartboxchannel/EFEKTA_eON213z/blob/main/IMAGES/003.jpg) 

### Troubleshooting

If a device does not connect to your coordinator, please try the following:

1. Power off all routers in your network.
2. Move the device near to your coordinator (about 1 meter).
or if you cannot disable routers (for example, internal switches), you may try the following:
2.1. Disconnect an external antenna from your coordinator.
2.2. Move a device to your coordinator closely (1-3 centimeters).
3. Power on, power on the device.
4. Restart your coordinator (for example, restart Zigbee2MQTT if you use it).

If the device has not fully passed the join

1. If the device is visible in the list of z2m devices, remove it by applying force remove
2. Restart your coordinator (for example, restart Zigbee2MQTT if you use it).
3. Click on the icon in z2m - allow joining (you have 180 seconds to add the device)
4. Go to the LOGS tab
5. Press and hold button (1) for 2-3 seconds, until device start flashing the LED repeatedly
6. Wait, in case of successfull join, device will flash led 5 times, if join failed, device will flash led 2 times



### Other checks

Please, ensure the following:

1. Your power source is OK (a battery has more than 3V). You can temporarily use an external power source for testings (for example, from a debugger).
2. The RF part of your E18 board works. You can upload another firmware to it and try to pair it with your coordinator. Or you may use another coordinator and build a separate Zigbee network for testing.
3. Your coordinator has free slots for direct connections.
4. You permit joining on your coordinator.
5. Your device did not join to other opened Zigbee network. When you press and hold the button, it should flash every 3-4 seconds. It means that the device in the joining state.


## Components (BOM):

comming soon
