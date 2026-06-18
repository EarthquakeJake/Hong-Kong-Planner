# 🇭🇰 Hong Kong Salary & Budget Planner

A single-page web app for planning Jake & Maria's move to Hong Kong: take-home pay
(HK salaries tax + MPF), household budgeting, job-offer comparison, and a Netherlands-vs-HK
"is the move worth it?" check. Dark neon-harbour theme, works on phone and desktop, and
saves your inputs automatically in the browser.

Everything runs in the browser — there is no server and no data leaves your device.

---

## Files

| File | What it is |
|------|------------|
| `index.html` | The whole app (HTML + CSS + JS in one file). This is all you need. |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is. |
| `icon.png` | *(optional)* Home-screen icon for iPhone. Add your own 180×180 PNG, or ignore. |
| `README.md` | This file. |

---

## Host it for free with GitHub Pages

### Option A — GitHub website (no tools needed)

1. Sign in at <https://github.com> and click **New repository**.
   - Name it e.g. `hk-planner`, set it **Public**, click **Create repository**.
2. On the new repo page click **uploading an existing file**.
3. Drag in **`index.html`** and **`.nojekyll`** (and `icon.png` if you made one), then **Commit changes**.
4. Go to **Settings → Pages**.
5. Under *Build and deployment → Source* choose **Deploy from a branch**,
   pick branch **`main`** and folder **`/ (root)`**, then **Save**.
6. Wait ~1 minute. Your public link appears at the top of the Pages screen:

   ```
   https://<your-username>.github.io/hk-planner/
   ```

That URL is shareable and works on any phone or computer.

### Option B — Git command line

```bash
cd hk-planner-site
git init
git add .
git commit -m "HK salary & budget planner"
git branch -M main
git remote add origin https://github.com/<your-username>/hk-planner.git
git push -u origin main
```

Then enable Pages as in steps 4–6 above.

---

## Use it on your iPhone

1. Open the published `github.io` link in **Safari**.
2. Tap the **Share** button → **Add to Home Screen**.
3. It launches full-screen like an app, with the dark theme in the status bar.

> **Note:** Your saved inputs live in that browser's local storage. They persist between
> visits on the same device/browser, but they are *per-device* — Jake's iPhone and Maria's
> iPhone keep separate copies. The **↺ Reset** button clears them.

*(Optional)* For a nicer home-screen icon, drop a 180×180 px PNG named `icon.png` into the
folder before uploading. Without it the phone just uses a screenshot — still works fine.

---

## Updating it later

Edit `index.html` (or replace it), commit/upload the new version, and GitHub Pages
republishes automatically within a minute.

---

## Disclaimer

All figures are **planning estimates, not tax advice**. Built on Hong Kong 2025/26
salaries-tax rules and MPF caps, and Netherlands 2026 box-1 rates. Verify with the IRD,
the Belastingdienst, and your employer before making decisions.
