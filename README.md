# bitcoin-ticker
Simple bitcoin ticker for the Pimorono InkyPhat Red.

## Equipment
* Raspberry Pi Zero W v1.1
* Pimorono Inky pHAT Red (SSD1608)

## Setup
1. Install Raspbian Lite
2. Update and upgrade 
```Bash
sudo apt update && sudo apt upgrade -y
```
3. Install Inky pHAT 
```Bash
curl https://get.pimoroni.com/inky | bash
```
4. Install the font we're using
```Bash
pip install font-fredoka-one
```
5. Install Git
```Bash 
sudo apt install git
```
6. Clone this repo
```Bash
git clone https://github.com/Rubstubs/bitcoin-ticker.git
```
7. Open crontab
```Bash
crontab -e
```
Add this line:
```Bash
*/2 * * * * python3 /home/pi/bitcoin-ticker/bitcoin-ticker.py
```
Crontab will then run the script every second minute

[![thelooks.jpg](https://i.postimg.cc/MHdPKh8M/thelooks.jpg)](https://postimg.cc/8ffBZXcN)