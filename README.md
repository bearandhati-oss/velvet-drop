# Velvet Drop site (https://bearandhati-oss.github.io/velvet-drop)

Static site: home, support, and privacy. Same pattern as the Folkguard and Brecken's Beats pages: one public repo per app under the `bearandhati-oss` GitHub account, served by GitHub Pages from the `main` branch root, with a black support bar on the support page that points to the central Cole Builds support page (https://colebuildsai.com/support#velvet-drop). Links are relative so they work under `/velvet-drop/`, and GitHub Pages serves `privacy.html` at `/privacy` and `support.html` at `/support`.

URLs for App Store Connect once published:
- Privacy Policy URL: https://bearandhati-oss.github.io/velvet-drop/privacy
- Support URL: https://bearandhati-oss.github.io/velvet-drop/support

Publish with `Tools/publish_site.sh` from the project root (needs `gh auth login` as `bearandhati-oss`). It creates the public repo `bearandhati-oss/velvet-drop` if missing, pushes this folder as the `main` branch, and turns on GitHub Pages for `main` at `/`. Nothing in this folder is published until that script is run by hand.

The central support page at colebuildsai.com is a separate Netlify site. Add a Velvet Drop card there with the anchor id `velvet-drop` so the support bar's link lands on it.

Check after deploying:
- https://bearandhati-oss.github.io/velvet-drop/privacy and /support load without a redirect.
- Both pages show the colebuildsai@gmail.com contact and the support bar link.
