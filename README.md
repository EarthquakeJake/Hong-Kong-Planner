# 🇭🇰 Hong Kong Salary & Budget Planner

A single-page web app for planning Jake & Maria's move to Hong Kong: take-home pay
(HK salaries tax + MPF), household budgeting, job-offer comparison, and a Netherlands-vs-HK
"is the move worth it?" check. Dark neon-harbour theme, works on phone and desktop, and
saves your inputs automatically in the browser.

Everything runs in the browser — there is no server and no data leaves your device.

## What's inside

| Tab | What it does |
|-----|--------------|
| 💼 **Salary & Tax** | Take-home pay per person or household: salaries tax (2025/26 or 2026/27 allowances), MPF, 13th month, bonus, housing allowance. |
| 💰 **Full picture** | The complete net picture from your final packages + rent, per person **and** combined, per month or per year: tax, MPF, rent, budgeted spending, hidden/annual costs → what is left to spend and save. Also shows the *monthly cash-flow reality* (HK has no tax withholding, 13th month/bonus arrive as lumps), a *first tax bill* timeline (final tax + provisional tax hit at once), the HK$100,000 domestic-rent deduction, and tips such as employer MPF and rental reimbursement schemes. |
| 🏮 **Budget** | Editable monthly budget and one-off relocation costs. Rent is linked to the Full picture tab. |
| ⚖️ **Offer Compare** | Two offers side by side, after tax & MPF. |
| 🇳🇱→🇭🇰 **Move check** | Dutch net vs Hong Kong net, with a cost-of-living adjustment. |

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

## Model notes

- **Spending vs savings:** budget lines marked 💰 are savings, everything else is spending. Every tab uses that one definition; one-off lines marked ↩ are refundable.
- **MPF** is calculated per monthly contribution period (so a bonus or 13th month can raise it), employer and employee separately. An employer pension above the mandatory 5% can be entered as a % of base.
- **Tax rules are versioned per year of assessment** (2025/26 incl. the one-off HK$3,000 reduction of final tax, 2026/27). The first-tax-bill estimate uses each year's own rules and never applies one-off reductions to provisional tax.
- **Household mode** assigns child/parent allowances and the rent deduction to whoever they save the most tax for (or as chosen), and Offer Compare runs each offer through the same household calculation.
- **Employer rent refund scheme** can be switched on (who, how much); it replaces the rent deduction.
- **NL estimate** uses the official 2026 brackets and credits, caps the 30% ruling, and taxes each earner separately.
- Budget figures from the estimator are rough placeholders, not verified prices. Eligibility for allowances and deductions is assumed, not checked.

All figures are **planning estimates, not tax advice**. Built on Hong Kong 2025/26 and
2026/27 salaries-tax rules, MPF caps and the domestic-rent deduction, and Netherlands 2026
box-1 rates. The hidden/annual cost lines are placeholders — replace them with your own. Verify with the IRD,
the Belastingdienst, and your employer before making decisions.
