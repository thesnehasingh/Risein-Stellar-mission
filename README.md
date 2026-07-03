# 🚀 STELLAR // MISSION CONTROL

> A Stellar testnet dApp with a NASA-inspired terminal UI — built for the Rise In Stellar Journey to Mastery, Level 1 White Belt Challenge.

![Stellar Testnet](https://img.shields.io/badge/Network-Stellar%20Testnet-orange?style=flat-square)
![Freighter](https://img.shields.io/badge/Wallet-Freighter-yellow?style=flat-square)
![HTML](https://img.shields.io/badge/Built%20With-HTML%20%2F%20JS-green?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)

---

## 📌 Project Description

**Stellar Mission Control** is a single-page decentralized application (dApp) built on the **Stellar Testnet**. It uses the **Freighter** browser wallet extension for secure key management — your private key never leaves your browser.

The UI is inspired by NASA ground control terminals: amber phosphor text on near-black, CRT scanlines, and live data panels — making it visually distinct from every other submission.

### ✅ Features

| Feature | Description |
|---|---|
| 🔗 Wallet Connect | Connect / disconnect Freighter wallet with one click |
| 💰 Live Balance | Fetches real XLM balance from Horizon API |
| 💵 USD Conversion | Shows your XLM balance converted to USD (live price) |
| 📤 Send XLM | Single send with address, amount, and optional memo |
| 📦 Batch Send | Send XLM to multiple addresses in one transaction |
| 📷 QR Code | Auto-generates a scannable QR of your wallet address |
| 📋 Transaction Log | Last 20 operations with type, amount, peer, date & explorer link |
| 📡 Network Stats | Live ledger number, base fee, and TPS from Horizon |
| ⚡ Boot Animation | Terminal-style animated system check on page load |

---

## 🛠️ Setup Instructions (Run Locally)

### Prerequisites

- A modern browser (Chrome / Brave / Firefox)
- [Freighter Wallet](https://freighter.app) browser extension installed
- Freighter set to **Testnet** (Settings → Network → Test SDF Network)
- A funded testnet account — use [Stellar Friendbot](https://laboratory.stellar.org/account/create?network=testnet)

### Run Locally

No build tools or npm required. It's a single HTML file.

```bash
# 1. Clone the repository
git clone https://github.com/thesnehasingh/Risein-Stellar-mission

# 2. Open the file in your browser
cd stellar-mission-control
open index.html       # macOS
start index.html      # Windows
xdg-open index.html   # Linux
```

Or simply **double-click** `index.html` in your file explorer.

### Live Demo


---

## 📸 Screenshots

### 1. Wallet Connected State
> Connect Freighter → the terminal boots and shows your address + QR code

![Wallet Connected](screenshots/wallet-connected.png)

### 2. Balance Displayed
> Live XLM balance fetched from Horizon API, with USD conversion

![Balance Display](screenshots/balance.png)

### 3. Successful Testnet Transaction
> Send XLM via Freighter — sign in the extension popup, submit to testnet

![Send Transaction](screenshots/send-tx.png)

### 4. Transaction Result Shown to User
> Confirmed transaction hash with direct link to StellarExpert explorer

![Transaction Result](screenshots/tx-result.png)

---

## 🏗️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML / CSS / JS | Frontend (no framework needed) |
| [Stellar SDK v11](https://github.com/stellar/js-stellar-sdk) | Build & submit transactions |
| [Freighter API v5](https://freighter.app) | Wallet connection & transaction signing |
| [QRCode.js](https://github.com/davidshimjs/qrcodejs) | QR code generation |
| [Stellar Horizon API](https://horizon-testnet.stellar.org) | Balance, operations, network stats |
| [Coingecko API](https://coingecko.com) | Live XLM/USD price |

---

## 🔐 Security

- **Your private key never touches this app.** All signing is handled by the Freighter extension.
- No backend server. No database. Fully client-side.
- Enforces Testnet — rejects connection if Freighter is on Mainnet.

---

## 📁 Project Structure

```
stellar-mission-control/
├── index.html      # The entire dApp (single file)
└── README.md       # This file
```

---

## 🎯 White Belt Checklist

- [x] Freighter wallet setup & integration
- [x] Stellar Testnet
- [x] Wallet connect functionality
- [x] Wallet disconnect functionality
- [x] Fetch connected wallet's XLM balance
- [x] Display balance clearly in the UI
- [x] Send XLM transaction on testnet
- [x] Show success / failure state to user
- [x] Display transaction hash / confirmation
- [x] Public GitHub repository
- [x] README with description, setup, screenshots

---

## 👤 Author

Built for the **Rise In — Stellar Journey to Mastery** program, July 2026 Challenge.

---

## 📄 License

MIT — free to use, study, and modify.
