# Insomnya

Insomnya is a lightweight bookmarklet that helps keep your screen awake on supported HTTPS pages.

It uses the browser Screen Wake Lock API, so there is no installation, no extension, and no background service.

## Features

- Prevents screen sleep on supported pages.
- Shows a small on-page badge with status.
- Lets you pause and resume by clicking the badge.
- Removes itself cleanly when the bookmarklet is triggered again.
- Reacquires wake lock when the tab becomes visible again.

## Quick Setup

1. Open `bookmarklet.html` in your browser.
2. Make sure your bookmarks bar is visible.
3. Drag the coffee button onto the bookmarks bar.
4. Open any supported HTTPS page.
5. Click the saved Insomnya bookmark.

## Usage

1. Click the bookmarklet on a page where you want to keep the display awake.
2. Confirm the bottom-right badge shows `Awake`.
3. Click the badge to toggle `Paused` and `Awake`.
4. Click the bookmarklet again to remove the badge and clean up listeners.

## Compatibility

- Supported: Edge 84+, Chrome 84+, Opera 70+.
- Not supported: Firefox.
- Requirement: Secure context (`https://`).

## Limitations

- Wake lock is browser/device dependent and can be released by system policy (battery saver, OS rules, etc.).
- If you move to a completely different site, trigger the bookmarklet again on that page.

## Release

- Current version: `v1.0.0`
- Scope: initial public-ready bookmarklet with setup page, usage docs, MIT license, and security policy.

## Privacy and Security

- No telemetry, analytics, or network calls are added by Insomnya.
- The bookmarklet executes in the current page context and manipulates the page DOM only to add a status badge.

## Attribution

This project was inspired by concepts used in NoSleep.js.

## License

MIT. See LICENSE.
