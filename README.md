# BCR PLAY — Press Play and Feel Everything

Streaming app front-end for BCR Studios. One file. No build step. No dependencies.

## Deploy on GitHub + Render

1. Create a new GitHub repo (e.g. `bcr-play`).
2. Upload `index.html` (and this README) to the repo root and commit.
3. Go to [render.com](https://render.com) → **New → Static Site**.
4. Connect your GitHub repo.
5. Publish directory: `/` (root). Build command: leave empty.
6. Deploy — your app is live.

The app is a single self-contained `index.html` (all artwork embedded), so it also
works dropped on any static host or opened straight from disk.

## Upload section security

- **No passwords, tokens or credentials exist in this file or its code.**
- The owner creates a **personal password** at first run; the browser keeps only a
  one-way SHA-256 hash — the password itself is never stored, shown or sent anywhere.
- The **GitHub token** (the public sharing key, created when your repo is connected)
  lives in the browser session only. It is never written to disk, logs or exports,
  and is displayed only masked.
- Wrong password? The gate refuses generically and reveals nothing.

> Note: this is app-level UI locking. When you grow past a static site, add
> server-side authentication for full production security.

## Two keys

| Key | What it does |
| --- | --- |
| Personal password | Unlocks the Upload section (next to the Home button) |
| GitHub token | Arms **public sharing** — publishing titles to your connected repo |

## What's inside

- **Home** — hero, Now Streaming, BCR Studios Originals, Animations, Your Uploads
- **Upload** (locked) — password + token gate, publish console for movies & animations
- **Search** — live search + genre filters
- **Library** — My List, Continue Watching, Your Uploads
- **Profile** — stats, settings, lock / sign-out
- **Player** — BCR Play binge player: autoplay countdown, Up Next card, Skip Intro,
  full control deck (seek, volume, captions, fullscreen)

Press Play and Feel Everything. — BCR Play, powered by BCR Streamer.
