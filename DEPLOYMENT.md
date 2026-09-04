# YatraAI Deployment Guide

This document provides step-by-step instructions to deploy YatraAI to the public internet.

---

## 🚀 Quick Deploy (5 Minutes) - Vercel Recommended

### Prerequisites
- GitHub account
- Vercel account (free at vercel.com)
- Project already pushed to GitHub

### Steps:

#### 1. Push Code to GitHub (if not already done)
```bash
git add .
git commit -m "Production ready YatraAI"
git push origin main
```

#### 2. Deploy to Vercel
1. Visit [vercel.com](https://vercel.com)
2. Click **"New Project"**
3. Click **"Import Git Repository"**
4. Paste: `https://github.com/sarthaklagad1294-art/yatra-ai`
5. Click **"Import"**
6. Vercel auto-detects configuration (Vite + React)
7. Click **"Deploy"**

**⏱️ Deployment takes 1-2 minutes**

#### 3. Get Your Public URL
After deployment completes:
- Vercel shows: `https://yatra-ai.vercel.app`
- This is your **public shareable link** 🎉

#### 4. Auto-Deploy on Future Updates
Every time you push to GitHub `main` branch:
- Vercel automatically rebuilds and deploys
- Your public link stays the same

---

## 📱 Complete Step-by-Step for Beginners

### Step 1: Prepare Your Project

```bash
# Navigate to project folder
cd yatra-ai

# Make sure everything is up to date
npm install

# Test locally
npm run dev
```

### Step 2: Push to GitHub

```bash
# Initialize git (if not done)
git init

# Add all files
git add .

# Create first commit
git commit -m "Initial commit: YatraAI production ready"

# Add GitHub remote
git remote add origin https://github.com/sarthaklagad1294-art/yatra-ai.git

# Set main branch
git branch -M main

# Push to GitHub
git push -u origin main
```

**Verify**: Visit https://github.com/sarthaklagad1294-art/yatra-ai and confirm all files are there

### Step 3: Connect Vercel

1. Create free Vercel account at https://vercel.com/signup
2. Click **"Continue with GitHub"**
3. Authorize GitHub access
4. You're logged in! Now:
5. Click **"New Project"** (top right)
6. Click **"Import Git Repository"**
7. In search box, type: `yatra-ai`
8. Select: `sarthaklagad1294-art/yatra-ai`
9. Click **"Import"**

### Step 4: Configure Deployment

Vercel auto-detects everything, but verify:

- **Framework**: Vite ✓
- **Build Command**: `npm run build` ✓
- **Output Directory**: `dist` ✓
- **Environment Variables**: (Leave empty) ✓

Click **"Deploy"**

### Step 5: Wait for Deployment

You'll see:
```
Building...
✓ Build complete
✓ Deployment complete
```

### Step 6: Get Your Public Link

After "Deployment complete", you see:
```
🎉 Congratulations!
Your site is live at: https://yatra-ai.vercel.app
```

**Share this link with anyone!** They can access your app instantly.

---

## 🔄 Make Updates Later

After deployment, to update your app:

```bash
# Make changes locally
# Test: npm run dev

# Commit and push
git add .
git commit -m "Fixed bug / Added feature"
git push origin main
```

**Vercel automatically deploys** - your public link stays the same! ✨

---

## 🌍 Alternative Hosting Options

### Option A: GitHub Pages (Free)

```bash
# Install gh-pages
npm install --save-dev gh-pages

# Update vite.config.js
# export default {
#   base: '/yatra-ai/',
#   ...
# }

# Deploy
npm run build
npx gh-pages -d dist
```

Access at: `https://sarthaklagad1294-art.github.io/yatra-ai`

### Option B: Netlify (Free)

1. Go to [netlify.com](https://netlify.com)
2. Click "Add new site"
3. "Import an existing project"
4. Connect GitHub → Select `yatra-ai`
5. Build: `npm run build` | Publish: `dist`
6. Deploy!

Access at: `https://yatra-ai.netlify.app`

### Option C: Firebase Hosting (Free)

```bash
npm install -g firebase-tools
firebase login
firebase init hosting
npm run build
firebase deploy
```

---

## 🐛 Troubleshooting

| Problem | Solution |
|---------|----------|
| "Build failed" | Check Node.js version: `node --version` (needs 20.19.0+) |
| "Cannot find module" | Run `npm install` before pushing |
| "Blank page deployed" | Check `vite.config.js` → `base` setting |
| "404 on page refresh" | Vercel rewrite rules are set ✓ |

---

## ✅ Deployment Checklist

- [x] All files pushed to GitHub
- [x] `package.json` has correct version
- [x] `README.md` is complete
- [x] `.gitignore` has sensitive files
- [x] No API keys in code
- [x] `vite.config.js` optimized
- [x] `vercel.json` configured
- [x] `index.html` has meta tags
- [x] Responsive design tested
- [x] Linting passes: `npm run lint`
- [x] Build succeeds: `npm run build`

---

## 🎯 Your Public URL

Once deployed, share this link:

```
https://yatra-ai.vercel.app
```

Anyone with this link can:
- ✓ Use your app instantly
- ✓ No installation needed
- ✓ Works on mobile, tablet, desktop
- ✓ Lightning fast (global CDN)

---

## 📞 Need Help?

- Vercel Docs: https://vercel.com/docs
- Vite Docs: https://vitejs.dev
- React Docs: https://react.dev
- GitHub Issues: Create one on your repo

---

**Deployment Status**: 🟢 Ready for Production

Last Updated: September 4, 2026
