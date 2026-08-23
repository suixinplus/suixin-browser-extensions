# browser-extensions

> 🇺🇸 [English](README.en.md)

浏览器扩展版本信息托管，配合 jsDelivr CDN 实现扩展内版本升级提醒检测。

## 插件列表

| 插件                                    | Chrome 商店                                                                          | Edge 商店                                                                                     | 说明                                                                                                                                      |
|-----------------------------------------|--------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| JSON Viewer Extend · 随心录Plus         | [前往安装](https://chromewebstore.google.com/search/%E9%9A%8F%E5%BF%83%E5%BD%95Plus) | [前往安装](https://microsoftedge.microsoft.com/addons/search/%E9%9A%8F%E5%BF%83%E5%BD%95Plus) | 功能丰富的 JSON/JSONP 高亮查看器，支持 XML/SOAP 排版。基于 Manifest V3 和 CodeMirror 6 构建的现代浏览器扩展，替代浏览器原生 JSON 查看器。 |
| 微信公众号文章编辑帮助工具 · 随心录Plus | [前往安装](https://chromewebstore.google.com/search/%E9%9A%8F%E5%BF%83%E5%BD%95Plus) | [前往安装](https://microsoftedge.microsoft.com/addons/search/%E9%9A%8F%E5%BF%83%E5%BD%95Plus) | 在微信公众号编辑器中注入 HTML 源码编辑功能，支持 Markdown 编写、实时预览、多端适配。                                                      |

## version.json 字段说明

| 字段                  | 类型   | 用途                             |
|-----------------------|--------|----------------------------------|
| `name`                | string | 扩展显示名称                     |
| `latest_version`      | string | 最新版本号，扩展本地与之对比     |
| `min_browser_version` | string | 最低兼容版本，低于此版本强制提醒 |
| `update_url`          | string | 跳转商店的链接，提醒用户去更新   |
| `release_notes`       | string | 更新日志，展示给用户看           |
| `released_at`         | string | 发布日期，格式为 `YYYY-MM-DD`    |

### 示例

```json
{
  "name": "JSON Viewer Extend · 随心录Plus",
  "latest_version": "1.0.5",
  "min_browser_version": "1.0.5",
  "update_url": "https://chromewebstore.google.com/search/%E9%9A%8F%E5%BF%83%E5%BD%95Plus",
  "release_notes": "修复若干已知问题，优化性能",
  "released_at": "2026-08-23"
}