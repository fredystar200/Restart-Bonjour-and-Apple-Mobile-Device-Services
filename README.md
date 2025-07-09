# Restart-Bonjour-and-Apple-Mobile-Device-Services

A simple Windows batch script to restart the **Apple Mobile Device Service** and **Bonjour Service** with automatic elevation of administrative privileges.

---

## Description

This script helps quickly restart two important Apple services on Windows machines:

- **Apple Mobile Device Service** — Required for iTunes and Apple device connectivity.
- **Bonjour Service** — Apple's zero-configuration networking service.

If these services become unresponsive or you experience connection issues with Apple devices, running this script can help resolve the problem by restarting them.

The script automatically checks for administrator privileges and requests elevation if necessary, so you can run it seamlessly.

---

## Features

- Automatically detects if the script is running with admin rights.
- Requests admin privileges if not already elevated.
- Stops and restarts the **Apple Mobile Device Service**.
- Stops and restarts the **Bonjour Service**.
- Simple, lightweight, and easy to use.

---

## Usage

1. [**Download the script here**](https://github.com/fredystar200/Restart-Bonjour-and-Apple-Mobile-Device-Services/releases)

2. Run it directly by **double-clicking** or **right-click > Run as administrator**.

3. Alternatively, launch it from PowerShell with administrative privileges using the command below:

```powershell
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/fredystar200/Restart-Bonjour-and-Apple-Mobile-Device-Services/main/Restart%20Bonjour%20and%20Apple%20Mobile%20Device%20Services.bat" -OutFile "$env:TEMP\Restart Bonjour and Apple Mobile Device Services.bat"; Start-Process -FilePath "$env:TEMP\Restart Bonjour and Apple Mobile Device Services.bat" -Verb RunAs
```

4. The script will stop and start the two services automatically.
