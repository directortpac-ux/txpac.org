# Texas Public Ambulance Corps (TPAC) — Official Website

The official website for **Texas Public Ambulance Corps (TPAC)**, a 501(c)(3) nonprofit ambulance service and Mobile Integrated Health system dedicated to expanding access to quality, patient-centered care in rural Central Texas.

**Live site:** [txpac.org](https://txpac.org)

## Project Structure

```
├── index.html      # Complete single-page website (all CSS/JS inline)
├── TPAC_Logo.png   # Organization logo (add manually)
├── CNAME           # Custom domain configuration for GitHub Pages
└── README.md       # This file
```

## Deploying on GitHub Pages

1. **Create a GitHub repository** (e.g., `txpac-website` or `txpac.org`)
2. **Push this project** to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: TPAC website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```
3. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Navigate to **Settings** > **Pages**
   - Under **Source**, select **Deploy from a branch**
   - Choose the `main` branch and `/ (root)` folder
   - Click **Save**
4. Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO/` within a few minutes.

## Setting Up a Custom Domain (txpac.org)

1. **Configure DNS** with your domain registrar. Add the following **A records** pointing to GitHub Pages:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
2. Optionally, add a **CNAME record** for the `www` subdomain:
   ```
   www  →  YOUR_USERNAME.github.io
   ```
3. The `CNAME` file in this repository is already configured with `txpac.org`.
4. In your GitHub repository, go to **Settings** > **Pages** > **Custom domain**, enter `txpac.org`, and click **Save**.
5. Check **Enforce HTTPS** once DNS propagation is complete (may take up to 24 hours).

## Adding the Logo

Place your `TPAC_Logo.png` file in the root of this repository alongside `index.html`. The website references it as `TPAC_Logo.png`.

## Technologies

- Single-page HTML with inline CSS and JavaScript
- Google Fonts (Merriweather, Source Sans 3)
- Responsive design (breakpoints at 1024px and 768px)
- Scroll-triggered animations via IntersectionObserver
- Zeffy donation form integration
- All icons are inline SVGs — no external dependencies

## License

Copyright 2026 Texas Public Ambulance Corps. All rights reserved.
