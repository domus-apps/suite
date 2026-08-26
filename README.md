# Domus Suite

One zip with every released Domus app, rebuilt automatically.

**Download:** [Domus.zip](https://github.com/domus-apps/suite/releases/latest/download/Domus.zip)

The bundle workflow pulls the latest release asset of each app
(oriel, transom, pharos, coffer, atrium, jamb), assembles them into a
`Domus` folder with a README, and publishes it as this repo's latest
release. It runs on a daily schedule and on `repository_dispatch`
(`event_type: app-release`) so an app release can trigger a rebuild;
apps without a release yet are simply skipped.

Apps keep themselves current via Sparkle after installation — the
bundle only needs to be a fresh first-install entry point.
