ADK Windows Wallet is a desktop client for interacting with the Aidos Kuneen (ADK) distributed ledger.

The application is designed as a single-asset, protocol-focused wallet, aligned with the architecture and direction of the ADK ecosystem.

This repository provides a modern desktop wallet interface and serves as a foundation for future integration with the ADK DAG network.

Key Characteristics
ADK-only wallet (no multi-asset support)
Desktop application for Windows
Designed for DAG-native interaction
Clean, minimal protocol-terminal interface
Structured for future node connectivity and synchronization
Modular architecture for extension and integration
Current Status

⚠️ Development / Demo Version

This version provides:

User interface and wallet flow simulation
ADK address format validation
Transaction UI (send / receive / activity)
Node / DAG status interface (placeholder)

This version does not yet include:

Live ADK network connectivity
Real transaction broadcasting
Verified cryptographic wallet implementation
Proof-of-Work (PoW) execution
Installation
Requirements
Windows 10 or later
Node.js (LTS)
Clone Repository
git clone https://github.com/AidosKuneen/adk-windows-wallet.git
cd adk-windows-wallet
Install Dependencies
npm install
Running the Wallet

Start the application in development mode:

npm start
Building for Windows
Option 1 — Automated Build

Double-click:

build-windows.bat
Option 2 — Manual Build
npm run dist
Build Output

Compiled binaries are generated in:

/release

Artifacts include:

Portable executable (.exe)
Installer package (Setup.exe)
Versioning

This project follows a simple semantic versioning model:

MAJOR.MINOR.PATCH

Example:

0.1.0
0.x indicates early-stage development
Increment MINOR for feature updates
Increment PATCH for fixes
Releases

To create a release:

Build the wallet:

npm run dist
Go to GitHub → Releases
Click “Create new release”
Tag version (e.g. v0.1.0)
Upload files from /release
Publish release
ADK Address Format

The wallet follows the Aidos Kuneen address specification:

Character set: A–Z and 9
Length:
81 trytes (without checksum)
90 trytes (with checksum)
Project Structure
assets/          → Branding and icons
main.js          → Electron main process
preload.js       → Secure bridge layer
index.html       → UI structure
styles.css       → Visual styling
app.js           → Wallet logic (demo)
package.json     → Project configuration
Roadmap

Planned development phases:

ADK node / API integration

Real address derivation (ADK-compatible)

Transaction creation and broadcasting

Proof-of-Work (PoW) integration

DAG synchronization and status tracking

Secure key management

Production release

Security Notice

This software is not production-ready.

Do not use with real funds until:

cryptographic functions are implemented and verified
network connectivity is stable
security audits are completed
Contributing

Contributions are welcome.

Please:

fork the repository
create a feature branch
submit a pull request
License

Open-source, part of the Aidos Kuneen ecosystem.

Aidos Kuneen

GitHub:
https://github.com/aidoskuneen
