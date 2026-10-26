# Rahi Digital Portfolio — Netlify edition

## Deploy
This folder is the site root. If your GitHub repository contains it inside `rahman-rahi-portfolio/`, configure Netlify Base directory as `rahman-rahi-portfolio`, publish directory `.`, functions directory `netlify/functions`. Keep the repository connected to Netlify so functions and dependencies are built.

## Environment variables
In Netlify project configuration add `ADMIN_PASSWORD` (your private admin password) and `SESSION_SECRET` (a different random secret of 32+ characters). Redeploy after saving. Never commit these values to GitHub.

## Admin
Visit `/admin.html`, sign in using `ADMIN_PASSWORD`. Update profile/contact/social links/education/skills and add/edit/delete portfolio items. Images/videos are uploaded to Netlify Blobs; keep uploads under 50 MB and within your account's current usage limits.

## Notes
Data persists in Netlify Blobs. Free usage and storage/bandwidth limits can change; check your Netlify plan and usage dashboard.
