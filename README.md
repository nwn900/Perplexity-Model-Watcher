# 🔍 Perplexity Model Watcher (Firefox)

A Firefox extension that shows which model Perplexity is currently using by extracting the `display_model` and `user_selected_model` fields from Perplexity network responses.

- **Toolbar badge**
  - 🟢 OK when `display_model === user_selected_model`
  - 🔴 `!` when they differ (mismatch)
- **In-page overlay** (draggable + minimizable) that shows the two model values and a status chip
- **Privacy-first**: runs locally, collects nothing
- **Minimal permissions**: `storage`, `tabs`, and host access only for `https://*.perplexity.ai/*`

---

## ✨ Features

- 🎯 Real-time: watches fetch/XHR responses and extracts model fields
- 🖼️ Overlay: draggable/minimizable card with colored status chip
- 🟢/🔴 Badge: OK when display == user-selected; `!` on mismatch
- 🔐 Privacy-first: no data collection, all local
- ⚡ Minimal permissions: `storage`, `tabs`, host = `https://*.perplexity.ai/*`

---

## ✅ How to use

1. Install the extension (see **Install** below).
2. Open Perplexity in Firefox: `https://www.perplexity.ai/`
3. Run any query (the extension needs network traffic to detect model fields).
4. Check:
   - **Toolbar badge** for quick status (🟢 / 🔴 `!`)
   - **Overlay** for details (`display_model` and `user_selected_model`)

### Overlay toggle
Open the extension’s **Options** page to enable/disable the in-page overlay.

---

## 🚀 Install

### Option A: Install from GitHub Releases (recommended)
1. Go to **Releases** in this repo and download the latest `.xpi`.
2. In Firefox, open `about:addons`.
3. Click the ⚙️ (gear icon) → **Install Add-on From File…**
4. Select the downloaded `.xpi`.

> Note: Firefox generally requires signed extensions for permanent installation. If your build is unsigned, you may need a dev-focused Firefox build or a signed release package.

### Option B: Run from source (temporary, for development)
1. Clone the repo (or download ZIP and extract):
   ```bash
   git clone https://github.com/<your-user>/<your-repo>.git
   cd <your-repo>
