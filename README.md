# SpotiKit

A JavaScript userscript that customizes the Spotify Web interface.

## Installation

1. Install [Tampermonkey](https://www.tampermonkey.net/)[Violentmonkey](https://violentmonkey.github.io/).
2. Click the raw link below — Tampermonkey/Violentmonkey will open the install dialog:
   - **https://raw.githubusercontent.com/kitbodega/SpotiKit/main/SpotiKitMobileDesktop.user.js**
3. Click **Install**.
4. Go to [open.spotify.com](https://open.spotify.com) and reload.

## Features

### Mobile-like Desktop UI (`open.spotify.com`)
- **Floating player** with glassmorphism (blur, border, rounded corners) and minimize toggle button
- **Transparent bottom navigation bar** with Home, Search, and Library tabs
- **Library as full-screen overlay** (no persistent sidebar)
- **Search input hidden globally**, shown only on Search page
- **Right sidebar (Now Playing) visible** but selectively collapsed — hides close button, artist bio, and credits; keeps the **queue list** visible
- **Auto-closes Now Playing panel** when it opens on song play (MutationObserver)
- Official Spotify SVGs extracted from the DOM for the bottom nav icons

### Premium Spoof fake & Page Blockers (`spotify.com/account/*`, payments, etc.)
- Text replacements (e.g. "Spotify Free" → "Premium Individual", "Shuffle play" → "Play any song")
- Pink Premium branding on plan cards
- Premium/duo/student/family pages blocked — replaced with "you don't need Premium" message
- Payment page blocker — replaces `payments.spotify.com` with "don't waste your money" message
- Disable payment forms and checkout buttons
- Hide download/install app prompts, "Open in Desktop App" elements, and Premium navigation links

## Notes

- Client-side JavaScript only. No Spotify servers are modified.
- No account data is changed. Visual customization only.

##Acknowledgments:

* Special thanks to **[Myst1cX](https://github.com/Myst1cX)** for their excellent work on [this extension](https://www.reddit.com/c/chatwRCHSlWr/s/hi7uBRaaHr)[cite: 1].(This is the one I highly recommend for spotikit) [how do I install this extension in mobile?](https://github.com/Myst1cX/uSpot/#installation-on-a-mobile-device)

## Ad-Blocking

For ad-blocking, using the **[uBlock Origin](https://ublockorigin.com/)** browser extension instead of custom userscripts[cite: 1].
### Why use uBlock Origin?
* **Reliability:** uBlock Origin uses the `webRequest` API to intercept and replace ad requests with silent placeholders (e.g., 1-second clips), ensuring a seamless listening experience without playback errors[cite: 1].
* **Maintenance:** Ad-blocking filters require constant updates due to changes on Spotify's side. The uBlock Origin team is best positioned to monitor and push these updates immediately[cite: 1].
* **Performance:** Relying on DOM-based hiding or silencing techniques is inefficient and can lead to playback issues or forced waits during ad intervals. Using a dedicated extension ensures the script remains lightweight and focused on UI customization[cite: 1].
## License

MIT
