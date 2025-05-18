# ⚔️ APP-KILLER — Termux Shizuku Background App Terminator ⚡

**Boldly eliminate background apps with the power of Shizuku!**  
`app-killer` is a powerful script that utilizes the **Shizuku API** (via `adb shell content` providers) in **Termux** to **force-stop all background apps**.

---

## ✨ Features & Advantages

- 🔋 **Save Battery** – Stop unnecessary background processes draining your device’s power.  
- ⚡ **Boost Performance** – Free up RAM and CPU by killing non-essential apps.  
- 🛡️ **Enhance Security** – Kill unauthorized apps running silently in the background.  
- 🔧 **ADB-Free Automation** – No root required — just Shizuku + Termux.

---

## ⚙️ Requirements

- Android 10 or above (best with Android 11+ for wireless debugging)  
- **Shizuku** app (active and running)  
- **Termux** installed  
- Internet access (for setup and repo clone)

---

## 🚀 Installation & Usage

🔴**termux tutorial**: [YT WATCH 🎥📸](https://youtube.com/shorts/CQb2CHg9rKg?si=zRhEUVMkBy2mD01B)

### 📦 Step 1: Install Termux

- **GitHub**: [termux-app/releases](https://github.com/termux/termux-app/releases)  
- **F-Droid**: [f-droid.org Termux](https://f-droid.org/en/packages/com.termux/)

> **Note**: ❌ **Do NOT use the Play Store version** — it's outdated and unsupported.

---

### 🧩 Step 2: Install Shizuku
🔴**setup videos on**: [YT WATCH 🎥📸](https://youtube.com/shorts/DLphMCEZSqE?si=V6Gr--hg58G9zFyQ)
- **GitHub**: [Shizuku/releases](https://github.com/RikkaApps/Shizuku/releases)  
- **Official Site**: [shizuku.rikka.app](https://shizuku.rikka.app/download/)  
- **Play Store**: [Shizuku on Play Store](https://play.google.com/store/apps/details?id=moe.shizuku.privileged.api)

> **Note:**  
> i) Also available on F-Droid  
> ii) Recommended: Android 11+ for Wireless Debugging  
> iii) Android 10 or lower requires PC for setup (mini guide below)

---

## 📡 Setup Shizuku on Android 10+ (Wireless Debugging)

1. **Connect your device** to any **Wi-Fi** and turn on a **mobile hotspot** (needed for pairing).  
2. Open **Shizuku App** → **Grant all required permissions**.  
3. Tap **"Pairing"** section → Click the **blue button** (Developer Options).  
4. **Enable Developer Options**, scroll down:
    - Enable **USB debugging**
    - Enable **Wireless debugging**  
    *(If you can't enable Wireless Debugging, see PC setup below)*  
5. Tap the **" | "** icon beside Wireless Debugging → opens full menu.  
6. Tap **"Pair device with pairing code"** → Enter the 6-digit code shown.  
    - **IMPORTANT**: Don’t close the code screen until paired!  
    - If no popup shows: scroll from the top, open notification, then enter code there.  
7. Once paired, you’ll see **Shizuku** in the "Paired devices" list.  
8. Return to **Shizuku home**, tap **Start** (blue button).  
9. You’ll now see **"Shizuku is running"** at the top!  

> **Note**:  
> If a **red warning** appears under "Shizuku is running" — go to **Settings**, search and enable:  
> **"Disable permission monitoring"**

You're now ready to use **Shizuku-API** in other apps/scripts.

---

## ⚔️ Setup app-killer in Termux

1. Open **Termux** and run:

   ```bash
   pkg install git
   git clone https://github.com/yourusername/app-killer.git
   cd app-killer
   chmod +x app-killer.sh
   ./app-killer.sh
