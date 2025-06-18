
# SAVAGE_XMD WhatsApp Bot

This repository contains everything you need to deploy the SAVAGE_XMD WhatsApp bot using Render — no Termux required.

---

## Features
- ✅ Baileys-powered WhatsApp bot
- ✅ Pairing code (NOT QR code)
- ✅ Session API backend
- ✅ Session Scanner site (static)
- ✅ Ready for Render deployment
- ✅ Mobile-friendly

---

## Project Structure
```
SAVAGE_XMD_WITH_SESSION_API/
│
├── SAVAGE_XMD-main/         # Main bot source
├── scanner/                 # Session scanner website (static)
├── package.json             # Node dependencies
├── session-api.js           # Session API backend
├── session.html             # Web UI for scanning
├── whatsapp.js              # WhatsApp initialization file
└── README.md                # You're reading it :)
```

---

## Deployment Guide (No Termux Required)

### 🔵 Step 1: Upload to GitHub
1. Go to [GitHub](https://github.com)
2. Create a new repository named `SAVAGE_XMD`
3. Upload all files in this zip to the new repo.

---

### 🔵 Step 2: Deploy Session API Backend on Render
1. Go to [Render Dashboard](https://dashboard.render.com)
2. Click **New > Web Service**
3. Connect your GitHub repo
4. Select:
    - **Root directory**: This folder
    - **Build command**: `npm install`
    - **Start command**: `node session-api.js`
5. Deploy. Done!

---

### 🔵 Step 3: Deploy Session Scanner Website (Static Site)
1. From the same repo, create a **new static site** in Render.
2. Point the static site to `/scanner/` folder.
3. Render will build and host your session scanner site.

---

## Bonus: Art + Branding

![](./branding.jpg)

This project includes cool branding art. Feel free to customize.

---

## Created for:
**CKLAMZY / SAVAGE BOY** — the one and only 🛡️

> Powered by Baileys and Render, styled with 🔥.
