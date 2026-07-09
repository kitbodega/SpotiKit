# SpotiKit

A JavaScript userscript that customizes the Spotify Web interface.

## Installation

1. Install [Tampermonkey](https://www.tampermonkey.net/)[Violentmonkey](https://violentmonkey.github.io/).
2. Get [uSpot](https://github.com/Myst1cX/uSpot/releases/tag/2.0). [how do I install this extension in mobile?](https://github.com/Myst1cX/uSpot/#installation-on-a-mobile-device)
3. Click the raw link below — Tampermonkey/Violentmonkey will open the install dialog:
   - **https://raw.githubusercontent.com/kitbodega/SpotiKit/main/SpotiKitMobileDesktop.user.js**
3. Click **Install**.
3. Go to [open.spotify.com](https://open.spotify.com) and reload.

## Features

### Mobile-like Desktop UI (`open.spotify.com`)
- **Floating player** with glassmorphism (blur, border, rounded corners) and minimize toggle button
- **Tabs navigation bar** Home, Search, and Library tabs
- **Library as full-screen overlay** (no persistent sidebar I think the library is broken.)
- **Search input hidden globally**, shown only on Search page


## Premium Spoof fake & Page Blockers:
Removed from mobile; use the [Myst1cX fork](https://github.com/Myst1cX/SpotiKit) Desktop only.

## Notes

- Client-side JavaScript only. No Spotify servers are modified.
- No account data is changed. Visual customization only.

## Ad-Blocking

* Special thanks to **[Myst1cX](https://github.com/Myst1cX)** for their excellent work on [this extension](https://github.com/Myst1cX/uSpot/).(This is the one I highly recommend for spotikit)

For ad-blocking, using the **[uBlock Origin](https://ublockorigin.com/)** browser extension instead of custom userscripts[cite: 1].
### Why use uBlock Origin?
* **Reliability:** uBlock Origin uses the `webRequest` API to intercept and replace ad requests with silent placeholders (e.g., 1-second clips), ensuring a seamless listening experience without playback errors
* **Maintenance:** Ad-blocking filters require constant updates due to changes on Spotify's side. The uBlock Origin team is best positioned to monitor and push these updates immediately.
## License

MIT
