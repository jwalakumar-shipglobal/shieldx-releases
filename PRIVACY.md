# ShieldX privacy policy

_Last updated: October 24, 2026 · applies to ShieldX 0.1.2 and later_

ShieldX is a browser extension for Chrome, Microsoft Edge, Brave, Opera, Vivaldi and Firefox. It blocks known advertising, tracking and malicious requests. **ShieldX does not collect, store, sell or share personal data.**

## What ShieldX collects

Nothing. There are no accounts, analytics, telemetry, crash reports, advertising IDs or third-party SDKs.

## What ShieldX stores on your device

ShieldX keeps the following in your browser's local extension storage, on your device only:

- **Settings:** which protection layers are on, your site exceptions and per-site preferences.
- **Counters:** two cumulative counts (ad elements hidden and pages filtered) and the date counting started.
- **Filter-list updates:** only if you turn on optional live updates of EasyList or EasyPrivacy. The previous version is kept for rollback.
- **Per-tab counts:** temporary counts for open tabs. These are cleared when the tab or browser closes.

None of this leaves your device. Removing ShieldX deletes all of it.

## How blocking works

- **Network blocking:** done by the browser's own blocking engine (`declarativeNetRequest`). ShieldX gives the browser its rules, but it never receives the addresses of the pages you visit or the requests they make.
- **Element hiding:** on each page, ShieldX reads only the page's hostname to decide which hiding rules apply. It doesn't record the hostname or send it anywhere.
- **YouTube ad blocking:** on YouTube pages, a ShieldX script removes ad-break entries from the video data YouTube sends to its own player. This happens entirely inside your browser, and nothing is sent anywhere.

## Network requests made by ShieldX

- **By default:** none. The EasyList and EasyPrivacy filter lists are built into the extension.
- **Optional live updates:** if you turn on live updates of these lists, ShieldX downloads them from `https://easylist.to/` about once a day, without cookies. Your browser asks your permission first. The downloads contain no information about you or your browsing.
- **No remote code:** ShieldX never downloads or runs code.

## Websites and ShieldX

No website can read or change your ShieldX settings. The published extension accepts no messages from web pages.

## Permissions

| Permission | Why ShieldX needs it |
|---|---|
| Block content on websites (`declarativeNetRequest`) | Lets the browser block requests that match ShieldX's lists |
| Read and change data on websites (content scripts) | Hides leftover ad boxes with CSS, and removes ad breaks on YouTube. Page content is never collected. |
| `storage` | Saves your settings on your device |
| `activeTab` | Lets the popup show the current site and its blocked count when you open it |
| `alarms` | Refreshes optional filter-list updates about once a day |
| `https://easylist.to/*` (optional) | Requested only if you turn on live filter-list updates |

## Children

ShieldX collects no personal information from anyone, including children.

## Changes

If this policy changes, the date above will be updated and the change will be noted in the release notes.

## Contact

Open an issue at <https://github.com/markworldorg/shieldx-releases/issues>.
