---
title: Get it on Google Play Badge
---

# Hugo Shortcode for Google Play Badge

Allow users to download your Application from Google Play.

*Google Play and the Google Play logo are trademarks of Google LLC.*

## Minimal example

This is a badge for downloading popular chess application:

{{< google-play-button app="com.chess" >}}

Code:

```
{{</* google-play-button app="com.chess" */>}}
```

## Full example

You can customize badge language:

{{< google-play-button
    app="com.chess"
    lang="ko"
    alt="다운로드하기 Google Play"
    width="250"
    >}}

Code:

```
{{</* google-play-button
    app="com.chess"
    lang="ko"
    alt="다운로드하기 Google Play"
    width="250"
    */>}}
```

## Parameters

| Parameter  | Default  | Description |
| ---------- | -------- | ----------- |
| `app`  | —    | The id of an application in Google Play |
| `lang` | `en` | The two-letters language code |
| `alt`  | `Get it on Google Play` | The text alternative to image for screen readers |
| `width` | `200` | The badge width in pixels |

## Site Parameters

You can set defaults in Site Parameters. For `config.toml`:

```toml
[params.HugoShortcodes.GooglePlay]
    App = 'com.chess'
    Lang = 'en'
    Alt = 'Get it on Google Play'
    Width = '200'
```

For `config.yaml`:

```yaml
params:
  HugoShortcodes:
    GooglePlay:
      App: "com.chess"
      Lang: "en"
      Alt: "Get it on Google Play"
      Width: "200"
```

## Installation

{{< install-shortcode name="deploy-to-do" >}}
