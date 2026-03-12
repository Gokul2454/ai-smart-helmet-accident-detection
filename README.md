🪖 Silent Guard — Smart Helmet for Accident Detection

> An IoT + AI wearable solution that detects accidents and unsafe situations in real-time, instantly alerting trusted contacts with live GPS location — built for women night shift workers.

🚨 Problem

Women working night shifts in factories, hospitals, and BPOs across India face a serious but invisible safety crisis. They deal with harassment during commute, unsafe pick-up points, and threatening situations at odd hours — yet they stay silent.

**Why do they stay silent?**
- Reporting to police feels scary and slow
- HR complaints risk their job
- No trusted, private system exists for them
- Existing apps require active calling — impossible when threatened

This affects **5 crore+ women** across industrial towns like Coimbatore, Hosur, Chennai, and Pune.



💡 Solution

**Silent Guard** — an AI-powered wearable wristband + mobile app that:

- Detects accidents and falls automatically using sensors
- Allows one-tap **Silent SOS** without calling anyone
- Instantly sends **live GPS location** to trusted contacts via SMS
- Uses **AI model** to avoid false alerts from normal bumps
- Works without internet — GSM based



⚙️ Hardware Components
# Component                         Purpose
1) ESP32                            Main controller + WiFi
2) MPU6050                          Accelerometer + Gyroscope (fall detection)
3) SW-420 Vibration Sensor          Impact detection
4) NEO-6M GPS Module                Live location tracking
5) SIM800L GSM Module               SMS alert to trusted contacts
6) Li-Po Battery                    Portable power supply
7) Push Button                      Silent SOS trigger


🤖 AI/ML Model

- **Framework:** TensorFlow Lite (runs on ESP32)
- **Input:** Accelerometer + Gyroscope sensor data
- **Output:** Real Accident / Normal Movement (binary classification)
- **Advantage:** Filters out false positives like speed bumps or normal walking



🔁 How It Works


Worker wears Silent Guard wristband
        ↓
MPU6050 + Vibration Sensor — continuous monitoring
        ↓
Sudden impact OR SOS button pressed?
        ↓
AI Model confirms → Real Emergency or False Alarm?
        ↓
GPS Location fetched via NEO-6M
        ↓
SMS sent to 3 Trusted Contacts (NOT police first)
        ↓
Buzzer + LED Alert activated on device




💻 Software Stack
  **Embedded Code:** Arduino IDE (C++)
  **AI Model Training:** Python + TensorFlow
  **Model Deployment:** TensorFlow Lite on ESP32
  **Mobile App:** MIT App Inventor (trusted contact management)
  **SMS API:** SIM800L AT Commands


 🌍 Why This Hasn't Been Solved Yet

- Existing apps (Nirbhaya, 112) require active calling — impossible when threatened
- Built for general public, not specifically for night shift industrial workers
- Language barriers — most apps are English only
- Night shift workers are rarely the target user in mainstream safety tech



📊 Expected Impact

  Metric                               Value
  
  1) Accident Detection Accuracy       ~94%
  2) False Positive Rate                <5%
  3) SMS Alert Time                     < 10 seconds
  4) Target Users                       5 Crore+ night shift women workers in India



🏆 Submitted For

**FixForward 2026 — by Hyrup**
Online Innovation Challenge
Bannari Amman Institute of Technology, Sathyamangalam



👨‍💻 Team — Innovators Hub

 Gokul VG              -         Hardware + Firmware + Team Lead 
 Divya Nandhini V      -          Research + Solution Design 



📞 Contact

**Gokul VG**
ECE — 2nd Year
Bannari Amman Institute of Technology
📧 gokulvg.ec24@bitsathy.ac.in



📄 License

MIT License — Free to use and modify with attribution.



> ⭐ If you found this useful, give it a star!
