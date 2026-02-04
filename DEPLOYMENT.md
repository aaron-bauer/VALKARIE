# Valentine's Proposal - Deployment Guide

## Quick Deploy to Render (Free)

### Step 1: Prepare Your Project
✅ Already done! You have:
- `requirements.txt` - Dependencies listed
- `render.yaml` - Render configuration
- `app.py` - Production-ready Flask app
- `index.html` - Frontend
- `proposal.js` - JavaScript logic

### Step 2: Push to GitHub
1. Go to https://github.com and create an account (if you don't have one)
2. Create a new repository named `valentines-proposal`
3. In PowerShell, navigate to your project folder and run:
```powershell
git init
git add .
git commit -m "Initial Valentine's proposal app"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/valentines-proposal.git
git push -u origin main
```

### Step 3: Deploy to Render
1. Go to https://render.com
2. Sign up with GitHub
3. Click "New +" and select "Web Service"
4. Connect your GitHub repository
5. Fill in the details:
   - Name: `valentines-proposal`
   - Start Command: `python app.py`
   - Plan: Free
6. Click "Create Web Service"
7. Wait 2-3 minutes for deployment
8. You'll get a URL like: `https://valentines-proposal.onrender.com`

### Step 4: Share Your Link
Send the URL to your special someone and they can open it on any device!

**Example:** `https://valentines-proposal.onrender.com`

### Notes:
- The free tier sleeps after 15 minutes of inactivity (takes 30 seconds to wake up)
- Responses are stored in JSON file during runtime
- Works perfectly on mobile browsers!

## Alternative Options
- **Railway.app** - Similar to Render, also free
- **PythonAnywhere** - Python-specific hosting
- **Replit** - Instant online coding/hosting

---
Good luck with your proposal! 💕
