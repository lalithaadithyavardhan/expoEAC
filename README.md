# 📱 Android APK Build Guide (Expo EAS)

This guide outlines the steps to build a standalone Android APK for this project using **EAS (Expo Application Services)**.


## 🛠️ Initial Setup (One-Time Only)

Follow these steps if you are setting up the project for the first time.

### 1. Install EAS CLI
Open your terminal or command prompt in the project folder and install the EAS CLI globally:

```bash
npm install -g eas-cli
```

Verify the installation:
```bash
eas --version
```

### 2. Login to Expo
Authenticate with your Expo account:

```bash
expo login
```
> *Note: Log in with the same account used for development.*

### 3. Configure EAS
Generate the build configuration file (`eas.json`):

```bash
eas build:configure
```

**During configuration:**
- ✅ It creates an `eas.json` file.
- ✅ Choose **Android** when asked.
- ✅ Select **APK** (not AAB) if prompted, or ensure your `eas.json` has a `preview` profile configured for APK generation.

---

## 🚀 Building the APK

Perform these steps whenever you want to generate a new installable file.

### 4. Start the Build
Run the following command to build the APK using the preview profile:

```bash
eas build -p android --profile preview
```

**What happens next?**
- ☁️ Expo uploads your latest code.
- ⚙️ The cloud builder compiles your APK.
- ⏳ **Wait time:** Approximately 5–10 minutes.

### 5. Download & Install
Once the build is complete:
1. The terminal will show a **download link**.
2. Or, visit your dashboard: Expo Builds → Projects → Builds.
3. 📥 **Download** the `.apk` file.
4. 📲 **Install** it directly on your Android phone.

🎉 **DONE! Your updated app is ready.**

---

## 🔁 Updating the App

Every time you change your code and want a new APK, just run:

```bash
eas build -p android --profile preview
```

> No QR codes, no reinstalling Expo Go required.
