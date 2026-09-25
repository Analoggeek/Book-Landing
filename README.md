# 📘 Master Book of Ethical Hacking & Cybersecurity: Landing Page

A high-conversion sales page for **Master Book of Ethical Hacking & Cybersecurity, 2nd Edition (v2.0)** by **Analog Geek**.

- ✅ One file (`index.html`) with no build step and no outside libraries or fonts
- ✅ Works with GitHub Pages as it is (includes `.nojekyll`)
- ✅ Fully responsive, with a CSS-only 3D book cover
- ✅ Conversion features: countdown timer, sticky mobile CTA, price anchoring, comparison table, FAQ, exit-intent coupon, and an optional real-buyer toast

## 🚀 Deploy on GitHub Pages (2 minutes)
1. Create a new repo on GitHub (for example `ethical-hacking-book`).
2. Upload everything in this folder (`index.html`, `assets/`, `.nojekyll`, `README.md`).
3. Go to **Settings → Pages → Source: Deploy from a branch → `main` / root → Save**.
4. Your site will be live at `https://<username>.github.io/ethical-hacking-book/`.

Or use git:
```bash
git init && git add . && git commit -m "Landing page"
git branch -M main
git remote add origin https://github.com/<username>/ethical-hacking-book.git
git push -u origin main
```

## ⚙️ Customize (open `index.html` and find `const CONFIG`)
| Key | What it does |
|---|---|
| `price` / `mrp` | Selling price (currently ₹499) and original price (the discount % is calculated for you) |
| `buyUrl` | Payment link (currently `https://rzp.io/rzp/g8qXx8E`). Every Buy / Get Book button uses it |
| `contactUrl` | WhatsApp link, for example `https://wa.me/91XXXXXXXXXX` |
| `offerHours` | Countdown length for each visitor |
| `stockClaimed` / `stockTotal` | Real sales count (keep `0` to hide the bar) |
| `coupon` | Exit-intent popup code (keep `""` to turn it off) |
| `recentBuyers` | Real recent buyers for the social-proof toast (keep `[]` to turn it off) |

> Tip: Please only use real sales numbers, buyers and reviews. Fake social proof hurts trust, and it can break consumer-protection rules.

## 📁 Structure
```
index.html        # the entire page (HTML + CSS + JS)
assets/favicon.svg
.nojekyll         # tells GitHub Pages to serve the files as they are
```

## 🔁 Auto-redirect after payment (Razorpay)
The page tells buyers they'll be redirected to the book automatically. To make that happen:
Razorpay Dashboard → **Payment Pages / Payment Links** → open this link → **Settings → "Redirect to URL after successful payment"** → paste your book's download link (Google Drive, etc.) → Save.
