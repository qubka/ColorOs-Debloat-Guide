# ColorOs Debloat Chinese Content

## 📑 Table of Contents

- [📱 How to Enable Google Services, Gboard & Google Wallet](#-how-to-enable-google-services-gboard--google-wallet)
  - [✅ 1. Enable Google Services (GMS)](#-1-enable-google-services-gms)
  - [🎹 2. Set Up Gboard (Google Keyboard)](#-2-set-up-gboard-google-keyboard)
  - [💳 3. Set Up Google Wallet (NFC Payments)](#-3-set-up-google-wallet-nfc-payments)
- [🧹 How to Remove Chinese Content from Quick Glance](#-how-to-remove-chinese-content-from-quick-glance)
- [🔍 How to Replace Chinese Global Search](#-how-to-replace-chinese-global-search)
- [🔵 How to Enable Google Circle to Search](#-how-to-enable-google-circle-to-search)
- [⏰ How to Fix Delayed Notifications & Allow Background Apps](#-how-to-fix-delayed-notifications--allow-background-apps)
- [🛠️ More ColorOS Essentials](#-more-coloros-essentials)


## 📱 How to Enable Google Services, Gboard & Google Wallet

This guide helps you fully integrate Google's apps and services on Chinese ColorOS builds.

---

### ✅ 1. Enable Google Services (GMS)

1. Go to:  
   `Settings → System & Update → Google Settings`

2. Enable:  
   `Google Mobile Services (GMS)`

3. Install Google Play Store:  
   Use the default **App Market** on your device (search for `"App Market"`).

---

### 🎹 2. Set Up Gboard (Google Keyboard)

1. Open Google Play Store → Search and install **[Gboard](https://play.google.com/store/apps/details?id=com.google.android.inputmethod.latin)**
2. Go to:  
   `Settings → System & Update → Keyboard & Input Method`
3. Set current keyboard to: **Gboard**
4. *Optional Cleanup*:
    - Uninstall all Chinese input methods except for Baidu Input (system app)
5. *Secure Keyboard for Passwords*
    - Disabling is optional, makes password typing easier

---

### 💳 3. Set Up Google Wallet (NFC Payments)

1. Install **[Google Wallet](https://play.google.com/store/apps/details?id=com.google.android.apps.walletnfcrel)** from Google Play
2. Go to:  
   `Settings → AI → Disable EZPay`
3. Then go to:  
   `Settings → Connection & Sharing → NFC`
    - Enable **NFC**
    - Set **Default Payment App** to: **Google Wallet**

You’re now ready to use Google services, input via Gboard, and tap to pay with Google Wallet!

---

## 🧹 How to Remove Chinese Content from Quick Glance

If you're seeing Chinese content (like "trending news", Breeno, etc.) in your notification panel, here’s how to clean it up completely.

### Step-by-step Instructions:

1. Go to:  
   `Settings → Home screen & Lock screen → Swipe down on Home`  
   → Set to `"Notification & Quick Settings"`

2. Swipe down on the Home screen to open the notification panel
3. Tap the top-left user icon
4. Tap the gear icon (top-right) to enter **Quick Glance** settings
5. Disable features:

#### Under "Customize Layout":

- Disable Quick Functions
- Disable Recommended Services
- Disable Trending News

#### Under "Notification Settings":

- Disable New Update Notifications
- Disable Service Notifications
- Disable Basic Notifications

6. Add widgets to fill the panel
    - Use an **even number** of widgets to avoid the Chinese "Add Widget" button

**Useful widgets in English**:
- Weather
- Battery
- Storage
- Steps
- Connected Devices

✅ **Done!** Your notification panel should now be clean and free of Chinese content.

⚠️ *Note: Some widgets still contain Chinese text, but most essentials are translated.*

---

## 🔍 How to Replace Chinese Global Search

If your Global Search is still in Chinese, switch to the English version:

### Step-by-step:

1. Go to:  
   `Settings → Home screen & Lock screen → Enable "Show Search at Bottom"`

2. Install **[Oppo Global Search](https://play.google.com/store/apps/details?id=com.oppo.quicksearchbox)** from Google Play
3. Go to:  
   `Settings → Apps → App Management`  
   → Tap 3 dots (top-right) → **Enable "Show System Apps"**

4. Find **Global Search** in the list
5. Tap it → **Storage Usage** →
    - Press **Clear Data** and **Clear Cache**

6. Go back to Home Screen
    - Tap the bottom search bar
    - Select the newly installed **Oppo Global Search** as default

✅ **Done!** Bottom search now works in English with no Chinese suggestions.

⚠️ *Note: This doesn’t affect the search in the notification panel ("Quick Glance").*

---

## 🔵 How to Enable Google Circle to Search

Workaround using MiCTS and Google Assistant

### Setup Steps:

1. Disable all Breeno/AI stuff:  
   `Settings → AI → Disable:`
    - Breeno
    - Breeno Suggestions
    - Breeno Touch
    - Breeno Memory
    - AI Search
    - AI Voice Subscribe

2. Install **[MiCTS](https://github.com/parallelcc/MiCTS/releases/)**
    - Download APK from the release page

3. Install from Google Play:
    - Google
    - Google Voice Search
    - Google Assistant

4. Verify Google Assistant:
    - Open Google App → Profile → Settings → Google Assistant
    - Go to: **Digital Assistants from Google**
    - Ensure **Google Assistant** is selected (not Gemini)

5. If MiCTS has issues:
    - Check troubleshooting guide on GitHub

6. *(Optional)* Bind gesture to trigger Circle to Search
    - Use **[Vivid N.G](https://play.google.com/store/apps/details?id=com.ivianuu.oneplusgestures)** (Play Store)
    - [Root] Use **Xposed Edge** via **Xposed Framework**

7. **Post-Setup Configuration:**  
   `Settings → Apps → Auto Launch`
    - Add:
        - Google
        - Google Assistant
        - MiCTS
        - Your gesture app (e.g., Vivid N.G)

   Also in your gesture app, enable background activity

🎉 Enjoy Circle to Search functionality!

---

## ⏰ How to Fix Delayed Notifications & Allow Background Apps

Tired of delayed app alerts? These steps keep apps alive and responsive.

✅ Fixing just the first 2 options is usually enough. The rest are for maximum reliability.

---

### 1. Disable Cached App Suspension

Enable Developer Mode:  
`Settings → About Device → Version`  
→ Tap **"Version number" 7 times** → You are now a developer!

Then:  
`Settings → System & Update → Developer Options → Apps`  
→ **Suspend execution for cached apps → Disable**  
*(Requires reboot)*

---

### 2. Disable Sleep Standby Optimization

`Settings → Battery → Power Saving Settings → Sleep standby optimization`  
→ Disable this setting

---

### 3. Disable App Management

`Settings → Apps → App Management → [Your App] → Manage App If Unused`  
→ Disable this

---

### 4. Allow Background Activity

`Settings → Apps → App Management → [Your App] → Battery Usage`  
→ Select: **Allow Background Activity**

---

### 5. Enable Auto Launch

`Settings → Apps → Auto Launch → [Your App]`  
→ Enable **Auto Launch**

---

### 6. [Root] Use FCM Fix Module

If rooted, install **[FCMFix](https://github.com/kooritea/fcmfix)** Magisk module  
→ Fixes Google Firebase (FCM) delayed notifications

---

## 🛠️ More ColorOS Essentials

### 1. Disable Lock Screen Magazine

`Settings → Home Screen & Lock Screen → Lock Screen Magazine`  
→ Disable

---

### 2. Disable Calendar Spam

`Calendar App → Settings → Displayed Items`  
→ Disable:
- Subscriptions
- Service Reminders
- Suggested Events
- Recommendation Channels

---

### 3. Disable App Market Notifications

`Settings → Notifications → Manage Notifications`  
→ Find & disable noisy system apps

---

### 4. Remove Default Chinese Apps

`Settings → Apps → App Management`  
→ Uninstall or disable what you can

---

### ⚠️ Don't ADB Uninstall Critical System Apps!

Do **NOT** remove core apps like **Browser** or **App Market** via ADB  
→ May cause bootloops or OS instability

Instead:

- Just **hide them** from the launcher
- Don’t use them as default apps
- Avoid uninstalling without root & backup

---

### 5. Optional Modules for Rooted Devices

- **[magisk-module-oplus-cn2global](https://github.com/AndroPlus-org/magisk-module-oplus-cn2global)** → Restore Google Location + Nearby
- **[fcmfix](https://github.com/kooritea/fcmfix)** → Fix delayed notifications
- **[App Manager](https://github.com/MuntashirAkon/AppManager) / [Canta](https://github.com/samolego/Canta)** → Safely remove system apps

---

✅ These tweaks help clean your phone and make it fully usable with Google services.
