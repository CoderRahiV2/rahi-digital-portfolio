# Rahi Digital Portfolio — Netlify-only starter

This version uses Netlify Functions and Netlify Blobs instead of Firebase/Supabase. It includes a public portfolio and password-protected dashboard for adding/deleting entries and uploading images/videos up to 50 MB via chunked uploads.

## Deployment requirement
This project contains server-side functions and dependencies. **Netlify Drop/manual static upload will not deploy the backend.** Connect this folder/repository to Netlify through Git or use Netlify CLI so dependencies and functions are built.

## Setup
1. Deploy this folder using a Git-connected Netlify site; base directory is the folder containing `package.json` and `netlify.toml`.
2. In Netlify Project configuration → Environment variables, add `ADMIN_PASSWORD` (strong unique password) and `SESSION_SECRET` (separate random secret, 32+ characters). Do not put either secret in code.
3. Redeploy after adding the variables.
4. Open `/admin.html` on your deployed site and sign in using `ADMIN_PASSWORD`.

## Limits and notes
Netlify plan/credit limits apply to Functions, Blobs storage and bandwidth; this is not unlimited free hosting. Publicly uploaded media is public portfolio content. Test login, uploads, playback and deletion after deployment. This starter supports add/delete, not editing existing items.
