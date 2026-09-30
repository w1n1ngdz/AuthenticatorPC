# Authenticator PC (Windows Desktop) 🔐

A lightweight, secure desktop Two-Factor Authentication (2FA / TOTP) manager for Windows with modern dark mode styling, master password protection, and versatile QR code import tools.

Designed for users who want to generate, manage, and back up their 2FA codes directly on their PC without needing their smartphone.

---

## 🚀 Downloads (Ready-to-Use Installers)

Pre-built standalone installers are available for download directly from the repository / [Releases](https://github.com/w1n1ngdz/AuthenticatorPC/releases):

| Operating System | Setup Installer | Architecture |
| :--- | :--- | :--- |
| **Windows 10 / Windows 11** | [`GoogleAuthenticator_Win10_11_Setup.exe`](https://github.com/w1n1ngdz/AuthenticatorPC/blob/main/GoogleAuthenticator_Win10_11_Setup.exe) | 64-bit (x64) |
| **Windows 7 / Legacy Windows** | [`GoogleAuthenticator_Win7_32bit_Setup.exe`](https://github.com/w1n1ngdz/AuthenticatorPC/releases) | 32-bit (x86) & 64-bit |

> [!NOTE]
> No Python runtime or technical dependencies required. Just download and run the installer.

---

## ✨ Features

- **⏱️ Live 30-Second TOTP Generation**: Real-time 6-digit verification codes with visual progress countdown bar.
- **📋 One-Click Copy**: Click the copy icon to paste TOTP codes or secret keys instantly.
- **📥 Multiple Import Methods**:
  - **🖼️ Image File**: Import QR code screenshots (`.png`, `.jpg`, `.bmp`, `.webp`).
  - **📋 Clipboard Paste**: Paste a copied QR code or screenshot directly (`Ctrl+V` equivalent button).
  - **🔑 Manual Secret Key**: Add accounts manually via standard Base32 secret codes.
  - **📷 Live Webcam Scanning**: Scan QR codes directly using your computer's webcam.
- **🔄 Google Authenticator Migration Support**: Fully compatible with `otpauth-migration://` export QR codes as well as standard `otpauth://` URIs.
- **🔒 Master Password Protection**: Optional startup lock screen with SHA-256 hashed master password to protect your accounts from unauthorized access.
- **📤 Export & QR Viewer**: Re-generate and display the QR code for any stored account anytime to transfer between devices.
- **🎨 Modern Dark Mode UI**: Clean, responsive desktop user interface with French and English installer support.

---

## 📦 Installation & Getting Started

1. Go to the [Releases](https://github.com/w1n1ngdz/AuthenticatorPC/releases) page (or the uploaded installer files in this repo).
2. Download the installer matching your Windows edition:
   - For modern PCs (Windows 10 / 11): Download **`GoogleAuthenticator_Win10_11_Setup.exe`**.
   - For older systems (Windows 7 / 8 / 32-bit): Download **`GoogleAuthenticator_Win7_32bit_Setup.exe`**.
3. Run the installer and follow the setup wizard (optional desktop shortcut creation).
4. Launch **Authenticator PC** from your Start menu or Desktop!

---

## 🛠️ How to Import Accounts

### 1. From Google Authenticator App (Transfer Accounts)
1. On your phone, open **Google Authenticator** > tap menu / settings > **Transfer accounts** > **Export accounts**.
2. Either:
   - Take a picture or screenshot and load it via **"Import QR Image"** or **"Paste QR from Clipboard"**.
   - Or click **"Scan via Webcam"** and hold the phone screen up to your PC camera.

### 2. From Any Online Service (Google, GitHub, Discord, Binance, etc.)
- When enabling Two-Factor Authentication on a website:
  - Take a screenshot of the QR code and use **Paste QR from Clipboard** or **Browse Image File**.
  - Or copy the secret text key provided by the site and paste it into **"Enter Key Code"**.

---

## 🔒 Security & Privacy

- **100% Offline Storage**: Your keys never leave your device. All TOTP tokens are calculated locally following RFC 6238 specifications.
- **Local Vault**: Accounts are stored in your user profile app data folder (`%LOCALAPPDATA%\GoogleAuthenticatorApp\`).
- **Optional Master Lock**: Enable master password protection to lock the app upon startup.

---

## 📄 License

This binary release is distributed under the [MIT License](LICENSE).
<img width="1680" height="1050" alt="image" src="https://github.com/user-attachments/assets/8d291aed-b510-4016-a6fc-c14d468937f2" />
