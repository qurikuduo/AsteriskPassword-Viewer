[![Build Windows](https://github.com/qurikuduo/AsteriskPassword-Viewer/actions/workflows/build.yml/badge.svg)](https://github.com/qurikuduo/AsteriskPassword-Viewer/actions/workflows/build.yml)

# AsteriskPassword

AsteriskPassword，A star password viewer developed using C++ and MFC.


<img width="584" height="374" alt="0" src="https://github.com/user-attachments/assets/7753fb79-850d-4bfb-b650-e5a73fb5c6d6" />



## 📌 About the Project
AsteriskPassword is a Windows utility designed to reveal passwords hidden behind asterisks (`*`).  
It is built using the Microsoft Foundation Class (MFC) library and can retrieve the actual text from standard password input boxes on Windows.

The tool works by letting the user drag a target icon (crosshair) onto any password field. When released, the real password is captured and displayed.

## ✨ Features
- Lightweight MFC-based Windows application  
- Reads the real text behind star-masked password controls  
- Simple and clean user interface  
- Drag-and-drop target selector  
- Supports ANSI and Unicode password fields  

## 🛠️ Usage
1. Launch the application.  
2. Press and hold the target (crosshair) icon.  
3. Drag it over the password input field you want to inspect.  
4. Release the mouse button — the password will appear in the text box inside the application.

## 📂 Building the Project
### Requirements
- Visual Studio 2022 or newer with MFC support  
- Windows SDK  
- C++17 or newer (optional)

### Build Steps
1. Open `Asterisk-Password.sln` in Visual Studio.  
2. Select either `Release|Win32` or `Debug|Win32`.  
3. Build using **Build → Build Solution**.  
4. The executable will be located in `Asterisk/Release/AsteriskPassword.exe` (or `Asterisk/Debug/AsteriskPassword.exe`).

### GitHub Actions
- `.github/workflows/build.yml` runs CI builds on pushes to `main` and on pull requests.
- `.github/workflows/main.yml` builds and publishes a GitHub release asset when you push a `v*` tag, or when you manually dispatch it with a tag and release name.
- Both workflows use `Asterisk/Release/AsteriskPassword.exe` as the final executable path.

## ⚠️ Legal Disclaimer
This tool is intended **only** for:
- Testing your own applications  
- Educational purposes  
- Security research on systems you own or have explicit permission to test  

Using this software to retrieve passwords without authorization is **illegal**.  
The user assumes full responsibility for any misuse of this application.

## 📜 License
This project can be distributed under the MIT License, or you may replace it with your preferred license.
