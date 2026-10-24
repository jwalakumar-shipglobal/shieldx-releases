# Changelog

All ShieldX releases. Downloads are on the [Releases page](https://github.com/markworldorg/shieldx-releases/releases).

## v0.1.2 — October 24, 2026 (latest)

**Much stronger blocking**
- EasyList and EasyPrivacy are now built in and on by default. That adds tens of thousands of extra ad, pop-up and tracker rules, plus element hiding for individual sites.
- ShieldX's own rules take priority over community-list exceptions, so nothing ShieldX blocked before slips through.
- Measured on superadblocktest.com (October 2026): 92% with default settings, 98% in Strict mode.

**YouTube**
- New "Block YouTube video ads" setting, on by default. It removes ad breaks from YouTube's player data.
- Any ad that still starts plays muted at 16× speed while ShieldX presses Skip. Your volume and speed are then restored.
- Best effort: YouTube changes often, and some videos may take a few extra seconds to start.

**More browsers**
- One build works in Chrome, Microsoft Edge, Brave, Opera and Vivaldi (Chromium 121+).
- New Firefox build (Firefox 128+). Until it's signed on addons.mozilla.org, Firefox loads it as a temporary add-on.
- In Firefox, the blocked-count badge and the popup's per-tab count aren't available. All blocking works.

## v0.1.1 — October 24, 2026

v0.1.1 wasn't published as a separate download. All of these changes are included in v0.1.2.

**Downloads & support**
- Test builds are published on GitHub Releases, with a SHA-256 checksum for every download.
- Bug reports go to GitHub Issues, with a guided form for the details we need.
- New **Report a problem** and **Get updates** buttons in the ShieldX popup and settings.
- Links inside the extension now open public pages instead of a local address.

**Security**
- Builds without a website no longer accept messages from any web page, so only ShieldX itself can change its settings.

## v0.1.0 — October 24, 2026 (first release)

**Protection**
- Blocks hundreds of known ad servers, ad exchanges, trackers, fingerprinting and identity-sync services, using Chrome's built-in blocking engine.
- Security protection against browser cryptominers, malvertising and pop-under networks.
- Telemetry blocking for error-reporting services and device-maker tracking endpoints.
- Optional Enhanced privacy and "Cookie banners, chat & experiments" lists for maximum protection.
- Best-effort blocking of ad endpoints on YouTube and Spotify Web.
- Cosmetic filtering hides leftover ad boxes, with a per-site off switch.

**Control**
- One-click allowlist from the popup, with subdomain-aware matching.
- Optional EasyList and EasyPrivacy domain rules, validated before use, with rollback.
- A YouTube helper that presses YouTube's own Skip button when it's available.

**Privacy & design**
- No account, no telemetry, no remote code. All settings stay on your device.
- Light and dark themes across the popup and settings.
