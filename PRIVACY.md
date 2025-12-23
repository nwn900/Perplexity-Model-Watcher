# Privacy Policy for Model Watcher

Effective date: 2025-11-05

Summary
- Model Watcher does not collect, transmit, sell, or share any personal data.
- All processing happens locally in your browser.

What the extension does
- Injects a small script into pages on https://*.perplexity.ai/* to read the text of network responses (fetch/XHR) and extract the fields `display_model` and `user_selected_model` for display.
- Shows those values in an in‑page overlay and the extension popup.
- Stores user preferences (only the overlay toggle) using Chrome/Brave `chrome.storage.sync` and `chrome.storage.local` for the overlay position.

Data flow and retention
- No data is sent to any remote server by this extension.
- The extension does NOT collect browsing history, page content, or any identifiers beyond the two model fields mentioned above, which are displayed only to you and not persisted.
- Overlay position (per origin) is kept locally with `chrome.storage.local` and can be cleared by removing the extension or clearing extension storage.

Permissions
- The extension requests minimal permissions: `storage`, `tabs`, and access only to pages under https://*.perplexity.ai/*.

Contact
- Open an issue on the GitHub repository for questions or concerns.
