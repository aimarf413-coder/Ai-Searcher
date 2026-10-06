# 🌌 Shary's Private Searcher (v2.0)

> Ultra-sleek Galactic Liquid Glass Private Searcher & Cloaked Browser powered by **Ultraviolet**, **BareMux**, and **Epoxy Wisp**.

Made by **Edgarr (w antigravity) :>**

---

## ✨ Features

- **Liquid Glass & Galactic Flow UI**: Refractive glass panels (inspired by ColorOS 16 / iOS / Google Pixel) with smooth spring transitions and an animated living cosmic canvas.
- **100% In-Frame Cloak**: Launches seamlessly into `about:blank` with zero URL history leakage.
- **Ultraviolet Proxy Engine**: Intercepts requests, strips CSP / `X-Frame-Options`, and rewrites scripts, styles, and links so sites run completely inside the frame.
- **Full YouTube Support**: Direct access to `youtube.com` — watch videos, search, and browse without third-party clones or Error 150.
- **Integrated Tab System**: Open multiple tabs, switch between them, and close them with `×`. Links with `target="_blank"` stay inside the tab deck.
- **Tab Disguise (Cloaking)**: Change tab title & favicon to Google Docs, Google Drive, Canvas LMS, Student Portal, or Gmail.
- **Panic Emergency Key**: Instantly close the window with `Escape`, `` ` `` (backtick), or `F4`.
- **Wisp Relay Selector**: Pre-configured with fast public Wisp relays (*Mercury Workshop*, *Anura*) with an option to plug in your own private `wss://` relay.

---

## 🚀 How to Run Locally

You can run the built-in server with zero external dependencies:

```bash
npm start
# or
node server.js
```

Open [http://localhost:8080](http://localhost:8080) in your browser.

---

## 🌐 Recommended Free Hosting Services

Because this project uses static client-side Service Workers connecting to WebSocket Wisp relays, you can host it completely for free on several popular platforms:

### 1. Vercel (Recommended — Fastest Setup)
- **Why**: Free SSL, global edge CDN, and zero configuration needed. `vercel.json` is already included with the proper `Service-Worker-Allowed` headers.
- **Steps**:
  1. Push this folder to a GitHub repository.
  2. Go to [vercel.com](https://vercel.com) and click **"Add New Project"**.
  3. Import your GitHub repository and click **Deploy**.
  4. Your site is live on `https://your-project.vercel.app`!

### 2. Netlify
- **Why**: Great free tier with automatic HTTPS and instant drag-and-drop deploy.
- **Steps**:
  1. Go to [netlify.com](https://www.netlify.com).
  2. Go to **Sites** -> Drag & drop this project folder into the Netlify upload zone.
  3. Your site deploys in seconds.

### 3. Cloudflare Pages
- **Why**: Unlimited bandwidth and ultra-fast edge network.
- **Steps**:
  1. Push code to GitHub / GitLab.
  2. Go to the Cloudflare dashboard -> **Workers & Pages** -> **Create application** -> **Pages**.
  3. Connect your repository and deploy.

### 4. Render / Railway / Koyeb
- **Why**: Full Node.js runtime hosting if you prefer running `server.js` directly as a Web Service.
- **Steps**:
  1. Create a free **Web Service** on Render or Railway.
  2. Set the build command to `npm install` and start command to `node server.js`.
