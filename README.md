# SysBlock
<img align="left" src="images/ic_launcher.png" width="140" />
SysBlock is a powerful, self-imposed digital wellbeing tool for Android designed to help you regain control of your time. It combines app blocking, usage limits, and strict "freeze" protocols to prevent you from bypassing your own rules.

## Key Features

*   **App Blocking:** Block distracting apps completely or set daily usage limits (e.g., "30m", "1h").
*   **Master Switch:** A global toggle to enable or disable all blocking rules instantly.
*   **Freeze Protocol:** Lock specific lines of your configuration for set time periods (e.g., "08:00 AM - 05:00 PM"). During this time, you cannot edit or delete those rules.
*   **Uninstall Protection:** Optional Device Admin permission prevents the app from being force-stopped or uninstalled, ensuring you stick to your commitment.
*   **Raw Config Editor:** Advanced users can edit the `CONFIG.SYS` file directly for precise control over rules.

## Getting Started

### Installation

1.  Download the latest APK from the [Releases](https://github.com/estiaksoyeb/SysBlock-Releases/releases) page.

<p align="left">
        <a href="https://github.com/estiaksoyeb/SysBlock-Releases/releases/download/1.0.1/SysBlock-1.0.1.apk">
            <img src="https://img.shields.io/badge/Download-SysBlock%20APK-green?style=for-the-badge&logo=android" alt="Download SysBlock">
        </a>
</p>

2.  Install the APK on your Android device.
3.  Grant the necessary permissions:
    *   **Accessibility:** Required to detect and block app launches.
    *   **Usage Access:** Required to track daily app usage time.

### Basic Usage

1.  **Home Screen:** View active rules and system status. Use the "Master Switch" to toggle protection.
2.  **Manage Apps:** Tap "MANAGE BLOCKED APPS" to select apps.
    *   Tap an app to set a limit (e.g., `30m`) or leave it blank for an instant block.
    *   New rules are appended to your configuration.
3.  **Advanced Editor:** Tap "EDIT RAW" to access the configuration file directly.
    *   **Syntax:** `SET | APPLOCK | com.package.name | 30m`
    *   **Freeze:** Tap the gear icon ⚙️ to schedule times when specific lines cannot be edited.

## Configuration Guide

The `CONFIG.SYS` file drives the app's behavior.

*   **Block an App:** `SET | APPLOCK | com.facebook.katana | 30m`
*   **Master Switch:** `SET | MASTER_SWITCH | true`
*   **Uninstall Protection:** Add `PREVENT_UNINSTALL` on a new line.

## Developer

**Istiak Ahmmed Soyeb**

*   [Twitter](https://twitter.com/estiaksoyeb)
*   [GitHub](https://github.com/estiaksoyeb)
*   [Telegram](https://t.me/estiaksoyeb)

## Proprietary Software

This project is **Closed Source**. All rights are reserved by the developer. Unauthorized distribution, modification, or reverse engineering is prohibited.

