# Suchitra Financial Services — Frontend

## Quick Start

```bash
# 1. Install dependencies
npm install

# 2. Start development server
npm start
# Opens at http://localhost:3000

# 3. Build for production (GoDaddy upload)
npm run build
# Creates build/ folder — upload contents to public_html on GoDaddy
```

## Connecting to Backend

Open `src/App.jsx` and find this line near the top:

```js
const API_BASE = "http://localhost:5000/api";
```

Change it to your live backend URL:
```js
const API_BASE = "https://suchitra-backend.onrender.com/api";
```

Then run `npm run build` again and re-upload to GoDaddy.

## GoDaddy Deployment Steps

1. Run `npm run build`
2. Login to GoDaddy → Hosting → cPanel → File Manager
3. Open `public_html` folder
4. Delete all existing files inside it
5. Upload all files from the `build/` folder
6. Done — your site is live!

## Pages Included
- Home
- Services (with apply form)
- EMI Calculator
- Eligibility Checker
- About
- Contact
- Admin Dashboard (🔐 password protected)
