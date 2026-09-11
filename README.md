# MADAR MVP

MADAR is a World Intelligence MVP built with Next.js + TypeScript.

## 1. What you need

- A GitHub account
- A Vercel account
- Node.js installed if you want to run the project locally

No paid domain, server, or database is required for this first demo.

## 2. Run MADAR on your computer

Open a terminal in this folder:

```bash
npm install
npm run dev
```

Then open:

`http://localhost:3000`

The Iraq demo page is:

`http://localhost:3000/iraq`

For a production-style local test:

```bash
npm run build
npm run start
```

## 3. Put MADAR on GitHub

1. Sign in to GitHub.
2. Create a new repository named `madar-mvp`.
3. Keep it private or public; either works for this experiment.
4. Upload the contents of this folder to the repository.
5. Make sure `package.json` is in the repository root.

You can also use Git from the terminal:

```bash
git init
git add .
git commit -m "Initial MADAR MVP"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/madar-mvp.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username.

## 4. Deploy on Vercel — easiest method

1. Open Vercel and sign in with GitHub.
2. Choose **Add New Project**.
3. Select the `madar-mvp` GitHub repository.
4. Vercel should detect **Next.js** automatically.
5. Keep the default settings.
6. Click **Deploy**.
7. Wait for the build to finish.
8. Vercel will give you a free `*.vercel.app` deployment URL.

For this MVP, you do not need to buy a domain or configure a server.

## 5. Important Vercel settings

Recommended values if Vercel asks:

- Framework Preset: `Next.js`
- Root Directory: `.`
- Install Command: `npm install`
- Build Command: `npm run build`
- Output Directory: leave the Vercel default
- Node.js Version: use the current Vercel-supported default

Vercel automatically detects Next.js and normally handles the build configuration for you.

## 6. Environment variables

There are no environment variables required by the current demo.

Later, when we add APIs or a database, secrets should be added in:

**Vercel → Project → Settings → Environment Variables**

Do NOT put passwords, database credentials, private API keys, or secret tokens in the GitHub repository.

For browser-visible variables in Next.js, only variables deliberately prefixed with `NEXT_PUBLIC_` are exposed to the client.

## 7. Updating the live website

After connecting GitHub to Vercel:

```bash
git add .
git commit -m "Update MADAR"
git push
```

A new deployment is automatically created from the push.

## 8. Current MVP pages

- `/` — MADAR home
- `/iraq` — Iraq country profile using demo data

## 9. Current limitations

The current numbers and events are DEMO DATA. They are not presented as verified real-world statistics.

The next engineering stage is:

1. PostgreSQL/Supabase database
2. Real country/entity records
3. Source records
4. Search API
5. Relationship graph
6. Real data ingestion
7. Authentication and user watchlists

## Official deployment references

Vercel's current Next.js deployment flow is documented in its official Next.js guide:
https://vercel.com/docs/frameworks/full-stack/nextjs

Next.js deployment documentation:
https://nextjs.org/docs/app/getting-started/deploying
