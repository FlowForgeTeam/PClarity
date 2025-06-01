# PClarity  
> Desktop productivity analytics that respects your privacy  

[🚀 Jump to Development Setup](#development-environment-setup)

## What is PClarity?  

PClarity is an open-source Windows application that helps you understand how you spend time on your computer. Unlike cloud-based alternatives, all your data stays on your machine.  

## Key Features  

- 📊 **Automatic Time Tracking** - Track application usage without manual timers 
- 📈 **Productivity Analytics** - Visualize your computer usage patterns 
- 💻 **System Monitoring** - CPU, RAM, GPU usage in one place  

## Why PClarity?  

- **Lightweight** - Built with C++ and Electron for optimal performance
- **Offline First** - Works without internet connection 
- **Open Source** - Transparent, auditable, and community-driven 
- **Free Forever** - Core features will always be free  

## Tech Stack  

- **Backend:** C++ with Win32 API
- **Frontend:** Electron + Node.js
- **Package Manager:** vcpkg (C++)
- **Database:** SQLite (local storage)

## Status  

🚧 **Under Development** - First release coming soon!  

---  

Made with ❤️ by FlowForge Team  

---  

## Development Environment Setup

### Prerequisites

- **Windows Platform** (required for Win32 API calls)
- **Visual Studio 2019/2022** with C++ development tools
- **Node.js** (LTS version recommended)
- **vcpkg** package manager
- **C++20** compiler support

### Setup Instructions

#### 1. Install Visual Studio
- Download and install Visual Studio with C++ desktop development workload
- Ensure C++20 standard library support is included
- Set your platform target to Windows

#### 2. Set up vcpkg
- Follow the [official vcpkg installation guide](https://vcpkg.io/en/getting-started.html)
- Clone vcpkg repository and run bootstrap script
- Integrate vcpkg with Visual Studio: `vcpkg integrate install`

#### 3. Install C++ Dependencies
```bash
vcpkg install nlohmann-json:x64-windows
```

#### 4. Set up Node.js and Electron
- Install Node.js from [official website](https://nodejs.org/)
- Follow the [official Electron setup guide](https://www.electronjs.org/docs/latest/tutorial/quick-start)
- Install project dependencies: `npm install`

#### 5. Configure C++ Project
- Set C++ standard to C++20 in Visual Studio project properties
- Ensure `<filesystem>` header is available (requires C++17/20)
- Configure vcpkg toolchain integration

#### 6. Build and Run
- Build the C++ backend using Visual Studio
- Start the Electron frontend: `npm start`

### Additional Resources
- [Win32 API Reference](https://docs.microsoft.com/en-us/windows/win32/)
- [Electron Documentation](https://www.electronjs.org/docs/)
- [vcpkg Documentation](https://vcpkg.io/en/docs/)

For detailed setup instructions, refer to the official guides for each technology.