# Novice Code

A phone-first creative dashboard. It reads your day (weather, daylight, room sound, what you've been listening to, what's on your mind) into a five-color creative code, then pulls live references to build from: mood boards, fits, songs with previews, vertical video, and artwork.

Everything runs in the browser. There's no server and no account. Keys, your library, and saved days stay on your phone.

## Put it on your phone (about 5 minutes)

1. Make a free GitHub account if you don't have one.
2. Create a new public repository called `novice-code`.
3. Upload every file in this folder (drag them onto the repo page) and commit.
4. In the repo, go to **Settings → Pages**, set the source to **Deploy from a branch**, pick `main` and `/ (root)`, and save.
5. After a minute you'll get a link like `https://yourname.github.io/novice-code/`. Open it in Safari on your iPhone.
6. Tap **Share → Add to Home Screen**. It now opens like an app.

Location and the microphone only work over HTTPS, which GitHub Pages gives you for free. Netlify Drop (app.netlify.com/drop) also works: drag the folder in and you get a link.

## Set it up

Open **Settings** in the app.

- **Location**: tap Allow. Used for local weather and daylight (Open-Meteo, no key needed).
- **Microphone**: tap Listen now. Measures how loud the room is for five seconds. Nothing is recorded or sent anywhere.
- **Anthropic API key**: needed for **Generate today** and **Scan**. Get one at console.anthropic.com. Calls go straight from your phone to Anthropic and are billed to your account.
- **Pexels API key** (optional, free at pexels.com/api): adds real photos and playable vertical video clips.

Without keys the app still works: Today builds options from your saved codes, and the references still load from the free sources.

## Where references come from

Shown inside the app (free, no key):
- **Are.na** and **Openverse** for mood board and fit images
- **Art Institute of Chicago** for artwork
- **Apple's iTunes Search** for album art and 30-second song previews

With a Pexels key: **Pexels** photos and vertical video.

One tap away (opens the app or site): Pinterest, Cosmos, Grailed, Depop, SSENSE, Spotify, Apple Music, SoundCloud, TikTok, YouTube, Letterboxd, Behance.

Pinterest, Spotify, TikTok, and Instagram don't offer public search that a small app like this can call, so those are links instead of previews.

## Keep your library

Your library lives in this browser only. Use **Export library** now and then to back it up, and **Import library** to move it to a new phone.

## Developer view

Settings → Developer view shows the color system, raw values, and fine-tune controls on scans.

## Notes

- Your API keys are stored in your browser. Don't use this on a shared phone, and don't commit keys to the repo.
- The external sources can change or rate-limit at any time. If a section comes back empty, the links under it still work.

## License

MIT. See LICENSE.
