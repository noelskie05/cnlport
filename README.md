# Cristopher Noel Lopez — Portfolio

A self-contained, zero-build static portfolio site. Open `index.html` directly in any browser — no server, no npm, no build step required.

---

## 📂 Folder Structure (What to keep)

```
your-portfolio/
├── index.html          ← the whole site (this file)
└── images/             ← all your images (copy from client/public/images/)
    ├── me.png
    ├── hollow.png
    ├── velvet.png
    ├── gala.png
    ├── yuji.jpg
    ├── toji.jpg
    ├── tomie.jpg
    ├── heavenly.jpg
    ├── sukuna.jpg
    ├── apparel_1.jpg
    ├── apparel_2.jpg
    ├── apparel_3.jpg
    ├── apparel_4.jpg
    ├── lanyard_1.png
    ├── lanyard_2.png
    ├── dp_blast_1.png
    ├── dp_blast_2.png
    ├── join_dp.png
    ├── bsis_1.png
    ├── bsis_2.png
    ├── bsis_3.png
    ├── bsis_4.png
    └── grad.png
```

> **Important:** Copy your images from `Site-Revamp/client/public/images/` into a folder called `images/` next to `index.html`.

---

## 🖥️ Running Locally

Just double-click `index.html` — it opens in your browser with no setup needed.

If images don't load when opened as `file://`, start a simple local server:

```bash
# Python (built-in)
python -m http.server 8080

# Node (if installed)
npx serve .
```

Then open `http://localhost:8080` in your browser.

---

## 🚀 Deploy to GitHub Pages (Free Hosting)

1. **Create a new repository** on GitHub named `your-username.github.io` (this gives you a clean URL like `https://noelskie05.github.io`)
   - Or any repo name, e.g. `portfolio` → URL will be `https://noelskie05.github.io/portfolio/`

2. **Add your files:**
   ```bash
   git init
   git add index.html images/
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/your-username/your-repo.git
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repo → Settings → Pages
   - Source: **Deploy from a branch**
   - Branch: `main` / `/ (root)`
   - Click Save

4. Your site will be live in ~2 minutes at the URL shown in Settings → Pages.

---

## ✏️ Customizing

Everything is in `index.html` — search for these to update:

| What to change | Search for |
|---|---|
| Your name | `Cristopher Noel Lopez` |
| Social links | `href="#"` under "social-links" |
| Work experience dates | `AUG 2025`, `AUG 2024`, etc. |
| Live site URLs | `liveUrl:` in the `openModal(...)` calls |
| Hero stats | `data-target="20"` / `data-target="3"` |
| Profile photo | `images/me.png` |

---

## 📝 Notes

- No framework, no build tools, no Node.js needed
- Works offline once images are local
- Google Fonts loaded from CDN (requires internet on first load; browsers cache them)
- The contact form shows a confirmation but doesn't send email — to make it send, add [Formspree](https://formspree.io) or [EmailJS](https://emailjs.com)
