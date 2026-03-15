# Setup Guide

## 1. GitHub

Create a new empty GitHub repository, then connect it locally:

```bash
git remote add origin git@github.com:YOUR_USERNAME/YOUR_REPO.git
git branch -M main
git add .
git commit -m "Initial Shopify store setup"
git push -u origin main
```

If you prefer HTTPS:

```bash
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git branch -M main
git add .
git commit -m "Initial Shopify store setup"
git push -u origin main
```

## 2. Shopify CLI

This repo already includes Shopify CLI as a local dev dependency. Authenticate with:

```bash
npx shopify auth login
```

Then connect or create a theme:

```bash
npm run dev
```

Or, if a theme already exists in the store:

```bash
npm run pull
npm run dev
```

## 3. Recommended starting work

- Build the homepage first
- Set up the main navigation
- Create starter collection templates
- Add product metafields for fabric, craft, and delivery timeline
