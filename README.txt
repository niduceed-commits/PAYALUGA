PAYALUGA WEBSITE STARTER

1. Open config.js and replace YOUR_PROJECT_URL and YOUR_PUBLISHABLE_KEY with the values from Supabase > Project Settings > API / API Keys.
2. Do not put a service_role key, secret key, or database password in config.js.
3. Upload index.html and config.js to a static host (GitHub Pages or Netlify).
4. In Supabase > Authentication > URL Configuration, set the deployed website URL as Site URL and add it to Redirect URLs.
5. For live chat updates, run this optional SQL once:
   alter publication supabase_realtime add table public.chat_messages;
   If it says the table is already included, that is fine. The Refresh button works without Realtime.

Features: email/password registration and login, pending approval screen, admin approval/rejection, admin news posting, questions/answers, and group chat.

Safety: keep the community private; only invite approved students. Avoid collecting student phone numbers, home addresses, school IDs, or other unnecessary personal data. Have a trusted adult/community moderator oversee the group. This starter does not yet include report/block controls or a full moderation queue, so test carefully before inviting students.
