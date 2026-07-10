# Security Policy

## Scope

Burger 101 is a static, client-side HTML/CSS/JS page with no backend, no server-side code, and no user accounts or stored personal data. It loads Leaflet, Leaflet.markercluster, and Google Fonts from public CDNs, and calls the browser's Geolocation API only when the user taps "Find me."

Given that scope, the realistic security surface is small, but reports are still welcome — e.g. XSS via the search/filter inputs, a malicious/compromised CDN dependency, or a link that doesn't go where it claims (Directions/Instagram links).

## Reporting a Vulnerability

If you find a security issue:

1. Do **not** open a public GitHub issue for it.
2. Open a private report via GitHub's **Security → Report a vulnerability** tab on this repo (or contact the maintainer directly if that's unavailable).
3. Include steps to reproduce, the affected file/version, and your browser/OS.

You should get an initial response within a few days. Since this is a small hobby project maintained in spare time, please be patient.

## Supported Versions

Only the latest version of each HTML file in this repo is supported. There are no LTS or patched-back releases.

## Disclosure

Once a fix is available, it will be noted in the commit history / release notes. Credit will be given to reporters who want it.
