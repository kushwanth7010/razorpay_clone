# Razorpay-Inspired Landing Page (Portfolio Clone)

A **static, educational front-end recreation** of a payment-platform landing page built with HTML, Tailwind CSS 4, and Vite 7. It does not process payments, access Razorpay APIs, collect real payment credentials, or represent an official Razorpay product.

**Repository:** https://github.com/kushwanth7010/razorpay_clone

**GitHub Pages URL:** https://kushwanth7010.github.io/razorpay_clone/

## Implemented features

- Responsive landing-page layout, navigation, product sections, and branded illustrations.
- Utility-based styling using Tailwind CSS 4.
- Vite development server and optimized static production build.
- Automated build and GitHub Pages deployment through GitHub Actions.

**Implementation note:** The present page is authored in `index.html` and styled with Tailwind. React packages are installed in `package.json` but the page is **not implemented with React components**. Several demonstration links (`#`) are placeholders, not working payment or account flows.

## Run locally

Use Node.js **22.12+** (or another version supported by Vite 7), npm, and Git.

```bash
git clone https://github.com/kushwanth7010/razorpay_clone.git
cd razorpay_clone
npm ci
npm run dev
```

Open the URL printed by Vite (usually http://localhost:5173).

Build and preview the deployable site:

```bash
npm run build
npm run preview
```

The build is written to `dist/`. The Vite base path is `/razorpay_clone/` so local development and GitHub Pages subpath assets resolve correctly.

## Deployment and verification

Pushing to `main` triggers `.github/workflows/deploy.yml`. It installs dependencies with `npm ci`, builds the site, uploads `dist/`, and deploys to GitHub Pages. Configure **Settings → Pages → Build and deployment → GitHub Actions** in the repository.

Follow progress at https://github.com/kushwanth7010/razorpay_clone/actions. A passing build proves the site compiled and the deployment step succeeded; browser layout and placeholder links need separate manual checks.

## Project structure

```text
index.html                    Static page markup
style.css                     Tailwind theme and styles
images/                       Local page illustrations and icons
package.json                  Build scripts and dependencies
package-lock.json             Reproducible npm dependency lockfile
vite.config.js                Tailwind plugin and GitHub Pages base
.github/workflows/deploy.yml  Automated build and deployment
```

## Attribution

This is an independent educational UI clone. Razorpay's name and referenced branding belong to their respective owners. No affiliation, payment processing, or commercial functionality is implied.
