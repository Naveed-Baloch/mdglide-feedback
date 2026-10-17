# MD Glide privacy policy

The official, current policy is published at [baloch.dev](https://baloch.dev/apps/mdglide/privacy.html). A copy is retained below for reference.

Last updated: October 17, 2026.

MD Glide renders and edits Markdown in your browser. The extension has no accounts, analytics, advertising, or developer-operated document-processing server. MD Glide does not upload document contents to the developer.

## Data kept in your browser

- Theme, font, layout, and editor preferences are stored in `chrome.storage.sync`. Chrome may sync these preferences through your signed-in Chrome account, according to your browser settings.
- Custom CSS is stored in `chrome.storage.local` on this device.
- Recent file names, file handles, and opening times are stored locally in IndexedDB. Handles let you reopen files after Chrome grants permission. Document contents are read from the files, rather than stored in the recent-file list. Remove a recent entry using its Remove button.
- Allowed-site permissions and automatic-render registrations are managed by Chrome. Remove a site from the MD Glide home page or Chrome's extension settings.
- On local file pages, the last theme background is cached in the page's localStorage to reduce flashes during loading.

## Network requests

Document images can load from remote servers specified by the document. Those servers receive ordinary browser request information, including your IP address and the requested URL; images can act as tracking pixels. Custom CSS containing resource URLs (such as background images or fonts) can also make requests. CSS `@import` is ignored by the viewer and removed from HTML exports.

Markdown libraries, math styles, fonts, and diagram rendering code are bundled locally. HTML exports embed math styles and fonts and do not require a math CDN. Images and other resources referenced by a document or custom CSS can still require a network connection in an exported file.

Live reload rereads local files and, for web documents, re-requests only local development servers such as localhost. It does not repeatedly poll other websites. Opening a web document or following a link uses Chrome's normal network behavior.

## Permissions and your controls

MD Glide reads local Markdown tabs only after you enable Chrome's Allow access to file URLs setting. On websites it uses access to the tab you chose through the toolbar, or a site you explicitly allowed. Saving uses a file handle you select through the browser's file picker.

You can clear custom CSS from the popup or home page, remove recent files and allowed sites, and uninstall the extension to remove its extension storage. Chrome manages synced preferences and browser storage separately. No data is sold or provided to the developer for analytics.

## Support and feedback

Support is maintained by Muhammad Naveed through the [MD Glide feedback repository](https://github.com/Naveed-Baloch/mdglide-feedback). The extension does not automatically send reports, document contents, browser history, or diagnostics to this repository.

If you choose to submit an issue, comment, screenshot, or sample file, that information is sent to GitHub and is visible publicly. The maintainer uses information you submit to investigate bugs, respond to support questions, and evaluate feature requests. Do not post confidential documents, credentials, personal information, or sensitive file paths. Use a sanitized example instead.

GitHub hosts these reports and handles account and service information under its [privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement). Support information is not used by the maintainer for advertising or sold. Public reports can remain available until removed; closing an issue does not delete it. Edit or delete your own contributions where GitHub permits, or contact the maintainer through the repository for a removal request. Public copies or third-party archives may remain outside the maintainer's control.

## Changes and contact

Updates to this policy will be posted here with a revised date. For questions about MD Glide or this policy, [open a sanitized support report](https://github.com/Naveed-Baloch/mdglide-feedback/issues/new/choose). These reports are public; do not include sensitive personal information.
