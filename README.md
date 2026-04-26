# Upload to GokApi

A [Dropzone 5](https://aptonic.com/dropzone5/) action for uploading files to a self-hosted [GokApi](https://github.com/Forceu/Gokapi) file-sharing server.

Drag files onto the action to upload them to your GokApi instance. The resulting share URL is copied straight to your clipboard, ready to paste.

## Installation

1. Download `GokApi.dzbundle`
2. Double-click to install in Dropzone, or copy it to `~/Library/Application Support/Dropzone/Actions/`

## Configuration

When you add the action, Dropzone will prompt you to fill in:

| Field | Value |
|-------|-------|
| **Server** | Your GokApi URL (e.g. `share.example.com`) |
| **Port** | Only if using a non-default port, otherwise leave blank |
| **Username** | Enter `api` (placeholder; not used, but Dropzone requires a value before the "Test Connection" button will run) |
| **Password** | Your GokApi API key (must have `UPLOAD` permission) |
| **Remote Path** | Leave blank (not used) |
| **Root URL** | Leave blank (not used) |

### Generating an API key

Sign in to your GokApi web UI, open **API** in the sidebar, and create a new key with the `UPLOAD` permission. Paste it into the action's Password field.

### HTTPS / HTTP

The action defaults to `https://`. If your instance uses plain HTTP, enter the full URL including the scheme (e.g. `http://gokapi.local`).

## Usage

- **Drag files** onto the action to upload them to GokApi. The share URL is copied to your clipboard on success.
- **Hold Shift while dragging** to bring up a single options dialog (expiry days, allowed downloads, optional password). Leave any field blank to keep the server default.
- **Click** the action to open the GokApi admin UI in your browser.

Upload progress is shown in real-time, weighted by file size when uploading multiple files.

## License

[MIT](LICENSE)
