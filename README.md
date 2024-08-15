<div align="center">

# Wake on Lan ESP32 Telegram Bot 👾

_Embedded telegram bot for ESP32 boards to send a WOL packet on a local network._  



</div>

## 📄 Description
This is the setup process for the **M5Atom** ESP32 board. A telegram bot is hosted on the board and listens for user commands, when the `/wol` command is received a Wake-on-Lan packet is broadcasted on the local network in order to turn on targeted device.

🪙 The board can stay running for about **1$** in electricity per year, the power consumption is less than half a watt. (Mileage may vary depending on ESP32 board used)

## ⚙️ Installation

- Install the following libraries from the Library Manager of the Arduino IDE:
  - [M5Atom](https://www.arduino.cc/reference/en/libraries/m5atom/): needed for the M5Atom board, if using a different board please download corresponding libraries.
  - [WakeOnLan](https://www.arduino.cc/reference/en/libraries/wakeonlan/): for sending magic packet
  - [UniversalTelegramBot](https://www.arduino.cc/reference/en/libraries/universaltelegrambot/): for using the Telegram API
- Create a new Telegram bot and configure your `BOT_TOKEN` and `ALLOWED_ID`  
  _You can use [@Botfather](https://t.me/botfather) to create a new bot and [@userinfobot](https://t.me/userinfobot) to get your ID_
- Fill your _WiFi configuration_ and the _MAC address_ of the PC you want to power on
- Compile and flash

## 🔎 Usage

- Use `/start` to get a list of the available commands
- Use the `/wol` command or press the physical button to turn on your PC
- Use the `/ping` command to check if the bot is online

