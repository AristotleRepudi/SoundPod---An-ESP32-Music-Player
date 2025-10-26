# SoundPod---An-ESP32-Music-Player
# 🚀 ESP32 Walkman – Because Normal MP3 Players Are Boring as Hell 🎧

This bad boy ain’t your regular MP3 player.
It’s an **ESP32-powered beast** that plays your tunes, charges like a champ, and flexes an OLED just to remind you you’re cooler than whoever’s still using an iPod Nano.

## 💀 The Brain
**ESP32-WROOM-32** — the overqualified little monster running this show.
- Wi-Fi + Bluetooth built in.
- Dual cores because one core’s for peasants.
- Handles audio, UI, and all your questionable firmware experiments.

## ⚡ Power Section
**AMS1117-3.3V LDO** – Converts battery juice into 3.3V ESP food.
**MCP73831 Li-ion Charger** – Handles charging so your Li-Po doesn’t go kaboom.
**JST PH-2.0 connector** – Your battery’s plug of destiny.

> ⚠️ Pro tip: Don’t short this section unless you enjoy fireworks and regret.

## 🔊 Audio Hardware
**DFR0299 MP3 Player Module** – Reads MP3s from SD card and spits out actual music.
- Supports microSD like a boss.
- Simple serial control, even your dog can code it.
- Can drive a mini amp or headphones (depending on your life choices).

## 🧠 Display & Bling
**0.96” OLED (SSD1306, I²C)** – Because headless debugging sucks.
Shows track names, volume, battery, and your tears when the firmware crashes.

## 🔋 Power Flow TL;DR
[USB] → [MCP73831] → [LiPo Battery] → [AMS1117-3.3V] → [ESP32 + OLED + DFR0299]
Smooth. Efficient. Chef’s kiss. 👨‍🍳💋

## 🧩 Pinout Highlights
| Component | Pin | Function |
|------------|-----|----------|
| ESP32 | RX/TX | Talks dirty to the DFR0299 |
| ESP32 | SDA/SCL | Chats with OLED |
| MCP73831 | PROG | Sets charge current (don’t mess it up) |
| AMS1117 | OUT | Feeds 3.3V dreams to ESP32 |

## 🧰 Tools & Parts
- **KiCad** – for your PCB wizardry
- **PlatformIO / Arduino IDE** – where code gets yeeted onto silicon
- **FreeCAD / Fusion 360** – for case modeling flex
- **Caffeine & sanity** – optional but recommended

## 🧪 Testing Checklist
- ✅ No magic smoke?
- ✅ OLED lights up?
- ✅ Music plays?
- ✅ You dance like a nerd?
If yes → congrats, you made a portable dopamine dispenser.

## 🔥 Future Upgrades (aka dreams that’ll probably break something)
- Add Bluetooth audio (ESP32 go brrrr)
- Make it rechargeable via USB-C
- Add a rotary encoder for volume control
- RGB LEDs because obviously.

## 💾 Folder Vibes
ESP32_Walkman/
├── schematics/
│   ├── walkman_schematic.kicad_sch
├── pcb/
│   ├── walkman_board.kicad_pcb
├── firmware/
│   ├── main.cpp
├── assets/
│   ├── logo.png
└── README.md   ← you’re reading this masterpiece

## ⚙️ TL;DR Setup
1. Flash firmware → **ESP32**
2. Insert SD card → loaded with MP3s
3. Plug in headphones → cry tears of joy
4. Realize you made a freakin’ *smart Walkman* from scratch 🤘

## 💀 Credits
- You – the absolute mad lad who made this.
- Coffee – the real power supply.
- ESP32 – for handling all our bullshit.
"# SoundPod---An-ESP32-Music-Player" 
