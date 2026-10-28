# Security and privacy

Security fixes apply to the current Comments v6 source in the default branch. Report vulnerabilities through GitHub Security Advisories. Do not include keys, private URLs or personal exports in public issues.

The script calls www.googleapis.com/youtube/v3 with a user-provided YouTube Data API key. It may optionally save that key in localStorage under yt-comments-exporter-api-key-v6 on the YouTube origin. Same-origin scripts and extensions may read it; disable key saving and restrict the key appropriately when needed. No key is embedded in this repository.

Exported data stays in browser memory until download. No analytics, project backend or external ZIP library is used. Review the readable source before execution.
