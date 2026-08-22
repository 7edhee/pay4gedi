
# Pay4gedi

A brief description of what this project does and who it's for
# Google Pay Web UI Simulation

An interactive, dark-themed web simulation of the Google Pay user interface built with HTML5, CSS3, and JavaScript. This project demonstrates front-end mobile interface replication, camera stream integration, and real-time asynchronous event logging via Webhooks.

> ⚠️ **IMPORTANT DISCLAIMER: FOR EDUCATIONAL PURPOSES ONLY**
> 
> This repository is strictly created for **educational, instructional, and UI design research purposes**. 
> * **Prohibited Use:** This project must **NEVER** be used for phishing, social engineering, credentials harvesting, deception, or any fraudulent activity.
> * **No Real Transactions:** This simulation does not process real payments, connect to banking APIs, or interact with actual financial networks.
> * **Liability:** The author assumes no responsibility or liability for any misuse, illegal activity, or unethical deployment of this codebase. Users are solely responsible for ensuring compliance with applicable laws and security standards.

---

## 🌟 Features

* **PIN & Biometric Lock Screen:** Simulates an application unlock sequence with dynamic dot updates and error state handling.
* **Camera Scan Overlay:** Requests webcam permissions to display a real-time QR scanner view with targeting reticles.
* **Customizable Payment Form:** Input fields for recipient name, amount, UPI VPA ID, payment bank, and note.
* **Dynamic Payment Flow:** Includes simulated loading spinners, audio feedback, and a receipt generation screen displaying dynamic timestamps.
* **Discord Webhook Integration:** Sends structured payload alerts to a specified Discord channel when transaction steps are triggered.

---

## 🛠️ Tech Stack

| Component | Technology |
| :--- | :--- |
| **Front-End** | HTML5, Modern CSS3 (CSS Variables, Flexbox, Grid) |
| **Scripting** | Vanilla JavaScript (ES6+) |
| **Media APIs** | MediaDevices API (`getUserMedia`), Web Audio API |
| **Integrations** | Fetch API / Discord Webhooks |

---

## 🔒 Configuration Notes

* **Discord Webhook URL:** Update line 533 (`const DISCORD_WEBHOOK_URL = 'YOUR_DISCORD_WEBHOOK_URL_HERE';`) with your active webhook endpoint to receive transaction payloads.
* **Local Web Server Requirement:** Due to browser security restrictions on camera streams (`getUserMedia`) and CORS policies on outgoing background `fetch` requests, run this file on a local web server (e.g., VS Code **Live Server** extension) rather than directly via `file://`.
* **Default PIN:** The hardcoded PIN for unlocking the screen is set to `7070` on line 532 (`const CORRECT_PIN = '7070';`).
* **Audio Setup:** The payment confirmation audio requires the asset `Google pay sent transaction sound Gpay payment sound - tuff mp3 (128k).mp3` in the root folder, or an equivalent media file URL.

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
