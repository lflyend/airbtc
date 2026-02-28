# AirBTC — Offline Bitcoin Signer

AirBTC is a fully offline Bitcoin key generation and transaction signing tool that runs entirely in your browser.  
The entire application is contained in a single HTML file (`index.html`) and can be downloaded and run locally without any network connection.

---

## 🔐 Core Purpose

AirBTC is designed for one purpose only:

- Generate Bitcoin private keys offline
- Derive public keys and addresses
- Sign Bitcoin transactions locally
- Produce raw transaction HEX (`txHex`) ready for broadcast

All operations occur entirely within the browser, allowing **air-gapped usage**.

---

## 🛡 Security Model

AirBTC follows a strict offline-first architecture:

- Entirely client-side
- No remote code
- No external dependencies or CDNs
- No analytics or tracking
- No network requests
- No data collection or storage outside the browser

Users can **download `index.html` and run it offline** safely on any computer, even on an air-gapped device.

---

## 💻 Usage

1. Download the single file `index.html`.
2. Open it in any modern browser.
3. Generate private keys and Bitcoin addresses offline.
4. Create and sign transactions entirely locally.
5. Copy the generated `txHex` and broadcast using your preferred tool.

All cryptographic operations are performed locally. **Your keys never leave your device.**

---

## 📦 Architecture

The Chrome Extension version uses a minimal MV3 structure:

- `index.html` — Entire app and cryptographic logic
- `background.js` — Minimal service worker
- `manifest.json` — Chrome extension config
- `icons/` — Optional extension icons

No build tools or external dependencies are required. The single HTML file is fully portable.

---

## 🌐 Offline / Air-gapped Usage

AirBTC is ideal for:

- Fully offline key generation
- Signing transactions on air-gapped devices
- Safe handling of private keys without exposing them to the network

Simply open the HTML file in a browser without internet to operate completely offline.

---

## 📄 Privacy

AirBTC does not:

- Collect user data
- Track user activity
- Transmit keys or transactions externally

See `privacy.html` for the official privacy statement.

---

## 📌 Official Distribution

Official version is distributed via the Chrome Web Store.  
Users may also download the single HTML file directly for offline usage.

Verify source code before running modified versions.

---

## 📜 License

MIT License