HUSTLECONNECT SA — SUPABASE CONNECTED UPDATE

This bundle connects the existing PWA to your Supabase project.

FILES
- index.html (updated website)
- manifest.webmanifest
- sw.js (cache version updated)
- icon-192.png
- icon-512.png

INSTALL UPDATE ON GITHUB
1. Download and extract this ZIP on your phone.
2. Open your GitHub repository: https://github.com/kerrionbantom23-droid/Hustle-Connect---SA
3. Choose Add file > Upload files.
4. Upload the five individual files from the extracted folder to the repository root, replacing files with the same names. Do not upload the ZIP itself.
5. Commit the changes. Wait a few minutes, then open the GitHub Pages site in Chrome.
6. If your installed app still shows the old version, open the website in Chrome, refresh, close and reopen the app. If needed, remove the old home-screen app and install it again.

DATABASE BEHAVIOUR
- The website loads only rows where status = approved.
- New submissions are inserted with status = pending and are not shown publicly until approved.
- To approve a submission, open Supabase > Table Editor > listings, inspect the listing, and change status from pending to approved. Reject suspicious or false listings instead.
- Example cards are clearly marked as sample ideas, not verified vacancies.

SECURITY NOTES
- The browser contains a Supabase publishable key. That key is intended for public client apps, but Row Level Security must stay enabled and policies must remain restrictive. Never place a database password, sb_secret key, or service_role key in this website.
- Public submissions can attract spam. Review submissions before approval; before scaling, add authentication, abuse/rate limits, reporting, and a privacy policy. Do not collect unnecessary personal information.
- If submission fails, check Supabase API settings and table permissions/policies. The table must be public.listings and the columns must include id, title, category, location, contact, description, status, and created_at.
