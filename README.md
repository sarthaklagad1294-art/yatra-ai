# YatraAI — Smart AI Travel Companion & Decision Assistant

![YatraAI](https://img.shields.io/badge/Status-Active-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue) ![React](https://img.shields.io/badge/React-19.2.8-blue) ![Vite](https://img.shields.io/badge/Vite-8.2.0-purple)

## 🌍 Project Description

**YatraAI** is an intelligent travel companion web application that helps users make better travel decisions. While Google Maps shows you the route, YatraAI helps you decide the journey by providing comprehensive travel insights.

### Core Features:
- 🚌 **Transport Options Comparison**: Compare multiple transportation methods (bus, train, taxi, flight) with detailed cost and time analysis
- ⏱️ **Step-by-Step Public Transit Timelines**: Real-time public transportation schedules and detailed transit information
- 🍽️ **Local Food Recommendations**: Discover authentic local cuisine and dining options at your destination
- 💰 **Budget Breakdowns**: Detailed cost analysis for your entire trip including transport, accommodation, and food
- 🤖 **AI-Powered Itineraries**: Get personalized travel itineraries powered by artificial intelligence
- 🗺️ **Interactive Maps**: Explore destinations with interactive Leaflet-based maps
- 📱 **Fully Responsive**: Works seamlessly on mobile, tablet, and desktop devices

## 🚀 Technologies Used

### Frontend Framework
- **React** (v19.2.8) - Modern UI library
- **React DOM** (v19.2.8) - DOM rendering

### Build Tool & Development
- **Vite** (v8.2.0) - Lightning-fast build tool
- **@vitejs/plugin-react** (v6.0.4) - React plugin for Vite

### UI & Icons
- **Lucide React** (v1.16.0) - Beautiful, consistent SVG icon library

### Maps & Location
- **Leaflet** (v1.9.4) - Open-source mapping library

### Code Quality
- **Oxlint** (v1.75.0) - Fast JavaScript linter
- **@types/react** (v19.2.17) - TypeScript definitions for React
- **@types/react-dom** (v19.2.3) - TypeScript definitions for React DOM

### Deployment
- **Vercel** - Serverless deployment platform
- **GitHub Pages** - Static site hosting
- **Capacitor** - Mobile app framework (iOS/Android)

## 📋 Project Structure

```
yatra-ai/
├── src/                    # Source code
│   ├── components/        # React components
│   ├── pages/            # Page components
│   ├── hooks/            # Custom React hooks
│   ├── styles/           # CSS/styling
│   ├── utils/            # Utility functions
│   ├── App.jsx          # Main App component
│   └── main.jsx         # Entry point
├── public/               # Static assets
│   └── favicon.svg      # App favicon
├── dist/                 # Production build (auto-generated)
├── vite.config.js       # Vite configuration
├── vercel.json          # Vercel deployment config
├── capacitor.config.json # Capacitor mobile config
├── .oxlintrc.json       # Oxlint configuration
├── .gitignore           # Git ignore rules
├── index.html           # HTML entry point
├── package.json         # Dependencies and scripts
├── package-lock.json    # Locked dependency versions
└── README.md            # This file
```

## 🛠️ How to Run Locally

### Prerequisites
- **Node.js** (v20.19.0 or v22.12.0 or higher)
- **npm** (v10.0.0 or higher) or **yarn**
- **Git**

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/sarthaklagad1294-art/yatra-ai.git
   cd yatra-ai
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run development server**
   ```bash
   npm run dev
   ```
   The application will start at `http://localhost:5173`

4. **Build for production**
   ```bash
   npm run build
   ```
   This creates an optimized production build in the `dist/` folder

5. **Preview production build**
   ```bash
   npm run preview
   ```
   Preview the production build locally

6. **Run linting**
   ```bash
   npm run lint
   ```
   Check code quality with Oxlint

## 🌐 Deployment Guide

### Option 1: Deploy with Vercel (Recommended) ⭐

Vercel is the optimal choice for this project as it's optimized for React + Vite applications.

#### Steps:
1. **Push code to GitHub** (see section below)

2. **Connect to Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import your GitHub repository `sarthaklagad1294-art/yatra-ai`
   - Vercel auto-detects Vite configuration

3. **Configure Build Settings**
   - Build Command: `npm run build` ✓ (auto-detected)
   - Output Directory: `dist` ✓ (auto-detected)
   - Environment Variables: None required (unless adding API keys later)

4. **Deploy**
   - Click "Deploy"
   - Your app will be live at: `https://yatra-ai.vercel.app`

5. **Custom Domain** (Optional)
   - In Vercel Dashboard → Settings → Domains
   - Add your custom domain

**Auto-Deployment**: Every push to `main` branch automatically deploys to production.

---

### Option 2: Deploy with GitHub Pages

GitHub Pages hosts static sites for free directly from your repository.

#### Steps:
1. **Update `vite.config.js`**
   ```javascript
   export default {
     base: '/yatra-ai/',
     plugins: [react()],
   }
   ```

2. **Update `package.json` scripts**
   ```json
   "deploy": "npm run build && gh-pages -d dist"
   ```

3. **Install gh-pages**
   ```bash
   npm install --save-dev gh-pages
   ```

4. **Push code to GitHub**

5. **Deploy**
   ```bash
   npm run deploy
   ```

6. **Enable GitHub Pages**
   - Repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: `gh-pages` / `root`

7. **Access your site**
   - URL: `https://sarthaklagad1294-art.github.io/yatra-ai`

---

### Option 3: Deploy with Netlify

Alternative free hosting with excellent React support.

#### Steps:
1. **Push to GitHub** (same as above)

2. **Connect to Netlify**
   - Go to [netlify.com](https://netlify.com)
   - Click "Add new site" → "Import an existing project"
   - Connect GitHub account
   - Select `sarthaklagad1294-art/yatra-ai`

3. **Build Settings**
   - Build command: `npm run build`
   - Publish directory: `dist`

4. **Deploy**
   - Click "Deploy site"
   - Your site: `https://yatra-ai.netlify.app`

---

## 📤 Push Project to GitHub

### Step-by-Step Instructions:

#### Step 1: Initialize Git locally
```bash
cd yatra-ai
git init
git add .
git commit -m "Initial commit: YatraAI project setup"
```

#### Step 2: Add remote repository
```bash
git remote add origin https://github.com/sarthaklagad1294-art/yatra-ai.git
git branch -M main
```

#### Step 3: Push to GitHub
```bash
git push -u origin main
```

#### Step 4: Verify
- Visit: https://github.com/sarthaklagad1294-art/yatra-ai
- You should see all project files

---

## 📱 Responsive Design

The application is built to be fully responsive:

- **Mobile** (< 768px): Touch-optimized interface, stacked layout
- **Tablet** (768px - 1024px): Balanced two-column layout
- **Desktop** (> 1024px): Full multi-column layout with expanded features

All components use CSS media queries and flexible layouts (Flexbox/Grid) for optimal viewing on any device.

---

## 🔒 Security & Best Practices

✅ **No hardcoded credentials** - All sensitive data in environment variables  
✅ **Production builds optimized** - Minified and tree-shaken  
✅ **Linting configured** - Code quality checks with Oxlint  
✅ **Dependencies locked** - Exact versions in `package-lock.json`  
✅ **Git ignored** - Secrets, node_modules, build files excluded  

---

## 📝 Environment Variables

Currently, the project requires **no environment variables** for basic functionality.

**If adding external APIs in future:**

1. Create `.env.local` file (not committed to git)
2. Add variables:
   ```
   VITE_API_KEY=your_api_key_here
   VITE_MAP_TOKEN=your_token_here
   ```
3. Access in code: `import.meta.env.VITE_API_KEY`

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| `npm install` fails | Delete `node_modules` and `package-lock.json`, then reinstall |
| Port 5173 already in use | `npm run dev -- --port 3000` |
| Build fails | Check Node.js version: `node --version` (requires v20.19.0+) |
| Linting errors | Run `npm run lint` to see issues, fix manually or use auto-fix |

---

## 📞 Support & Contributions

- **Issues**: [GitHub Issues](https://github.com/sarthaklagad1294-art/yatra-ai/issues)
- **Discussions**: [GitHub Discussions](https://github.com/sarthaklagad1294-art/yatra-ai/discussions)
- **Contributing**: See [CONTRIBUTING.md](CONTRIBUTING.md)

---

## 📄 License

This project is licensed under the **MIT License** - see LICENSE file for details.

---

## 🙏 Acknowledgments

- Built with [React](https://react.dev)
- Powered by [Vite](https://vitejs.dev)
- Maps by [Leaflet](https://leafletjs.com)
- Icons from [Lucide React](https://lucide.dev)

---

## 🚀 Quick Links

| Link | Purpose |
|------|----------|
| [GitHub Repo](https://github.com/sarthaklagad1294-art/yatra-ai) | Source code |
| [Vercel Deployment](https://yatra-ai.vercel.app) | Live application |
| [Issues](https://github.com/sarthaklagad1294-art/yatra-ai/issues) | Bug reports |
| [Deployment Guide](DEPLOYMENT.md) | Step-by-step deployment |

---

**Made with ❤️ by YatraAI Team**

Last updated: September 4, 2026