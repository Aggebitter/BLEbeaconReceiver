# BLEbeaconReceiver
BLEBeaconReceiver

Just a quick "stolen" and modifyed snippet that I used to get presence detection on my mobile phone.
Baseded on:
https://github.com/pcbreflux/espressif/tree/master/esp32/arduino/sketchbook/ESP32_BLE_beaconscan

As BT, BLE and WiFi MAC-adresses nowdays är temporary and more and less random generated I needed a way to get the phones detected.
I've tryed diffrent BT,BLE and WiFi MAC scanners but why not turn it the other way? Create a BLE beacon at the Mobile phone side and
detect that Beacon. Now we got a presence detection! that I can control. 

As a beacon I use Beacon simulator avalible from Google Play by Vincent Hiribarren
https://play.google.com/store/apps/details?id=net.alea.beaconsimulator&hl=sv

In the file a lot of serial prints is commented out and I just use for the monent a Eddyston URL beacon
Did find out some buggs when I used it in altbeacon mode regarding the manufacturer ID as the 16 bit HEX is shown as 2 swapped 8 bit hex
(0xDEAD shows as 0xADDE) 

// Agge
