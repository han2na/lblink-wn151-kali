Driver LBlink WN151 Kali
- sudo apt-get update
- sudo apt-get upgrade
- reboot
- sudo apt-get install build-essential git dkms linux-headers-$(uname -r)
- git clone https://github.com/han2na/lblink-wn151-kali.git
- sudo dkms add ./lblink-wn151-kali
- sudo dkms build rtl8188fu/1.0 
- sudo dkms install rtl8188fu/1.0
- sudo cp ./lblink-wn151-kali/firmware/rtl8188fufw.bin /lib/firmware/rtlwifi/ 
