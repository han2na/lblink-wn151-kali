Driver LBlink WN151 Kali
- sudo apt-get update
- sudo apt-get upgrade
- reboot
- sudo apt-get install build-essential git dkms linux-headers-$(uname -r)
- git clone https://github.com/han2na/lblink-wn151-kali.git
- sudo dkms add ./rtl8188fu
- sudo dkms build rtl8188fu/1.0 
- sudo dkms install rtl8188fu/1.0
- sudo cp ./rtl8188fu/firmware/rtl8188fufw.bin /lib/firmware/rtlwifi/ 
