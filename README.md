# American90 🇺🇸

A free 90-day American English learning web app prototype. It includes:
- 90-day curriculum from foundations toward B1-style everyday communication
- American English vocabulary and usage
- daily lessons and quick checks
- XP, streaks, progress and achievements
- spaced-review area
- responsive desktop/mobile UI
- local demo account mode
- optional real multi-user authentication with Supabase

## Run on your Mac

1. Open Terminal.
2. `cd` into this folder.
3. Run a local server:

```bash
python3 -m http.server 3000
```

4. Open `http://localhost:3000`.

## Real accounts (free Supabase tier)

Create a free Supabase project, then replace these two values at the top of `index.html`:

```js
const SUPABASE_URL='YOUR_SUPABASE_URL';
const SUPABASE_ANON_KEY='YOUR_SUPABASE_ANON_KEY';
```

With real Supabase enabled, email/password authentication is used. For production, move progress data from localStorage into a `profiles`, `progress`, `lesson_results`, and `review_cards` schema with Row Level Security.

## Deploy for free

This is a static site and can be deployed on Vercel, Netlify or GitHub Pages. If you use Supabase, add the deployed site URL to Supabase Auth redirect settings.

## Product roadmap

For the next version, add real audio/TTS, a proper spaced-repetition scheduler, speaking recording, server-side progress, daily reminders, placement test, adaptive difficulty and a larger lesson/content database.
