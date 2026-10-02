# Over-OS

### The New Gaming Software for Windows 11

**Transform your Windows PC into a console experience.**

Over-OS is a modern Windows 11 gaming layer inspired by the best console experiences, bringing a fast Game Hub, Control Center, automatic cooling, game optimization, controller integration, notifications and much more into one application.



---

## 🚀 Features

### 1. ❄️ Automatic Cooling

A dedicated cooling application integrated into Over-OS.

* Automatic fan control
* Temperature monitoring
* CPU/GPU temperature tracking
* Custom cooling profiles
* Game-specific profiles
* Different fan speeds depending on the game
* Automatic performance/cooling mode
* Quiet mode
* Performance mode
* Custom fan curves
* Hardware monitoring

Example:

```text
eFootball
├── CPU Temperature: 61°C
├── GPU Temperature: 58°C
├── Fan: 65%
└── Profile: Performance
```

Users can configure different cooling behaviour for individual games.

---

### 2. 🏠 Over-OS Home & Control Center

A modern console-style Home interface for Windows.


Launch:

* 🎮 Games
* 🌐 Web browsers
* 📁 Applications
* ⚙️ Settings
* 🎵 Music
* 🖥️ Utilities

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/81e5aa78-dd9d-4b31-86ad-1dce21ef9f92" />

### Control Center

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/be9a46c5-6dab-4586-b115-507785c8e0f5" />

Press **F12** to open the Over-OS Control Center without leaving the current application.

Includes:

* 🔊 Volume
* 🎙️ Microphone
* 📶 Wi-Fi
* 🔵 Bluetooth
* ☀️ Brightness
* 🎮 Controller
* 🎵 Music
* 🔔 Notifications
* ⚡ Performance Mode
* ❄️ Cooling
* 💡 RGB
* 🖥️ Display
* 🔋 Battery
* 📸 Capture
* ⏱️ System information
* 👤 User profile

### Brightness Control

Change display brightness directly from Over-OS without opening Windows Display Settings.

Supports:

* Desktop monitors
* Laptops
* Multiple displays where supported
* Hardware/software brightness control

---

### 3. 🌐 Built-in Browser

Over-OS includes an integrated browser.

Use it for:

* Game guides
* YouTube
* Discord Web
* Game wikis
* Search
* Downloads
* Streaming
* Quick web access

The browser can be opened directly from the Home or Control Center.

---

### 4. ⚡ Ultra-Fast Game Optimization

When a game starts, Over-OS can activate a dedicated Game Optimization profile.

Goals:

* Prioritize the active game
* Reduce unnecessary background activity
* Reduce CPU usage from non-essential applications
* Reduce RAM usage where possible
* Optimize process priorities
* Pause optional background tasks
* Activate performance profiles
* Restore the previous state when the game closes

Example:

```text
GAME DETECTED
────────────────────

eFootball.exe

Game Optimization
       ACTIVE ✓

CPU Priority       HIGH
Background Tasks   REDUCED
Memory Usage       OPTIMIZED
Performance Mode   ON
```

Over-OS should avoid modifying critical Windows processes or services.

---

### 5. 🎮 Console Experience

Over-OS brings many console-style features to Windows.

Inspired by modern console UX:

* Home
* Control Center
* Game Library
* Game Switcher
* Recent Games
* User Profiles
* Notifications
* Music Controls
* Quick Settings
* Controller Center
* Performance Center
* Capture tools
* Friends/communication integrations
* Game status
* System status
* Quick resume-style workflows

The goal is simple:

> **Make Windows feel like a gaming console without replacing Windows.**

---

### 6. 💡 Dynamic Controller LED

Compatible controllers can dynamically change their lighting depending on the game.

Supported concept:

* PlayStation DualSense
* DualShock
* Xbox controllers where hardware/API support allows
* Other compatible RGB controllers

### Game Lighting

Example:

```text
Minecraft
→ Green

Cyberpunk 2077
→ Yellow

Rocket League
→ Blue

Horror Game
→ Dark Red

eFootball
→ White / Team Color
```

---

## 🎨 Intelligent Screen Color Detection

Over-OS can optionally detect the dominant colour of the active game and use it for compatible controller lighting.

### Region of Interest

Instead of analysing the entire screen, Over-OS focuses on the central **50% of the screen**, reducing interference from:

* Black bars
* HUD elements
* Windows UI
* Dark corners
* Other non-game areas

### 1×1 Pixel Sampling

The selected region can be reduced to a single pixel to obtain an approximate average colour extremely efficiently.

```text
FULL SCREEN
┌──────────────────────────────┐
│                              │
│      ┌────────────────┐      │
│      │                │      │
│      │    GAME AREA   │      │
│      │      ████      │      │
│      │                │      │
│      └────────────────┘      │
│                              │
└──────────────────────────────┘
             ↓
       COLOR SAMPLING
             ↓
          RGB COLOR
             ↓
      CONTROLLER LED
```

The capture system should be optimized to minimize CPU/GPU overhead and avoid affecting gameplay.

---

### 7. 🔔 Notification System

Modern notifications inspired by console UX.

Examples:

#### 🎵 Music Changed

```text
┌─────────────────────────────────┐
│ 🎵 NOW PLAYING                  │
│                                 │
│ Song Name                       │
│ Artist                          │
│                                 │
│              ▶                 │
└─────────────────────────────────┘
```

Other notifications:

* 🎮 Controller connected
* 🔋 Controller battery
* 🎮 Game started
* 🎮 Game closed
* 🏆 Achievement
* ⚡ Performance mode enabled
* ❄️ Cooling profile changed
* 📥 Download completed
* 🔔 System notifications
* 🎵 Music changed
* 🔌 USB device connected
* 📶 Network status

Notifications should use smooth animations and a modern dark/glass interface.

---

## 🖥️ Interface

Design direction:

**PlayStation-inspired + Windows 11 + modern glass UI**

Characteristics:

* Dark interface
* Glass effects
* Smooth animations
* Rounded cards
* Subtle shadows
* Gradient backgrounds
* Controller-first navigation
* Keyboard/mouse support
* 60 FPS UI animations
* Minimal interface
* Responsive layouts

---

## 🧩 Architecture

```text
Over-OS
│
├── OverOS.exe
│
├── Home
│   ├── Game Library
│   ├── Applications
│   ├── Browser
│   └── Recent Games
│
├── Control Center
│   ├── Audio
│   ├── Network
│   ├── Brightness
│   ├── Controller
│   ├── Performance
│   ├── Cooling
│   └── Notifications
│
├── Gaming Engine
│   ├── Game Detection
│   ├── Optimization
│   ├── Profiles
│   └── Process Management
│
├── Cooling Engine
│   ├── Temperature Monitor
│   ├── Fan Profiles
│   └── Game Profiles
│
├── Controller Engine
│   ├── DualSense
│   ├── Xbox
│   ├── HID
│   └── Dynamic Lighting
│
├── Media Engine
│   ├── Music
│   ├── Album Art
│   └── Media Controls
│
├── Notification Engine
│
└── Settings
```

---

## 🎯 Vision

Over-OS is designed to make Windows feel less like a traditional desktop and more like a dedicated gaming platform.

**One application.**

**One interface.**

**One gaming experience.**

> **Over-OS — Your Windows. Your Console.**
