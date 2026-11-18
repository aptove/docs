# Docs Guidelines

## Navigation

The navigation is defined in `docs.json` (Mintlify v3 format). `mint.json` is the legacy format and is no longer the source of truth.

### Adding a new page

When you create a new `.mdx` file, **do not add it to the navigation automatically**. Instead, ask the user:

> "Where should this page appear in the navigation bar? Options: which group (Getting Started / Aptove Router / Mobile App / Push Notifications), and where within that group (before/after which page)."

Wait for the user's answer before editing `docs.json`.

### Navigation file structure (`docs.json`)

```
navigation.tabs[0] ("Docs")
  groups:
    - Getting Started
    - Aptove Router
        - Transports (sub-group)
        - Advanced (sub-group)
    - Mobile App
    - Push Notifications
```
