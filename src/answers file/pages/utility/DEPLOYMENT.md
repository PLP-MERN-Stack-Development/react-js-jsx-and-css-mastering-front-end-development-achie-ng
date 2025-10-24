# Deployment Guide

This guide will help you deploy your React application to various platforms.

## 🌐 Deployment Options

### 1. Vercel (Recommended)

Vercel is the easiest way to deploy React applications with zero configuration.

#### Method A: GitHub Integration (Recommended)

1. **Push your code to GitHub**
```bash
git add .
git commit -m "Ready for deployment"
git push origin main
```

2. **Visit Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Sign up with your GitHub account
   - Click "New Project"
   - Import your repository
   - Vercel will auto-detect Vite and configure build settings
   - Click "Deploy"

3. **Configuration** (Usually auto-detected)
   - Build Command: `npm run build`
   - Output Directory: `dist`
   - Install Command: `npm install`

#### Method B: Vercel CLI

```bash
# Install Vercel CLI
npm i -g vercel

# Login
vercel login

# Deploy
vercel

# Deploy to production
vercel --prod
```

### 2. Netlify

Netlify offers great features for static sites.

#### Method A: Drag and Drop

1. Build your project:
```bash
npm run build
```

2. Visit [netlify.com](https://netlify.com)
3. Drag and drop the `dist` folder to the Netlify dashboard

#### Method B: GitHub Integration

1. Push code to GitHub
2. Go to Netlify dashboard
3. Click "New site from Git"
4. Connect to GitHub and select repository
5. Configure build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
6. Click "Deploy site"

#### Method C: Netlify CLI

```bash
# Install Netlify CLI
npm install -g netlify-cli

# Login
netlify login

# Initialize
netlify init

# Deploy
netlify deploy --prod
```

### 3. GitHub Pages

Good for simple hosting directly from GitHub.

#### Setup

1. **Install gh-pages**
```bash
npm install --save-dev gh-pages
```

2. **Update package.json**
```json
{
  "homepage": "https://yourusername.github.io/repository-name",
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d dist"
  }
}
```

3. **Update vite.config.js**
```