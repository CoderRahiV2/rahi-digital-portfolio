# Rahi Digital Portfolio — Netlify edition

## Deploy
This folder is the site root. The repository currently places it inside `rahman-rahi-portfolio/`, so set Netlify Base directory to `rahman-rahi-portfolio`, Publish directory to `.`, and Functions directory to `netlify/functions`. Keep Git connected so Netlify builds the functions and dependencies.

## Environment variables
In Netlify project configuration add `ADMIN_PASSWORD` (your private admin password) and `SESSION_SECRET` (a different random secret of 32+ characters). Redeploy after saving. Never commit these values to GitHub.

## Admin
Visit `/admin.html` and sign in using `ADMIN_PASSWORD`. The dashboard manages your profile, introduction, About Me, contact details, education, skills, social links, profile picture, and portfolio items. Images/videos are stored in Netlify Blobs. Keep uploads under 50 MB and within your account's current usage limits.

## Persistent storage
Profile, portfolio records and uploaded media are saved in Netlify Blobs. Free usage, storage and bandwidth limits can change; check your Netlify plan and usage dashboard.
