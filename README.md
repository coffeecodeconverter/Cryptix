# Cryptix
**Ultra-Portable, Offline-First Password Management**

## Introduction
**Cryptix** is a lightweight, high-security password manager and generator designed for users who demand total control over their data. Built as a standalone **HTML application**, Cryptix is truly platform-agnostic—it requires no installation, works entirely offline, and runs in any modern web browser. 

In an era of cloud-based breaches, Cryptix puts the "vault" back in your hands. Your credentials never touch a third-party server; they live only where you choose to keep them.

Try the Live Project Here: <br>
**https://turnerworks.uk/portfolio/cryptix/index.html**
<br>

<img width="1718" height="926" alt="image" src="https://github.com/user-attachments/assets/35bbb910-21d5-4672-a059-c58ff6ed2cb8" />

---

## 🔒 Security & Portability
Unlike traditional password managers that tie you to a specific OS or subscription, Cryptix is a single-file utility that travels with you on a USB drive, phone, or local machine.

*   **Offline-First Architecture:** All encryption and decryption happen locally in your browser. No internet connection is required to access your vault.
*   **Encrypted JSON Storage:** Your credentials are saved as a robustly encrypted JSON blob. This ensures your data is unreadable to anyone without your master key.
*   **No Vendor Lock-in:** Since the vault is stored as a standard (but encrypted) file, you can easily backup, move, or sync your data using your preferred method (Dropbox, Sync, or manual USB backups).

---

## 🚀 Key Features

### 🔑 Advanced Password Generation
Create cryptographically strong passwords on the fly. 
*   Customize length and character sets (symbols, numbers, casing).
*   Ensure every account has a unique, unhackable footprint.

### 📁 Import & Export System
Manage your data with zero friction:
*   **Export:** Save your encrypted vault to a local file whenever you make changes.
*   **Load:** Simply upload your encrypted JSON file and enter your master password to unlock your credentials.

### 📱 Zero-Footprint Portability
Because Cryptix is built with HTML/JS, it is compatible with:
*   **Windows / macOS / Linux**
*   **Android / iOS**
*   **USB "Live" Environments**

---

## 🛠 How It Works

1.  **Initialize:** Open the `Cryptix.html` file in your browser.
2.  **Generate or Entry:** Create new credentials using the built-in generator or manually enter your existing accounts.
3.  **Encrypt:** Enter your Master Password. Cryptix secures the data instantly.
4.  **Save:** Export the resulting encrypted JSON file to your device.
5.  **Retrieve:** To access your passwords later, load the JSON file into Cryptix and provide your Master Password to decrypt the view.

---

## 📂 Data Format Example
Your data is stored in a structured format that prioritizes both security and ease of future parsing:
```json
{
  "vault_name": "MySecureVault",
  "last_updated": "2026-05-12",
  "payload": "U2FsdGVkX1+V0...[ENCRYPTED_DATA]..."
}
