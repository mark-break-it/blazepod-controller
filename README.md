# 🎮 Reaction Arcade

**Fast reactions. Bright colors. Endless fun.**

Reaction Arcade is a collection of interactive, light-based reaction games for compatible wireless LED pods. Challenge your reflexes, test your memory, or compete against a friend.

It's a lightweight, mobile-friendly web application that connects directly to nearby devices over Bluetooth.

## 🕹️ Game Modes

### 🟢 Whack-a-Mole

Hit green targets and avoid red ones. Up to four pods can light up simultaneously.

- **Easy:** Lights stay on for 2–5 seconds.
- **Medium:** Lights stay on for 1–3 seconds.
- **Hard:** Lights stay on for 0.5–1.5 seconds.
- **Endless:** Starts on Easy and becomes more difficult every 30 seconds. After reaching Hard, light durations decrease by another 0.1 seconds every 30 seconds, with a minimum of 0.3 seconds.

A green target that goes out before you hit it does not count as a mistake. **Three red hits end the game.** Standard games last two minutes; Endless has no time limit.

### ⚡ Reflex Rush

A 60-second reaction challenge with one green target and two red targets.

- Green hit: +1 hit.
- Red hit: +1 miss.
- Unlit pods: no effect.
- **Final score = hits − misses.**

### 🆚 Reflex Rush VS

Two players, three pods each, and one winner after 60 seconds.

Each player has one correct target, one red target, and one unlit pod. Player 1 targets **green**; Player 2 targets **blue**. A correct hit adds one hit, and a red hit adds one miss.

The players' targets operate independently: hitting a pod only changes that player's three pods. The highest final score (**hits − misses**) wins.

### 🌈 Color Rush

A 60-second head-to-head challenge with all six pods illuminated in different colors.

- Player 1 scores by hitting **green**.
- Player 2 scores by hitting **blue**.
- Other colors do nothing.
- Every successful hit changes the colors across all six pods.

The palette is designed to keep non-target colors visually distinct from green and blue.

### 🧠 Simon Says

Watch a sequence of illuminated pods, then repeat it from memory.

- Six pods have distinct colors.
- At the start, the pods dim to approximately 20% brightness.
- A target lights up brightly for 2.5 seconds, then returns to its dim state.
- There is a 2-second pause between sequence steps.
- Each successful level adds one more step to the sequence.
- **One mistake ends the game.**

## ✨ Features

- Five game modes, including single-player and two-player challenges
- Real-time timers, scores, and game-over screens
- Adjustable difficulty and an Endless challenge
- Dynamic LED colors and reduced gameplay brightness
- Automatic connection to previously authorized devices where supported
- Mobile-friendly, illustrated game selection screen
- No account, backend, or installation of the game itself required

## 🚀 Getting Started

1. Power on your compatible wireless LED pods.
2. Open Reaction Arcade in a browser that supports the required Web Bluetooth features.
3. Allow Bluetooth access and connect your devices.
4. Choose a game mode and any relevant difficulty settings.
5. Press **Start** and play!

Some modes require all six pods; others can run with fewer.

## 📱 Mobile Browser & Bluetooth Setup

Reaction Arcade uses the **Web Bluetooth API**. Browser support differs across operating systems, and some browsers need an extension or a dedicated Bluetooth-capable browser.

### 🍎 iPhone / iOS — Tested setup

**This project is currently developed and tested only on an iPhone.**

Safari on iOS does not offer the Web Bluetooth functionality this project needs by itself. The working setup uses the **Beacio Web Bluetooth extension** with Safari.

1. Install **Beacio** from the App Store.
2. Open **Settings → Apps → Safari → Extensions** (the exact menu may vary by iOS version).
3. Enable the extension.
4. Grant the extension access to the Reaction Arcade website, using **Allow on This Website** or the equivalent option when prompted.
5. Turn on Bluetooth and make sure the wireless pods are powered on.
6. Open Reaction Arcade in Safari, then use the app's connection button.
7. Approve any Bluetooth or device-selection prompts.

If connection or discovery fails, verify that the extension is enabled and has permission to run on the site. First-time device authorization may require selecting devices individually before automatic reconnection becomes available.

### 🤖 Android — Not yet tested

**Chrome for Android** is a sensible starting point because it supports Web Bluetooth on compatible devices. A separate extension is generally not necessary.

1. Enable Bluetooth on your Android device.
2. Open Reaction Arcade in Chrome.
3. Tap the connection button.
4. Grant Bluetooth or nearby-device permissions if requested.
5. Select and connect your pods.

**Android has not been tested with this project.** Device discovery, automatic reconnection, and other Web Bluetooth features may behave differently depending on the browser and device.

### 🌐 Browser Compatibility

| Platform | Suggested browser/setup | Project test status |
| --- | --- | --- |
| iPhone / iOS | Safari with Beacio extension | ✅ Tested |
| Android | Chrome | 🧪 Not tested |
| Windows | Chrome or Edge | 🧪 Not tested |
| macOS | Chrome or Edge | 🧪 Not tested |
| iPhone Safari without extension | Missing required Web Bluetooth support | ❌ Unsupported setup |

### 🔐 Bluetooth Permissions & Privacy

- The browser requests permission before connecting to devices.
- Device communication takes place locally over Bluetooth.
- Gameplay does not require an account or cloud service.
- Web Bluetooth generally requires a **secure context**, such as an HTTPS website or localhost.

**Troubleshooting:** If devices do not appear, check that Bluetooth is enabled, the pods are on, browser/extension permissions are granted, and the pods are not already connected to another app.

## 🛠️ Technology

- HTML5
- CSS3
- Vanilla JavaScript
- Web Bluetooth API
- GitHub Pages

The application is a static website; no framework, build step, or backend server is required.

## 🔬 Project Status

**Experimental hobby project — work in progress.**

The app is being developed and tested with a specific iPhone setup. Hardware compatibility, game mechanics, and browser behavior may change as development continues.

## 📄 Disclaimer

This is an independent, unofficial hobby project and is not affiliated with, endorsed by, or sponsored by any hardware manufacturer. All trademarks and product names belong to their respective owners.

---

**Made for fun, speed, and a little friendly competition.** ⚡
