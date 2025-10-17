# ⚡ MarketView Hardware

MarketView is a compact hardware module designed to display live market data — such as cryptocurrency or stock prices — directly on an OLED screen, powered by the ESP32-C3-WROOM-02.  
It’s built to be **portable, affordable, and educational**, giving users real-time updates in a minimal design that’s perfect for learning embedded systems, electronics, and PCB design.

---

## 🧠 Overview

- **Microcontroller:** ESP32-C3-WROOM-02-N4  
- **Display:** 0.96" OLED (I²C)  
- **Input:** 2 Push Buttons  
- **Indicators:** Power LED & Buzzer  
- **Power:** USB Type-C (5V) → 3.3V Regulated Output  
- **Board Type:** Custom PCB designed in EasyEDA  

The board connects to a host (or Wi-Fi) to fetch real-time crypto or stock data and display it instantly.  
MarketView merges software and hardware beautifully — offering insight into IoT data monitoring and PCB design.

---

## ⚙️ Hardware Details

| Component | Description | Reference |
|------------|--------------|------------|
| **U1** | ESP32-C3-WROOM-02-N4 | Main MCU |
| **U3** | 3.3V Voltage Regulator | Power Conversion |
| **U4** | USB Type-C Connector | Power Input |
| **U5, U6** | 5.1 kΩ Resistors | CC1/CC2 Pull-down |
| **R1** | 1 kΩ | Power LED |
| **D1** | LED (3mm) | Power Indicator |
| **BZ1** | Piezo Buzzer | Sound Alert |
| **S1, S2** | Push Buttons | Mode Control |
| **OLED1** | 0.96" I²C OLED Display | Market Display |

---

## ⚡ Power Section

- **VBUS (5V)** → Regulator **Input**  
- **Regulator GND** → Common Ground  
- **Regulator Output (3.3V)** → ESP32 3.3V Pin  
- **CC1 and CC2** → Each connected through **5.1 kΩ** resistor → GND  
- **USB GND** → Common Ground  
- **Optional:** Add 100 µF capacitor (input) and 10 µF capacitor (output) for stability.  

---

## 🧩 Required Files

For EasyEDA version:

- `BOM.csv`
- `Gerber.zip`
- `Schematic.json`
- `PCB.json`
- `Assembly.csv`
- `Schematic.pdf`

Additionally:
- `ReadMe.md` (this file)
- Renders or Screenshots of your board design
- Optional `.step` or `.stl` 3D model

---


## 💡 Future Plans

- Add a Li-ion battery with charging IC (TP4056).  
- Implement data fetching via Wi-Fi to display live market prices.  
- Integrate sound notifications for major market changes.

---

## 🧾 License

This project is open source under the **MIT License**.  
Feel free to modify, remix, and improve upon it.

---


**📦 Built by Joel (2025)**  
