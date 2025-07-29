# 🔐 Smart Safety Box with Arduino UNO and Fingerprint Security

## 📌 Overview
Smart safety box project using Arduino UNO with fingerprint security system and additional security features.

## 🛠️ Hardware Components
- Arduino UNO
- R307 Fingerprint Sensor
- Solenoid Door Lock
- DFPlayer Mini
- KY-012 Active Buzzer 5V
- Push Button
- Speaker
- LEDs (Green and Red)
- 16x2 LCD Display
- Relay Module
- SW420 Vibration Sensor

## 🔌 Wiring Configuration

### Fingerprint Module
```
🔴 Red Wire    -> 5V
⚫ Black Wire  -> GND
💛 Yellow Wire -> D2 (TX)
💚 Green Wire  -> D3 (RX)
```

### LCD I2C
```
🟧 Orange Wire -> VCC 5V
🟫 Brown Wire  -> GND
💛 Yellow Wire -> A4 (SDA)
⚪ White Wire  -> A5 (SCL)
```

### DF3Player
```
🔴 Red Wire   -> 5V
⚫ Black Wire -> GND
🔵 Blue Wire  -> D11 (RX)
🟣 Purple Wire-> D10 (TX)
```

## ⚙️ How It Works

1. 🔋 Power Supply
   - System is powered by battery

2. 👆 Fingerprint Authentication
   - Detects and verifies fingerprint patterns for access

3. 🔊 Audio Feedback
   - DFPlayer handles MP3 playback through speaker
   - Provides voice feedback for different actions

4. ✅ Successful Authentication
   - Green LED turns on
   - "Door Unlocked" voice prompt
   - LCD displays "Door Unlocked"
   - Solenoid lock opens

5. ❌ Failed Authentication
   - Red LED turns on
   - "Wrong Fingerprint" voice prompt
   - LCD displays "Wrong Fingerprint"
   - Door remains locked

6. 🚨 Security Features
   - SW420 vibration sensor detects tampering
   - Triggers buzzer alarm for several seconds
   - Activates security protocol

7. 🔒 Manual Lock
   - Push button to manually lock the door
   - System resets to secure state

## 🔧 Additional Features
- LCD status display
- Dual LED indicators
- Serial monitoring
- Anti-tampering detection
- Audio feedback system

## ⚠️ Security Measures
- Fingerprint verification
- Vibration detection
- Alarm system
- Manual override option

---
💡 **Note:** Make sure to properly configure the fingerprint sensor and add authorized fingerprints before deployment.