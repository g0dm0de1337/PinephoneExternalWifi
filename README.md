# PinephoneProExternalWifi
Pinephone Pro Work with "External WiFi Adapter" 

Tested monitor mode with: 
- > TP-Link Archer T2U [RTL8821AU] 
- > Alfa Network AWUS036NHA [Atheros]
- > TP-Link TW-WN722N (3.2EU version)

Thx to https://github.com/aircrack-ng/rtl8812au

Wifi card chipset support:
- > RTL8821AU RTL8812AU RTL8813AU
- > many Atheros (example AR9271)

That works with kali, nethunter PRO, Mobian, UbuntuTouch

+ sudo apt-get install build-essential linux-headers-$(uname -r) dkms unzip git
+ sudo apt-get install bc mokutil libelf-dev 
+ git clone -b v5.6.4.2 https://github.com/aircrack-ng/rtl8812au.git 
+ cd rtl8812* 
+ sudo apt-get install dkms 
+ sudo make dkms_install 
+ make && make install 
+ sudo apt-get install firmware-ath9k-htc 
+ sudo apt-get install firmware-atheros

# FINISH !!

put a network card in your Pinephone PRO via USB-C and have FUN
