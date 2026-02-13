# Deploying sadbad.dev

## Current Status
The site is live temporarily at: https://eager-steaks-rest.loca.lt

## Deploy to Vercel (Manual Steps)

### Option 1: Via Vercel Dashboard
1. Go to https://vercel.com/new
2. Click "Add New Project"
3. Choose "Import Git Repository" or "Upload" (for local files)
4. Upload the `/home/claw/secure-openclaw/projects/sadbad-dev/` folder
5. No build configuration needed (it's a static HTML file)
6. Deploy!
7. Go to Project Settings > Domains > Add `sadbad.dev`

### Option 2: Via Vercel CLI (Needs Token)
```bash
cd /home/claw/secure-openclaw/projects/sadbad-dev
npx vercel deploy --prod --token YOUR_VERCEL_TOKEN
```

Get a token from: https://vercel.com/account/tokens

### Option 3: Via GitHub + Auto-Deploy
1. Push code to GitHub repo (e.g., sadbaddev/sadbaddev.github.io)
2. Connect repo to Vercel
3. Vercel will auto-deploy on push

## Files
- `index.html` - The complete single-page site
- No build step required
- No dependencies needed

## Domain Setup
After deploying, add the domain in Vercel:
1. Project Settings > Domains
2. Add: sadbad.dev
3. Configure DNS if needed (Vercel will guide you)
