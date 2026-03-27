# Raghu R — Portfolio Website

A cyberpunk-themed personal portfolio site built with HTML/CSS/JS, connected to Firebase Realtime Database for feedback collection.

## 🗂 File Structure

```
raghu-portfolio/
├── index.html              # Main portfolio page
├── render.yaml             # Render static site config
├── .gitignore
├── README.md
│
├── # ── Images (add these from your local folder) ──
├── r.jpg
├── player.jpeg
├── digital.jpeg
├── INFO.jpeg
├── ITC.jpeg
├── RED.jpeg
├── xo.jpeg
│
└── .github/
    └── workflows/
        └── deploy.yml      # Manual GitHub Actions deploy workflow
```

## 🚀 Hosting on Render

1. Push this repo to GitHub
2. Go to [render.com](https://render.com) → New → Static Site
3. Connect repo, set publish directory to `.`, leave build command blank
4. Copy the **Deploy Hook URL** from Render Settings
5. Add it as a GitHub secret: `RENDER_DEPLOY_HOOK_URL`

## ▶️ How to Deploy Manually

1. Go to GitHub repo → **Actions** tab
2. Click **"Deploy to Render"**
3. Click **"Run workflow"** → enter optional reason → **Run**

## 🔥 Firebase

Feedback form posts to Firebase Realtime Database via REST API.
No SDK needed — configured directly in `index.html`.
