# Verify My Wallet

A small, beginner-friendly Web3 dApp that lets users **connect MetaMask**, **sign a message** (address + timestamp + nonce), and **verify** the signature — all in the browser (no gas, no smart contract required).

---

## 🔗 Live demo
[Open the live demo here](https://verify-my-wallet-mansigoles-projects.vercel.app/)

---

## 🧾 Features
- Connect MetaMask and detect account / network changes  
- Generate a unique message containing address, ISO timestamp, and nonce  
- Sign the message using `personal_sign` (MetaMask)  
- Recover the signer from the signature using `web3.eth.accounts.recover` and compare it to the connected wallet  
- Download a JSON proof `{ address, message, signature, downloadedAt }`  
- Works on Ethereum testnets (Sepolia) — no real ETH required

---

## ⚙️ How to use
1. Open the **Live demo** link or run `index.html` locally.  
2. Click **Connect Wallet** and allow MetaMask.  
3. Click **Sign Message** and approve the signature in MetaMask.  
4. Click **Verify Signature** — if the recovered address matches your connected account you will see **✔ Verified**, otherwise **✖ Not Verified**.  
5. (Optional) Switch MetaMask accounts to test the “Not Verified” scenario.  
6. Click **Download Proof** to save the signed payload as a JSON file.

---

## 🧩 Files
- `index.html` — single-file app (HTML / CSS / JS)  
- `screenshots/` — folder for example screenshots (add these manually)  
- `README.md` — this file

---

## 📸 Screenshots
Add screenshots to the `screenshots/` folder and reference them here:

```md
![Connect Wallet](screenshots/connect.png)
![Sign Message](screenshots/sign.png)
![Verified Result](screenshots/verify.png)

