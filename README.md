# Discord Role Checker

[![Discord Role Checker](media/overview.png)](media/walkthrough.mp4)
*Click preview above to view source status overview.*

![Discord Role Checker icon](icon128.png)

**Status: incomplete Chrome extension scaffold. Role checking is not implemented.**

The idea has a name and an icon; the useful part still needs building. Today this repo helps set expectations, not check anyone's roles.

The recovered local folder contains a Manifest V3 extension shell, but this public repository publishes only this README and the existing icon. The local source has not been mirrored here, so this repository is not an installable extension.

## What the local scaffold currently contains

- `manifest.json` identifies a Chrome Manifest V3 extension and declares a popup, background service worker, and extension icons.
- `index.html` displays only a static “Discord Role Checker” heading.
- `service-worker.js` defines an action-click handler that attempts to inject a JavaScript alert into the active tab.

There is no Discord page inspection, member or role lookup, API integration, or role-results UI in the recovered source. The alert handler is not a role-checking feature.

## Permissions to review

The local manifest requests `storage`, `activeTab`, and `scripting`, and lists the broad `https://*/*` host permission twice. Narrow host permissions to the sites actually required before publishing or distributing an implementation.

## Media

The included icon is the only current visual asset. No meaningful interface screenshot is available because the popup is still a heading-only placeholder.
