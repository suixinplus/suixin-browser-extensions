# browser-extensions

> 🇨🇳 [中文文档](README.md)

Browser extension version info hosting, powered by jsDelivr CDN for in-extension update notifications.

## Extensions

| Extension                                           | Chrome Web Store                                                                    | Edge Add-ons                                                                                 | Description                                                                                                                                                                                                                |
|-----------------------------------------------------|-------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| JSON Viewer Extend · 随心录Plus                     | [Install](https://chromewebstore.google.com/search/%E9%9A%8F%E5%BF%83%E5%BD%95Plus) | [Install](https://microsoftedge.microsoft.com/addons/search/%E9%9A%8F%E5%BF%83%E5%BD%95Plus) | A feature-rich JSON/JSONP syntax highlighter and viewer with XML/SOAP formatting support. A modern browser extension built on Manifest V3 and CodeMirror 6, serving as a replacement for the browser's native JSON viewer. |
| WeChat Official Account Article Editor · 随心录Plus | [Install](https://chromewebstore.google.com/search/%E9%9A%8F%E5%BF%83%E5%BD%95Plus) | [Install](https://microsoftedge.microsoft.com/addons/search/%E9%9A%8F%E5%BF%83%E5%BD%95Plus) | Injects HTML source editing capabilities into the WeChat Official Account editor, with Markdown authoring, live preview, and multi-platform adaptation.                                                                    |

## version.json Fields

| Field                 | Type   | Description                                                                    |
|-----------------------|--------|--------------------------------------------------------------------------------|
| `name`                | string | Extension display name                                                         |
| `latest_version`      | string | Latest version number, compared against the installed version in the extension |
| `min_browser_version` | string | Minimum compatible version, forces an upgrade prompt if below this version     |
| `update_url`          | string | Link to the store page, directs users to install the update                    |
| `release_notes`       | string | Changelog displayed to users in the update notification                        |
| `released_at`         | string | Release date in `YYYY-MM-DD` format                                            |

### Example

```json
{
  "name": "JSON Viewer Extend · 随心录Plus",
  "latest_version": "1.0.5",
  "min_browser_version": "1.0.5",
  "update_url": "https://chromewebstore.google.com/search/%E9%9A%8F%E5%BF%83%E5%BD%95Plus",
  "release_notes": "修复若干已知问题，优化性能",
  "released_at": "2026-08-23"
}