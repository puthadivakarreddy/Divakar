# ESP32 Bluetooth OLED Display and RGB LED Control

This project uses an **ESP32** microcontroller to:

- Receive Bluetooth messages from a mobile device or PC.
- Convert normal English to a fun **Old English style** on an OLED screen.
- Control an **RGB LED** using Bluetooth commands.

## 📦 Features

- ✅ Bluetooth Serial Communication using `BluetoothSerial.h`
- ✅ Display messages on a 128x64 I2C **OLED screen** using the `Adafruit_SSD1306` and `Adafruit_GFX` libraries
- ✅ Simple Old English translator for fun message display
- ✅ RGB LED color control via formatted commands

---

## 🔧 Hardware Requirements

- ESP32 Dev Board
- 128x64 OLED display (I2C)
- Common Cathode RGB LED
- Resistors for LED (e.g., 220Ω)
- Breadboard and jumper wires

### 🖼️ OLED I2C Connection

| OLED Pin | ESP32 Pin |
|----------|-----------|
| VCC      | 3.3V      |
| GND      | GND       |
| SDA      | GPIO 21   |
| SCL      | GPIO 22   |

### 🔌 RGB LED Pin Configuration

- **Red**   → GPIO 16  
- **Green** → GPIO 17  
- **Blue**  → GPIO 18

---

## 📲 Bluetooth Commands

### RGB Control
Send commands via Bluetooth in the format:
