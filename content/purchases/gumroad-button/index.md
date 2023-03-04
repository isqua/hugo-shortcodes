---
title: Gumroad
---

# Hugo Shortcode for Gumroad

Sell your products with [Gumroad](https://gumroad.com/) buttons and overlays. Read more in [Gumroad Help](https://help.gumroad.com/article/135-setting-up-the-gumroad-overlay-on-your-website).

## Minimal example

Here is a simple embedded button for Gumroad good:

{{< gumroad-button id="demo" >}}Get on{{</ gumroad-button >}}

Code:

```
{{</* gumroad-button id="demo" >}}Get on{{</ gumroad-button */>}}
```

## Full example

{{< gumroad-button id="demo" affiliate="12345678" >}}Get with 10% discount on{{</ gumroad-button >}}

Code:

```
{{</* gumroad-button id="demo" affiliate="12345678" >}}Get with 10% discount on{{</ gumroad-button */>}}
```

## Parameters

| Parameter   | Default  | Description |
| ----------- | -------- | ----------- |
| `id`        | —        | ID of your good. You can get it from the URL of the good on Gumroad |
| `affiliate` | —        | Code of your affiliate Program |
| inner text  | —        | The text to show on the button |

## Site Parameters

You can set defaults and [custom domain](https://help.gumroad.com/article/153-setting-up-a-custom-domain) in Site Parameters. For `config.toml`:

```toml
[params.HugoShortcodes.Gumroad]
    Host = 'https://your_domain.com'
    Affiliate = '123456789'
```

For `config.yaml`:

```yaml
params:
  HugoShortcodes:
    Gumroad:
      Host: "https://your_domain.com"
      Affiliate: "123456789"
```

## Installation

{{< install-shortcode name="gumroad-button" >}}
