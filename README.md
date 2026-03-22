# Bubbles Accessibility Input System (BAIS)

![Version](https://img.shields.io/badge/version-0.0.20-blue)
![Platform](https://img.shields.io/badge/platform-Windows%20x64-0078D6)
![Electron](https://img.shields.io/badge/Electron-App-47848F?logo=electron)
![License](https://img.shields.io/badge/license-Custom-lightgrey)
![Status](https://img.shields.io/badge/status-Public%20Release-orange)
![Accessibility](https://img.shields.io/badge/focus-Accessibility-green)
![Security](https://img.shields.io/badge/security-No%20Stealth%20Behavior-brightgreen)

Bubbles Accessibility Input System (BAIS) is a desktop accessibility input utility for Windows. It gives you a clear, visible place to tune safe simulated input behavior using profiles, sensitivity controls, deadzone controls, smoothing, and shared or inherited settings.

BAIS is designed as a foundation for lawful accessibility workflows only. It does not hide itself, run stealth processes, tamper with memory, spoof processes, or attempt to bypass protections.

Current release: `0.0.20`

## ⬇️ Download BAIS

👉 [Download Latest Installer (v0.0.20)](https://github.com/KernFerm/Bubbles-Accessibility-Input-System-BAIS/releases/tag/Bubbles-Accessibility-Input-System-BAIS)

- > Windows x64 Installer
- > No setup required beyond installer
- > Safe, visible application

---

## 🚀 What's New in 0.0.20

- Added **Hip Aim Mouse Sensitivity control**
- Added **ADS Mouse Sensitivity control**
- Added **Smoothing modes**
  - Off
  - Light
  - Balanced (default)
  - Strong
- Added **Settings Inheritance system**
  - Shared → ADS inheritance behavior
  - Visual UI indication for inherited values
- Improved **profile system stability**
- Improved **device detection reliability**
- Improved **UI clarity and layout**

---

## What BAIS Is

BAIS is a Windows desktop application focused on accessible input configuration and safe simulation previewing.

It is intended to help users:

- detect supported controllers and accessibility-oriented input sources
- preview how profile changes affect simulated movement output
- tune Hip and ADS behavior without hidden background behavior
- save reusable profiles for different devices or accessibility needs

BAIS is a visible user-controlled utility. It is not presented as a background service, hidden component, or stealth tool.

---

## What The Application Does

BAIS helps you preview and manage accessibility-oriented input settings for different input sources in one place.

You can use it to:

- detect available gamepads automatically
- work with Xbox controllers
- work with PlayStation controllers
- work with accessibility controllers exposed through the Gamepad API
- work with keyboard input as an accessibility source
- work with mouse or trackpad input as an accessibility source
- work with touch-capable devices when available
- work with assistive switch or remapped keyboard-style input
- work with eye gaze or head tracking pointer-style input
- adjust **Hip Aim Mouse Sensitivity**
- adjust **ADS Mouse Sensitivity**
- adjust deadzone behavior
- apply smoothing modes to the safe simulation preview
- use shared or inherited settings
- choose ADS activation per input source
- save and load settings as JSON profiles

The app shows a live simulated output preview so you can see how your settings affect movement values before expanding the project further.

---

## Supported Input Sources

BAIS currently supports these visible input sources:

- Xbox controllers detected through the Gamepad API
- PlayStation controllers detected through the Gamepad API
- accessibility controllers detected through the Gamepad API
- keyboard input using WASD or arrow keys
- mouse or trackpad input
- touch input on touch-capable systems
- assistive switch or remapped keyboard-style input
- eye gaze or head tracking pointer-style input

---

## Top Menu Bar

The application includes a visible top menu bar with quick actions.

### File

- Refresh Devices
- Start Simulation
- Stop Simulation
- Emergency Stop
- Exit

### Profiles

- Save Current Profile
- Load Selected Profile
- Refresh Profile List

### View

- Reload Window
- Force Reload Window
- Toggle Developer Tools
- Zoom controls

### Help

- Usage Tips
- About BAIS

---

## How To Use BAIS

### 1. Start The Application

- Launch BAIS from the installer or development environment
- Wait for the interface to fully load

### 2. Choose An Input Source

In the Devices panel:

- click Refresh Devices if needed
- choose an Xbox controller, PlayStation controller, accessibility controller, keyboard, mouse or trackpad, touch input, assistive switch input, or eye gaze input from the selector
- read the device description shown in the list

### 3. Adjust Settings

Use the Shared, Hip, and ADS sections to tune behavior.

Available settings include:

- Shared Deadzone
- Shared Smoothing
- ADS Activation for the selected input source
- Hip Aim Mouse Sensitivity
- Hip Deadzone
- Hip Smoothing
- ADS Mouse Sensitivity
- ADS Deadzone
- ADS Smoothing
- Settings Inheritance

### 4. Start The Safe Simulation Preview

Click Start to begin the visible simulation preview.

While running:

- gamepad input uses the selected controller sticks and the user-selected ADS button
- keyboard input uses WASD or arrow keys, with Shift used for ADS mode by default and a Disabled option available if the user does not want keyboard ADS
- mouse or trackpad input uses pointer movement, with right mouse button down used for ADS mode by default
- touch input uses drag movement, with two touch points used for ADS mode
- assistive switch input uses keyboard-style movement and can use a configured ADS key or Disabled
- eye gaze or head tracking input uses pointer-style movement and can use a configured ADS key

Use Stop to end the preview normally.

Use Emergency Stop to halt the preview immediately.

---

## Settings Explained

### Hip Aim Mouse Sensitivity

Controls how strongly Hip movement is scaled in the simulation preview.

### ADS Mouse Sensitivity

Controls how strongly Aim Down Sight movement is scaled in the simulation preview.

### ADS Activation

Each input source can use its own ADS trigger.

- Mouse or trackpad defaults to right mouse button down
- Keyboard defaults to Shift
- Keyboard ADS can be disabled if the user does not want a keyboard ADS trigger
- Touch defaults to two touch points
- Gamepads default to left trigger and can be changed per controller family
- Accessibility switch input defaults to Shift and can also be disabled
- Eye gaze or head tracking can use a configured ADS key while pointer movement remains active

### Deadzone

Deadzone removes small movements near the center point. This is useful when you want to reduce unwanted drift or accidental motion.

### Smoothing

Smoothing softens changes between one output value and the next.

Available modes:

- Off
- Light
- Balanced
- Strong

Default smoothing is Balanced.

### Settings Inheritance

When Settings Inheritance is enabled, ADS deadzone and ADS smoothing inherit the Shared values. BAIS makes this clear by disabling those ADS controls and showing the inherited values directly in the UI.

When Settings Inheritance is disabled, ADS deadzone and ADS smoothing become fully editable on their own.

---

## Profiles

Profiles are saved as JSON files in the per-user application data profile store. Bundled defaults are seeded on first run.

You can:

- create or update a profile by entering a profile name and clicking Save Profile
- choose an existing profile from the dropdown and click Load Profile
- refresh the available profile list from the Profiles menu or the UI

The included `default.json` file provides a starting profile.

---

## Change Log

Version history is tracked in [change-log.md](./change-log.md).

---

## For Users

BAIS is meant to be easy to understand:

- choose an input source
- tune values
- preview the simulated output
- save a profile
- load it later

Everything is visible and user-controlled.

---

## Accessibility And Safety Scope

BAIS is for lawful accessibility and input customization only.

It does not include:

- hidden processes
- anti-detection behavior
- anti-cheat evasion
- process masking or spoofing
- driver-level code
- memory tampering
- stealth injection
