<div align="center">

# 🖥️ Fluxdesk Remote Desktop

### High-Performance Remote Desktop Solution with WebRTC & Real-Time Streaming

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![.NET](https://img.shields.io/badge/.NET-9.0-512BD4?logo=dotnet)](https://dotnet.microsoft.com/)
[![Platform](https://img.shields.io/badge/Platform-Windows-0078D6?logo=windows)](https://www.microsoft.com/windows)
[![WebRTC](https://img.shields.io/badge/WebRTC-Enabled-00C7B7?logo=webrtc)](https://webrtc.org/)
[![GitHub release](https://img.shields.io/github/v/release/Raoufbaa/Fluxdesk?include_prereleases&style=flat-square)](https://github.com/Raoufbaa/Fluxdesk/releases)
[![Downloads](https://img.shields.io/github/downloads/Raoufbaa/Fluxdesk/total?style=flat-square)](https://github.com/Raoufbaa/Fluxdesk/releases)

## 🚀 Quick Download

[![Download Latest Release](https://img.shields.io/badge/Download-Latest%20Installer-success?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/Raoufbaa/Fluxdesk/releases/download/latest/Fluxdesk_Setup.exe)

[![View All Releases](https://img.shields.io/badge/View-All%20Releases-blue?style=for-the-badge&logo=github)](https://github.com/Raoufbaa/Fluxdesk/releases)

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Configuration](#%EF%B8%8F-configuration) • [License](#-license)

</div>

---

## 📋 Overview

**Fluxdesk** is a cutting-edge remote desktop application built with **.NET 9** and **Avalonia UI**, designed for ultra-low latency control and high-performance screen streaming[web:85][web:88]. It combines **DirectX Desktop Duplication** for efficient screen capture with **WebRTC DataChannels** for near-instantaneous input transmission, delivering a smooth remote desktop experience optimized for gaming and real-time applications[web:85][web:86].

### ✨ Key Highlights

- 🚀 **WebRTC Ultra-Low Latency**: UDP-based input controls with <10ms response time
- 🎮 **Gaming-Optimized**: Touchpad & direct mouse modes, virtual joystick, WASD controls
- 📱 **Mobile-Friendly**: Responsive web interface with touch gestures
- 🔒 **Secure PIN Authentication**: 6-digit PIN with automatic firewall configuration
- ⚡ **Adaptive Quality**: Dynamic quality adjustment based on network conditions
- 🎯 **Dirty Region Optimization**: Binary frame encoding for reduced bandwidth

---

## 🎯 Features

### 🖱️ Control Features

- **Dual Mouse Modes**: Direct mapping or touchpad-style cursor control
- **Virtual Joystick**: Configurable WASD movement controls with lock feature
- **Gesture Support**: Two-finger scrolling, long-press for right-click
- **Keyboard Integration**: Full keyboard input with combo support (Ctrl+Alt+Del, etc.)
- **Custom Buttons**: Programmable action buttons for quick commands

### 🎥 Streaming Technology

- **DirectX Desktop Duplication**: Hardware-accelerated screen capture at 60 FPS
- **Multi-threaded JPEG Encoding**: Parallel frame processing for maximum throughput
- **Binary Frame Protocol**: Custom dirty region tracking for efficient updates
- **Adaptive Quality**: 5 quality presets (Very Low → Ultra) with auto-adjustment
- **Offscreen Canvas Compositing**: Smooth dirty region blending

### 🔧 System Management

- **Process Manager**: View, kill, and maximize running applications
- **App Launcher**: Quick launch for Explorer, Browser, Steam, Discord
- **System Commands**: Lock, Sleep, Shutdown, Restart, Sign Out
- **Task Manager Integration**: Direct access to Windows Task Manager

### ⚙️ Configuration

- **Customizable HUD**: 5 stats display levels (hidden to full telemetry)
- **Button Positioning**: Drag-and-drop UI customization in edit mode
- **Joystick Sizing**: Adjustable virtual joystick size
- **Quality Presets**: Fine-tune streaming quality vs. performance
- **Wake Lock Support**: Prevent mobile screen timeout during sessions

---

## 🛠️ Installation

### System Requirements

- **Operating System**: Windows 10/11 (64-bit)
- **Runtime**: .NET 9 Runtime (included in installer)
- **Privileges**: Administrator access (for firewall configuration)
- **Graphics**: DirectX 11 compatible GPU
- **Network**: WiFi or Ethernet connection

### Quick Start

1. **Download the installer**
   
   Click the button below to download the latest version:
   
   [![Download Fluxdesk](https://img.shields.io/badge/Download-Fluxdesk_Setup.exe-brightgreen?style=for-the-badge&logo=windows)](https://github.com/Raoufbaa/Fluxdesk/releases/download/latest/Fluxdesk_Setup.exe)

2. **Run the installer**
   
   Double-click `Fluxdesk_Setup.exe` and follow the installation wizard[web:85][web:91].

3. **Launch Fluxdesk**
   
   Find Fluxdesk in your Start Menu or Desktop shortcut[web:85].

4. **Connect from any device**
   
   Open the displayed URL in your mobile browser or another PC[web:85][web:88].

### Alternative: Manual Installation

If you prefer to download specific versions, visit our [Releases page](https://github.com/Raoufbaa/Fluxdesk/releases)[web:88][web:90].

---

## 📖 Usage

### Starting a Remote Session

1. **Launch Fluxdesk** on your Windows PC (host machine)
2. **Note the connection details** displayed in the application:
   - Local IP address (e.g., `192.168.1.100:5000`)
   - 6-digit PIN code (e.g., `123456`)
3. **Open the web interface** on your client device:
   - Enter `http://<host-ip>:5000` in your browser
   - Input the 6-digit PIN when prompted
4. **Start controlling** your PC remotely!

### Control Modes

**Direct Mouse Mode**: Move your cursor exactly where you tap/click[web:85].

**Touchpad Mode**: Swipe to move cursor, tap to click (like a laptop touchpad)[web:85].

**Virtual Joystick**: Use on-screen WASD controls for gaming applications[web:85].

---

## ⚙️ Configuration

### Quality Settings

Adjust streaming quality based on your network:

- **Very Low**: 480p, ~1 Mbps (mobile data)
- **Low**: 720p, ~2 Mbps (slow WiFi)
- **Medium**: 1080p, ~5 Mbps (standard WiFi)
- **High**: 1440p, ~10 Mbps (fast WiFi)
- **Ultra**: 4K, ~20 Mbps (gigabit LAN)

### Firewall Configuration

Fluxdesk automatically configures Windows Firewall on first launch[web:85]. If manual configuration is needed:

