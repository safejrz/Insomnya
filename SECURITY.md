# Security Policy

## Supported Scope

This repository contains a client-side bookmarklet that runs in the current browser page context.

Security expectations:

- No server component is included.
- No credentials are collected by project code.
- No analytics or telemetry endpoints are defined by project code.

## Known Constraints

- The bookmarklet requires secure contexts (`https://`) to request wake lock.
- The script executes with the same page permissions as the tab where it is launched.
- Behavior can vary by browser/version/OS power policy.

## Reporting a Vulnerability

Please report security issues privately before public disclosure.

Preferred report content:

- Browser and version
- Operating system
- Exact page context where issue appears
- Reproduction steps
- Expected vs actual behavior

If no private channel is available, open a minimal public issue without exploit details and request a private follow-up.
