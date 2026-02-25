# AgentBrowser Sparkle Updates Repo

This repository hosts Sparkle appcast feeds and release notes for AgentBrowser updates.
Enable GitHub Pages on the `main` branch (root) so Sparkle clients can access the feed URLs.

## Expected URLs

- `https://studio-82.github.io/agentbrowser-updates/appcast.xml`
- `https://studio-82.github.io/agentbrowser-updates/appcast-staging.xml`
- `https://studio-82.github.io/agentbrowser-updates/releases/<version>.html`

## Checklist

1. Create the repo and enable GitHub Pages
2. Confirm the Pages URL works
3. Ensure AgentBrowser `SUFeedURL` matches the final repo path
4. Configure the app repo CI secrets so the release workflow can publish signed appcast entries here

## Notes

- `appcast.xml` items are generated and signed by the app repo release workflow using Sparkle's `generate_appcast`.
- Keep this repo lightweight; release binaries stay on GitHub Releases in the app repo.
