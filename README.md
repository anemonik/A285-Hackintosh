<img src="screenshot.png" width="675" height="" >

# macOS Ventura 13.5 on Lenovo ThinkPad A285
Based on OC 0.9.4 Debug version.

<details>
💻 My configuration: <br>
| CPU       | AMD Ryzen 3 2300U 4-cores            |<br>
| GPU       | AMD Vega 6 512MB                     |<br>
| SSD       | Samsung 970 Evo Plus 500GB           |<br>
| Memory    | 8GB DDR4 2400Mhz                     |<br>
| Screen    | 12,5" 1920x1080 IPS                  |<br>
| WiFi & BT | MediaTek MT7921 (unsupported)        |<br><br>

BIOS Settings: <br>
| Fingerprint reader - OFF             |<br>
| CSM - OFF                            |<br>
| Secure Boot - OFF                    |<br>
| Wake on LAN - OFF                    |<br>
| Anti-Theft Current Setting- OFF      |<br>
| Intel VT-d - ON                      |<br>
| Intel Virtualization Technology - ON |<br>
| Excution Prevention - ON             |<br>
| Security Chip - OFF                  |<br>
</details>

To prepare OpenCore to install macOS you need to generate your own serial number, UUID and MLB for `MacBookPro16,3`. You can do that with a script called [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)

📝 Things to do: 
* Repair color banding
* Add fan control to YogaSMC
* Change OC Debug ver. to release
* Repair not working things (small chance for it currently)
* Add macOS Sonoma support (when it will came out from beta)


✅ Working:
* Graphic Acceleration 
* Keyboard (/w backlight)
* Audio (/w 3,5mm jack port)
* Display (there is a problem with color banding)
* USB ports
* Battery 
* Keyboard 
* Touchpad and Trackpoint
* HDMI port
* MicroSD slot

⚠️ Doesn't work:
* Wifi & BT (due to unsupported MediaTek card, but there are itlwm kexts already)
* Webcam (hanging up whole os when trying to open photo booth app)
* Microphone (detects internal one, but doesn't work)
* Sleeping
* WWAN