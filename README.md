# ShieldX — Ad & Tracker Blocker for Chrome

Privacy-first ad, tracker and security blocker for Google Chrome (Manifest V3).
No account, no analytics, no telemetry. Your settings never leave your device.

This repository hosts **ShieldX test releases** and collects **bug reports**. The extension's source code isn't published here.

> ⚠️ ShieldX is currently in **public testing**. Only install builds downloaded from this repository's [Releases page](https://github.com/jwalakumar-shipglobal/shieldx-releases/releases), and always check the checksum.

## Download

1. Open the **[latest release](https://github.com/jwalakumar-shipglobal/shieldx-releases/releases)**.
2. Download `ShieldX-v<version>.zip` and `SHA256SUMS.txt`.
3. Check that the file isn't damaged or altered:
   - **Linux and macOS:** `sha256sum -c SHA256SUMS.txt` (on macOS: `shasum -a 256 -c SHA256SUMS.txt`)
   - **Windows (PowerShell):** `Get-FileHash .\ShieldX-v0.1.0.zip -Algorithm SHA256`, then compare the result with `SHA256SUMS.txt`

## Install in Chrome

1. Unzip the file into a folder you'll keep. Chrome loads ShieldX from that folder, so don't delete it.
2. Open `chrome://extensions`.
3. Turn on **Developer mode** (switch in the top-right corner).
4. Click **Load unpacked** and select the unzipped folder. It contains `manifest.json`.
5. Pin ShieldX: click the puzzle-piece icon in the toolbar, then the pin next to ShieldX.

**Requirements:** Google Chrome 121 or newer on Windows, macOS, Linux or ChromeOS.

**To update:** unzip the new version over the same folder, then click **reload ↻** on ShieldX in `chrome://extensions`.

**To remove:** click **Remove** on ShieldX in `chrome://extensions`. All ShieldX data is deleted along with it.

## What ShieldX does

**On by default:**
- **Ads:** blocks third-party ad servers, ad exchanges, video ad servers and affiliate trackers.
- **Trackers:** blocks analytics, session recording, fingerprinting and social-media pixels.
- **Security:** blocks cryptominers, malvertising and pop-under networks.
- **Telemetry:** blocks error-reporting and device-maker tracking endpoints.
- **Ad hiding:** hides the empty boxes ads leave behind, with a per-site off switch.

**Optional:**
- **Strict mode:** adds social widgets, cookie-consent banners and chat widgets.
- **EasyList and EasyPrivacy:** community lists you can download for wider coverage.

**Per-site control:** pause ShieldX on any site in one click from the popup.

## Known limitations

- No blocker can stop every ad, and websites change how they deliver ads.
- Video and audio ads served from the same servers as the content can't be reliably blocked. This includes many YouTube and Spotify ads.
- Changing protection for a site takes effect after reloading the page.

## Report a problem

Please **[open an issue](https://github.com/jwalakumar-shipglobal/shieldx-releases/issues/new/choose)** and include:
- your Chrome version
- the website address
- what you expected to happen

Never include passwords, cookies or personal data.

## Privacy

- **Local storage only:** ShieldX stores your settings and counters only in Chrome's local extension storage on your device.
- **No browsing data:** blocking is done by Chrome's built-in engine, so ShieldX doesn't receive the addresses of the pages you visit.
- **Optional downloads only:** ShieldX's only network requests are the optional EasyList and EasyPrivacy downloads from `easylist.to`. They happen only after you turn those lists on and Chrome asks for permission.

## Credits

EasyList and EasyPrivacy are © The EasyList authors (GPLv3 / CC BY-SA 3.0). ShieldX downloads them only if you turn them on.
