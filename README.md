# ⚔️ APP-KILLER — Termux Shizuku Background App Terminator ⚡

**Boldly eliminate background apps with the power of Shizuku!**  
`app-killer` is a powerful script that utilizes the **Shizuku API** (via `adb shell content` providers) in **Termux** to **force-stop all background apps**.

---

## ✨ Features & Advantages

- 🔋 **Save Battery**  
  Stops unnecessary background processes draining your device's power.

- ⚡ **Boost Performance**  
  Frees up RAM and CPU by killing non-essential apps, making your phone smoother.

- 🛡️ **Enhance Security**  
  Terminates unauthorized apps running silently in the background.

- 🔧 **ADB-Free Automation**  
  No need for root or a PC — control everything using **Shizuku** + **Termux** combo.

---

## ⚙️ Requirements

- Android device with **Shizuku** installed and active  
- **Termux** app (latest version)  
- Basic permissions granted for `adb shell content` access via Shizuku

---

## 🚀 Installation & Usage

1. **Install Shizuku** from [official site](https://shizuku.rikka.app/)
2. **Enable Shizuku** and allow access via wireless debugging (or root mode)
3. Open **Termux** and clone this repo:

   ```bash
   git clone https://github.com/yourusername/app-killer.git
   cd app-killer
   chmod +x app-killer.sh
