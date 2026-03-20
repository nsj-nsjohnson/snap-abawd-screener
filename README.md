# SNAP ABAWD Exemption Screener

A community-facing screening tool for Monroe County, NY residents to determine if they may be exempt from SNAP ABAWD (Able Bodied Adults Without Dependents) work requirements effective March 1, 2026.

## Policy Basis

- NYS OTDA SNAP Work Requirements
- One Big Beautiful Bill Act (H.R. 1) changes
- Monroe County Department of Social Services ABAWD guidance
- 12 exemption categories screened

## Deploy to Vercel

### Option 1: Deploy from GitHub (recommended)

1. Push this project to a GitHub repository
2. Go to [vercel.com](https://vercel.com) and sign in
3. Click **"Add New Project"**
4. Import your GitHub repository
5. Vercel will auto-detect the Vite framework. No configuration changes needed.
6. Click **Deploy**

### Option 2: Deploy via Vercel CLI

```bash
# Install Vercel CLI
npm i -g vercel

# From the project root directory
vercel

# Follow the prompts. Vercel will auto-detect Vite.
# For production deployment:
vercel --prod
```

## Local Development

```bash
npm install
npm run dev
```

Opens at `http://localhost:5173`

## Build

```bash
npm run build
```

Output goes to `dist/` directory.

## Project Structure

```
snap-screener/
├── index.html              # Entry point with meta tags
├── package.json            # Dependencies (React 18 + Vite 5)
├── vite.config.js          # Vite configuration
├── src/
│   ├── main.jsx            # React DOM mount
│   ├── App.jsx             # App wrapper
│   └── SNAPABAWDScreener.jsx  # Main screener component
└── README.md
```

## Notes

- No personal information is collected or stored
- This is a preliminary screening tool only
- MCDSS makes the final determination on ABAWD status and exemptions
- Links to Monroe County forms and NYS OTDA resources are included in results
