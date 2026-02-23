<div align="center">

# 🖥️ Fluxdesk Remote Desktop

### High-Performance Remote Desktop Solution with WebRTC & Real-Time Streaming

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![.NET](https://img.shields.io/badge/.NET-10.0-512BD4?logo=dotnet)](https://dotnet.microsoft.com/)
[![Platform](https://img.shields.io/badge/Platform-Windows-0078D6?logo=windows)](https://www.microsoft.com/windows)
[![WebRTC](https://img.shields.io/badge/WebRTC-Enabled-00C7B7?logo=webrtc)](https://webrtc.org/)
[![Avalonia](https://img.shields.io/badge/Avalonia-UI-7B68EE?logo=avalonia)](https://avaloniaui.net/)
[![GitHub release](https://img.shields.io/github/v/release/Raoufbaa/Fluxdesk-Releases?include_prereleases&style=flat-square)](https://github.com/Raoufbaa/Fluxdesk-Releases/releases)
[![Downloads](https://img.shields.io/github/downloads/Raoufbaa/Fluxdesk-Releases/total?style=flat-square)](https://github.com/Raoufbaa/Fluxdesk-Releases/releases)

## 🚀 Quick Download

[![Download Latest Release](https://img.shields.io/badge/Download-Latest%20Installer-success?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/Raoufbaa/Fluxdesk-Releases/releases/latest)

[![View All Releases](https://img.shields.io/badge/View-All%20Releases-blue?style=for-the-badge&logo=github)](https://github.com/Raoufbaa/Fluxdesk-Releases/releases)

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Configuration](#%EF%B8%8F-configuration) • [Architecture](#-architecture) • [Performance](#-performance) • [License](#-license)

</div>

---

## 📋 Overview

**Fluxdesk** is a cutting-edge remote desktop application built with **.NET 9** and **Avalonia UI**, designed for ultra-low latency control and high-performance screen streaming. It combines **DirectX Desktop Duplication API** for hardware-accelerated screen capture with **WebRTC DataChannels** for near-instantaneous input transmission, delivering a smooth remote desktop experience optimized for gaming, productivity, and real-time applications.

### ✨ Key Highlights

- 🚀 **WebRTC Ultra-Low Latency**: UDP-based input controls with <10ms response time
- 🎮 **Gaming-Optimized**: Touchpad & direct mouse modes, virtual joystick, WASD controls
- 📱 **Mobile-Friendly**: Responsive web interface with touch gestures and mobile optimization
- 🔒 **Secure PIN Authentication**: 6-digit PIN with automatic firewall configuration
- ⚡ **Adaptive Quality**: Dynamic quality adjustment based on network conditions
- 🎯 **Dirty Region Optimization**: Binary frame encoding reduces bandwidth by 70-95% in static scenes
- 🌐 **Ngrok Integration**: Global access via secure tunneling (optional)
- 🖼️ **Frame Interpolation**: Smooth 60 FPS experience even on lower frame rates

---

## 🎯 Features

### 🖱️ Advanced Input Control

- **🎯 Dual Mouse Modes**
  - **Direct Mode**: Absolute positioning - tap exactly where you want to click
  - **Touchpad Mode**: Relative movement - swipe to move cursor like a laptop touchpad
- **🕹️ Virtual Joystick**
  - Configurable WASD/ZQSD movement controls
  - Auto-lock forward movement feature
  - Adjustable joystick size (100-200px)
  - QWERTY/AZERTY keyboard layout support
  - Custom action buttons (Space, E, etc.)
- **👆 Touch Gestures**
  - Two-finger scrolling (vertical/horizontal)
  - Long-press for right-click
  - Pinch-to-zoom support
  - Swipe gestures for navigation
- **⌨️ Full Keyboard Support**
  - Physical keyboard input
  - Virtual keyboard for mobile devices
  - Key combinations (Ctrl+C, Ctrl+V, Alt+Tab, etc.)
  - Special keys (F1-F12, Windows key, etc.)
  - Text typing with automatic character mapping
- **🎨 Customizable Controls**
  - Drag-and-drop button positioning
  - Custom button creation with key combos
  - Resizable control elements
  - Save/load control layouts

### 🎥 High-Performance Streaming

- **⚡ DirectX Desktop Duplication**
  - Hardware-accelerated screen capture at 60 FPS
  - Zero-copy GPU memory access
  - Automatic recovery from display changes
  - Multi-monitor support ready
- **🔧 Multi-threaded JPEG Encoding**
  - Parallel frame processing with thread pooling
  - 4+ encoder threads for maximum throughput
  - Bitmap pooling for reduced GC pressure
  - Optimized memory allocation
- **📦 Binary Frame Protocol**
  - Custom dirty region tracking (64x64 tile-based)
  - Frame skip detection for identical frames
  - Selective tile encoding (only changed regions)
  - 70-95% bandwidth reduction in static scenes
  - Automatic keyframe insertion
- **🎚️ Adaptive Quality System**
  - 7 quality presets: Lowest → Native
  - Dynamic resolution scaling (480p → 4K)
  - Automatic quality adjustment based on encoding time
  - JPEG quality control (20-95)
  - Bandwidth optimization
- **🎬 Frame Interpolation**
  - Client-side 60 FPS interpolation
  - Smooth motion even at lower capture rates
  - Hardware-accelerated canvas rendering
  - Offscreen canvas compositing

### 🔧 System Management

- **📊 Process Manager**
  - View all running processes with memory usage
  - Filter by applications with windows
  - Kill/close processes remotely
  - Maximize/restore application windows
  - Real-time process list refresh
- **🚀 Quick App Launcher**
  - Windows Explorer
  - Default web browser
  - Steam client
  - Discord
  - Custom application support
- **⚙️ System Commands**
  - 🔒 Lock workstation
  - 😴 Sleep/suspend
  - 🔄 Restart
  - ⚡ Shutdown
  - 🚪 Sign out
  - 📊 Task Manager
- **🌐 Ngrok Tunneling**
  - Global internet access via secure tunnel
  - Automatic token management
  - Multi-port API detection (4040, 14040, 44040)
  - HTTPS/HTTP fallback support
  - Connection status monitoring

### 📊 Performance Monitoring

- **📈 Real-time Statistics**
  - FPS counter
  - Bandwidth usage (Mbps)
  - Frame encoding time
  - Dirty region ratio
  - Connection latency
  - WebSocket status
- **🎛️ 5 Stats Display Levels**
  - Hidden: No stats
  - Minimal: FPS only
  - Basic: FPS + Bandwidth
  - Standard: + Latency + Quality
  - Full: All telemetry data

### ⚙️ Advanced Configuration

- **🎨 UI Customization**
  - Drag-and-drop button positioning
  - Resizable control elements
  - Custom button creation
  - Layout save/restore
  - Edit mode with visual guides
- **🎮 Control Settings**
  - Joystick size adjustment
  - Mouse sensitivity
  - Scroll speed
  - Touch gesture sensitivity
  - Keyboard layout (QWERTY/AZERTY)
- **📺 Display Settings**
  - FPS limiter (10/30/60/Unlimited)
  - Quality presets (7 levels)
  - Adaptive quality toggle
  - Frame interpolation toggle
  - Fullscreen mode
- **🔋 Power Management**
  - Wake lock support (prevent screen sleep)
  - Battery-saving mode
  - Automatic disconnect on idle

### 🔐 Security Features

- **🔑 PIN Authentication**
  - 6-digit PIN code generation
  - Session-based authentication
  - Automatic PIN rotation
  - Secure WebSocket connections
- **🛡️ Firewall Integration**
  - Automatic Windows Firewall configuration
  - Port 8080 access management
  - Network interface detection
  - Security rule creation

### 🎯 Keyboard Shortcuts

- **📋 Common Actions**
  - Ctrl+C / Ctrl+V: Copy/Paste
  - Ctrl+T: New tab
  - Ctrl+W: Close tab
  - Alt+Tab: Switch windows
  - Alt+F4: Close window
  - Win+D: Show desktop
  - Win+R: Run dialog
  - Ctrl+Alt+Del: Security screen

---

## 🛠️ Installation

### System Requirements

- **Operating System**: Windows 10/11 (64-bit)
- **Runtime**: .NET 9 Runtime (included in installer)
- **Privileges**: Administrator access (for firewall configuration)
- **Graphics**: DirectX 11 compatible GPU with updated drivers
  - NVIDIA: GeForce 400 series or newer
  - AMD: Radeon HD 5000 series or newer
  - Intel: HD Graphics 2000 or newer
  - **Important**: Install latest GPU drivers from manufacturer's website
- **Network**: WiFi or Ethernet connection
- **RAM**: 2GB minimum, 4GB recommended
- **CPU**: Multi-core processor recommended for encoding

### Quick Start

1. **Download the installer**

   Click the button below to download the latest version:

   [![Download Fluxdesk](https://img.shields.io/badge/Download-Fluxdesk_Setup.exe-brightgreen?style=for-the-badge&logo=windows)](https://github.com/Raoufbaa/Fluxdesk-Releases/releases/latest)

2. **Run the installer**

   Double-click `Fluxdesk_Setup.exe` and follow the installation wizard. The installer will:

   - Install Fluxdesk application
   - Configure Windows Firewall rules
   - Create desktop and start menu shortcuts
   - Set up automatic updates (optional)

3. **Launch Fluxdesk**

   Find Fluxdesk in your Start Menu or Desktop shortcut. The application will:

   - Start the local web server on port 8080
   - Generate a secure 6-digit PIN
   - Display connection URLs (local + mobile)
   - Configure firewall automatically

4. **Connect from any device**

   Open the displayed URL in your mobile browser or another PC:

   - **Local**: `http://localhost:8080`
   - **Mobile**: `http://192.168.x.x:8080`
   - **Online**: Enable ngrok for global access

### Alternative: Manual Installation

If you prefer to download specific versions, visit our [Releases page](https://github.com/Raoufbaa/Fluxdesk-Releases/releases).

### GPU Driver Installation

For optimal performance, ensure you have the latest GPU drivers installed:

- **NVIDIA**: Download from [nvidia.com/drivers](https://www.nvidia.com/Download/index.aspx)
- **AMD**: Download from [amd.com/support](https://www.amd.com/en/support)
- **Intel**: Download from [intel.com/graphics](https://www.intel.com/content/www/us/en/download-center/home.html)

DirectX 11 support is required for hardware-accelerated screen capture.

---

## 📖 Usage

### Starting a Remote Session

1. **Launch Fluxdesk** on your Windows PC (host machine)

   - The server starts automatically on launch
   - A 6-digit PIN is generated for authentication
   - Connection URLs are displayed in the terminal

2. **Note the connection details** displayed in the application:

   - **PIN**: 6-digit code (e.g., `123456`)
   - **Local**: `http://localhost:8080`
   - **Mobile**: `http://192.168.x.x:8080` (your local IP)
   - **Online**: Enable ngrok for internet access

3. **Open the web interface** on your client device:

   - Enter the URL in your browser
   - Input the 6-digit PIN when prompted
   - Wait for WebRTC connection to establish

4. **Start controlling** your PC remotely!
   - Use touch gestures on mobile
   - Use mouse/keyboard on desktop
   - Enable virtual joystick for gaming

### Control Modes

**🎯 Direct Mouse Mode**

- Tap/click exactly where you want the cursor to go
- Absolute positioning for precision
- Best for: Desktop use, precise clicking

**🖱️ Touchpad Mode**

- Swipe to move cursor relative to current position
- Like using a laptop touchpad
- Best for: Mobile devices, general navigation

**🕹️ Virtual Joystick**

- On-screen WASD controls for gaming
- Configurable action buttons
- Auto-lock forward movement
- Best for: Gaming, 3D applications

### Ngrok Online Mode

Enable global internet access via ngrok tunneling:

1. **Get ngrok token**

   - Sign up at [ngrok.com](https://ngrok.com)
   - Copy your authentication token

2. **Enable online mode**

   - Click "START ONLINE" in Fluxdesk
   - Paste your ngrok token when prompted
   - Wait for tunnel to establish

3. **Share the URL**
   - Copy the public URL (e.g., `https://abc123.ngrok.io`)
   - Share with remote users
   - They can connect from anywhere in the world

---

## ⚙️ Configuration

### Quality Settings

Adjust streaming quality based on your network:

| Preset       | Resolution | Bandwidth | Use Case                        |
| ------------ | ---------- | --------- | ------------------------------- |
| **Lowest**   | 480p       | ~0.5 Mbps | Mobile data, very slow networks |
| **Very Low** | 540p       | ~1 Mbps   | Slow WiFi, battery saving       |
| **Low**      | 720p       | ~2 Mbps   | Standard WiFi                   |
| **Medium**   | 1080p      | ~5 Mbps   | Good WiFi (default)             |
| **High**     | 1440p      | ~10 Mbps  | Fast WiFi                       |
| **Ultra**    | 4K         | ~20 Mbps  | Gigabit LAN                     |
| **Native**   | Full       | ~30 Mbps  | Maximum quality                 |

### FPS Settings

Control frame rate for performance/quality balance:

- **10 FPS**: Battery saving, low bandwidth
- **30 FPS**: Standard streaming (recommended)
- **60 FPS**: Smooth gaming and video
- **Unlimited**: Maximum performance (120+ FPS)

### Adaptive Quality

Enable automatic quality adjustment:

- Monitors encoding time
- Reduces quality if encoding is slow
- Increases quality when performance improves
- Maintains target frame rate

### Frame Interpolation

Enable client-side 60 FPS interpolation:

- Smooth motion even at lower capture rates
- Hardware-accelerated rendering
- Minimal CPU overhead
- Best with 30 FPS capture

### Firewall Configuration

Fluxdesk automatically configures Windows Firewall on first launch. If manual configuration is needed:

1. Open Windows Firewall with Advanced Security
2. Create new Inbound Rule
3. Rule Type: Port
4. Protocol: TCP, Port: 8080
5. Action: Allow the connection
6. Profile: All (Domain, Private, Public)
7. Name: Fluxdesk Remote Desktop

---

## 🏗️ Architecture

### Technology Stack

**Backend (Server)**

- **.NET 9**: Modern C# runtime with performance optimizations
- **Avalonia UI**: Cross-platform XAML-based UI framework
- **ASP.NET Core**: Web server and API endpoints
- **SharpDX**: DirectX 11 bindings for screen capture
- **SIPSorcery**: WebRTC implementation for real-time communication

**Frontend (Client)**

- **Vanilla JavaScript**: No framework dependencies
- **WebRTC DataChannels**: Ultra-low latency input transmission
- **WebSocket**: Binary frame streaming
- **Canvas API**: Hardware-accelerated rendering
- **OffscreenCanvas**: Background frame compositing

### System Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                     Fluxdesk Server                         │
│  ┌──────────────────────────────────────────────────────┐  │
│  │              Avalonia UI (MainWindow)                │  │
│  │  • Server control • PIN display • Terminal output    │  │
│  └──────────────────────────────────────────────────────┘  │
│                            ↓                                │
│  ┌──────────────────────────────────────────────────────┐  │
│  │           ASP.NET Core Web Server (Port 8080)        │  │
│  │  • Static file serving • WebSocket middleware        │  │
│  │  • REST API endpoints • Authentication               │  │
│  └──────────────────────────────────────────────────────┘  │
│                            ↓                                │
│  ┌──────────────────────────────────────────────────────┐  │
│  │                    Services Layer                     │  │
│  │  ┌────────────────┐  ┌────────────────┐             │  │
│  │  │ScreenCapture   │  │ InputControl   │             │  │
│  │  │• DirectX API   │  │• Mouse/Keyboard│             │  │
│  │  │• JPEG Encoding │  │• Win32 API     │             │  │
│  │  │• Dirty Regions │  │• Gestures      │             │  │
│  │  └────────────────┘  └────────────────┘             │  │
│  │  ┌────────────────┐  ┌────────────────┐             │  │
│  │  │ WebRTC Service │  │ Process Mgmt   │             │  │
│  │  │• Peer Conn.    │  │• App Launch    │             │  │
│  │  │• DataChannels  │  │• System Cmds   │             │  │
│  │  │• ICE Handling  │  │• Task Manager  │             │  │
│  │  └────────────────┘  └────────────────┘             │  │
│  │  ┌────────────────┐  ┌────────────────┐             │  │
│  │  │ Ngrok Service  │  │ Auth Service   │             │  │
│  │  │• Tunneling     │  │• PIN Generation│             │  │
│  │  │• Token Mgmt    │  │• Validation    │             │  │
│  │  └────────────────┘  └────────────────┘             │  │
│  └──────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────┘
                            ↕
                    Network (WebSocket + WebRTC)
                            ↕
┌─────────────────────────────────────────────────────────────┐
│                     Web Client (Browser)                    │
│  ┌──────────────────────────────────────────────────────┐  │
│  │                  User Interface                       │  │
│  │  • Canvas display • Virtual controls • Menu system   │  │
│  └──────────────────────────────────────────────────────┘  │
│                            ↓                                │
│  ┌──────────────────────────────────────────────────────┐  │
│  │              JavaScript Application                   │  │
│  │  ┌────────────────┐  ┌────────────────┐             │  │
│  │  │ Frame Decoder  │  │ Input Handler  │             │  │
│  │  │• Binary Parser │  │• Touch Events  │             │  │
│  │  │• JPEG Decode   │  │• Mouse/Keyboard│             │  │
│  │  │• Dirty Regions │  │• Gestures      │             │  │
│  │  └────────────────┘  └────────────────┘             │  │
│  │  ┌────────────────┐  ┌────────────────┐             │  │
│  │  │ WebRTC Client  │  │ Frame Renderer │             │  │
│  │  │• DataChannel   │  │• Canvas API    │             │  │
│  │  │• ICE/STUN      │  │• Interpolation │             │  │
│  │  │• Heartbeat     │  │• Compositing   │             │  │
│  │  └────────────────┘  └────────────────┘             │  │
│  └──────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────┘
```

### Data Flow

**Screen Capture Pipeline**

1. DirectX Desktop Duplication captures screen at 60 FPS
2. Dirty region detection identifies changed areas (64x64 tiles)
3. Multi-threaded JPEG encoding compresses frames
4. Binary protocol packages full frames or dirty regions
5. WebSocket sends compressed data to client
6. Client decodes and renders to canvas

**Input Control Pipeline**

1. Client captures input events (touch, mouse, keyboard)
2. WebRTC DataChannel sends control messages (<10ms latency)
3. Server receives and parses control messages
4. InputControlService executes Win32 API calls
5. System processes input as if from local user

---

## ⚡ Performance

### Optimization Techniques

**Server-Side**

- 🚀 **Hardware Acceleration**: DirectX Desktop Duplication API
- 🧵 **Multi-threading**: 4+ parallel JPEG encoder threads
- 🎯 **Dirty Region Detection**: 70-95% bandwidth reduction
- 🔄 **Frame Skip Detection**: Identical frame elimination
- 💾 **Memory Pooling**: Bitmap reuse, reduced GC pressure
- ⚡ **Process Priority**: High priority for capture thread
- 🎚️ **Adaptive Quality**: Dynamic quality adjustment
- 📦 **Binary Protocol**: Efficient frame packaging

**Client-Side**

- 🎨 **Hardware Rendering**: GPU-accelerated canvas
- 🖼️ **OffscreenCanvas**: Background frame compositing
- 🎬 **Frame Interpolation**: Smooth 60 FPS display
- 📊 **Request Animation Frame**: Optimized render loop
- 💾 **Efficient Decoding**: Native JPEG decode
- 🔄 **Dirty Region Blending**: Selective canvas updates

### Performance Metrics

**Typical Performance** (1080p @ 30 FPS, Medium quality)

- **Latency**: 15-30ms (input to display)
- **Bandwidth**: 2-5 Mbps (with dirty regions)
- **CPU Usage**: 10-20% (server), 5-10% (client)
- **Memory**: ~200MB (server), ~100MB (client)
- **Frame Time**: 10-20ms encoding

**Gaming Performance** (1080p @ 60 FPS, High quality)

- **Latency**: 20-40ms
- **Bandwidth**: 8-15 Mbps
- **CPU Usage**: 20-30% (server), 10-15% (client)
- **Frame Time**: 8-15ms encoding

**Static Content** (Desktop, documents)

- **Bandwidth**: 0.1-1 Mbps (95% reduction)
- **Frame Skip**: 80-90% identical frames
- **Dirty Regions**: 1-5% of screen

---

## 🔧 Development

### Building from Source

**Prerequisites**

- .NET 9 SDK
- Visual Studio 2022 or VS Code
- Windows 10/11 SDK

**Clone and Build**

```bash
git clone https://github.com/Raoufbaa/Fluxdesk.git
cd Fluxdesk
dotnet restore
dotnet build
dotnet run
```

**Publish Single-File Executable**

```bash
dotnet publish -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true
```

### Project Structure

```
Fluxdesk/
├── Controllers/          # API endpoints
│   ├── AuthController.cs
│   └── WebRTCController.cs
├── Services/            # Business logic
│   ├── ScreenCaptureService.cs
│   ├── InputControlService.cs
│   ├── WebRTCService.cs
│   ├── NgrokService.cs
│   ├── ProcessManagementService.cs
│   ├── SystemCommandService.cs
│   └── AppLaunchService.cs
├── Middleware/          # WebSocket handling
│   └── WebSocketMiddleware.cs
├── Models/              # Data models
│   ├── AppInfo.cs
│   ├── ProcessInfo.cs
│   └── WebSocketMessage.cs
├── Helpers/             # Utility classes
│   ├── FirewallHelper.cs
│   ├── NgrokHelper.cs
│   └── ConsoleRedirect.cs
├── wwwroot/             # Web client
│   ├── index.html
│   ├── remote.html
│   ├── Scripts/
│   │   ├── Remote.js
│   │   └── FrameInterpolator.js
│   └── styles/
│       └── remote.css
├── MainWindow.axaml     # UI definition
├── MainWindow.axaml.cs  # UI logic
├── Program.cs           # Entry point
└── Fluxdesk.csproj      # Project file
```

### Key Dependencies

```xml
<PackageReference Include="Avalonia" Version="11.1.3" />
<PackageReference Include="SharpDX.Direct3D11" Version="4.2.0" />
<PackageReference Include="SharpDX.DXGI" Version="4.2.0" />
<PackageReference Include="SIPSorcery" Version="8.0.0" />
<PackageReference Include="System.Drawing.Common" Version="8.0.0" />
```

---

## 🐛 Troubleshooting

### Common Issues

**Server won't start**

- Check if port 8080 is already in use
- Run as Administrator for firewall configuration
- Verify .NET 9 runtime is installed

**Can't connect from mobile**

- Ensure devices are on same network
- Check firewall allows port 8080
- Verify IP address is correct

**Poor performance**

- Lower quality preset
- Reduce FPS to 30
- Enable adaptive quality
- Check network bandwidth

**Black screen**

- Verify DirectX 11 support (run `dxdiag` to check)
- Update graphics drivers to latest version:
  - NVIDIA: [nvidia.com/drivers](https://www.nvidia.com/Download/index.aspx)
  - AMD: [amd.com/support](https://www.amd.com/en/support)
  - Intel: [intel.com/graphics](https://www.intel.com/content/www/us/en/download-center/home.html)
- Check display permissions
- Restart application after driver update

**Input lag**

- Use WebRTC DataChannel (not WebSocket)
- Check network latency
- Reduce quality/FPS
- Close bandwidth-heavy applications

**Ngrok not working**

- Verify token is correct
- Check internet connection
- Ensure ngrok.exe is in project root
- Try different API ports

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **SharpDX** - DirectX bindings for .NET
- **SIPSorcery** - WebRTC implementation
- **Avalonia** - Cross-platform UI framework
- **ngrok** - Secure tunneling service
- **Font Awesome** - Icon library

---

## 📞 Support

- 🐛 **Issues**: [GitHub Issues](https://github.com/Raoufbaa/Fluxdesk-Releases/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/Raoufbaa/Fluxdesk-Releases/discussions)
- � **\*Releases**: [Download Page](https://github.com/Raoufbaa/Fluxdesk-Releases/releases)

---

## 🗺️ Roadmap

### Planned Features

- [ ] 🖥️ Multi-monitor support
- [ ] 🎮 Gamepad/controller support
- [ ] 🔊 Audio streaming
- [ ] 📹 Video codec support (H.264/VP9)
- [ ] 🔐 End-to-end encryption
- [ ] 👥 Multi-user sessions
- [ ] 📱 Native mobile apps (iOS/Android)
- [ ] 🐧 Linux server support
- [ ] 🍎 macOS server support
- [ ] 📊 Session recording
- [ ] 🌍 Internationalization (i18n)
- [ ] 🎨 Custom themes
- [ ] 📦 Portable version
- [ ] 🔄 Auto-update system

---

<div align="center">

**Made with ❤️ by the Fluxdesk Team**

⭐ Star us on GitHub — it motivates us a lot!

[![GitHub stars](https://img.shields.io/github/stars/Raoufbaa/Fluxdesk?style=social)](https://github.com/Raoufbaa/Fluxdesk/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/Raoufbaa/Fluxdesk?style=social)](https://github.com/Raoufbaa/Fluxdesk/network/members)

</div>
