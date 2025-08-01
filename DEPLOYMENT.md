# Deployment Guide - Valheim Projects Website

## Render Deployment

This website is configured for easy deployment on Render. The `render.yaml` file is already included.

### Steps to Deploy:

1. **Push to GitHub**: Upload your website files to a GitHub repository
2. **Connect to Render**: 
   - Go to [render.com](https://render.com)
   - Click "New +" and select "Static Site"
   - Connect your GitHub repository
3. **Configure**:
   - **Name**: `valheim-projects` (or your preferred name)
   - **Build Command**: Leave empty (no build required)
   - **Publish Directory**: `.` (root directory)
4. **Deploy**: Click "Create Static Site"

### Alternative Deployment Options:

#### Netlify
1. Drag and drop your website folder to [netlify.com](https://netlify.com)
2. Or connect your GitHub repository

#### Vercel
1. Go to [vercel.com](https://vercel.com)
2. Import your GitHub repository
3. Deploy automatically

#### Traditional Web Hosting
1. Upload all files to your web hosting provider
2. Ensure `index.html` is in the root directory

## File Structure Required:
```
valheim-projects-website/
├── index.html
├── styles.css
├── script.js
├── logo.png
├── selfie.png
├── staircase.jpeg
├── gate installation.jpg
├── outside gate.png
├── club-sign.jpeg
├── Landing Page Valheim.png
├── render.yaml
└── README.md
```

## Important Notes:
- All image files must be in the same directory as `index.html`
- The website is static and doesn't require a server
- No build process is needed
- Works with any standard web hosting service 