# privatematter-site

The public website for Private Matter: the home page, the [Privacy Policy](privacy/index.html), and the [Support](support/index.html) page. Plain HTML and one stylesheet; no scripts, cookies, analytics, or third-party resources.

The app links to the Privacy Policy, and App Store Connect needs both the Privacy Policy and Support URLs, so these paths must not move: `/privacy/` and `/support/`.

## Keep it true

The Privacy Policy describes what the app actually does. If a release changes what leaves the device (a new SDK, a server, Health reads, sync), update this policy and the App Store Connect privacy answers before that release ships. The app's source of truth is `DEPLOYMENT.md` in the app repository.

## Hosting

GitHub Pages from `main`, root folder. Once `privatematter.app` is registered, add a `CNAME` file containing `privatematter.app`, point the domain's DNS at GitHub Pages, and turn on Enforce HTTPS. Use relative links only; they work both at `/privatematter-site/` and at the domain root.

Published by Iron Beard Digital, LLC. Contact: support@privatematter.app.
