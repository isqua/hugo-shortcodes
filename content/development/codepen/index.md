---
title: Codepen
---

# Hugo Shortcode for Codepen

Embed any pens from [Codepen](https://codepen.io/) to demonstrate some front-end pieces. Add a caption for clarity.

## Minimal example

Here is a simple embedded iframe with a pen from Codepen:

{{< codepen id="wvrLBPZ" author="isqua" >}}

Code:

```
{{</* codepen id="wvrLBPZ" author="isqua" */>}}
```

## Full example

And this is the same pen in light UI theme, with shown tabs specified, with a specific height, a title, and a caption.

{{< codepen
    id="wvrLBPZ"
    author="isqua"
    caption="Look at this awesome example of native web stack beauty"
    title="Example of native web stack beauty"
    height="400"
    theme="light"
    tab="html,result"
    >}}

Code:

```
{{</* codepen
    id="wvrLBPZ"
    author="isqua"
    caption="Look at this awesome example of native web stack beauty"
    title="Example of native web stack beauty"
    height="400"
    theme="light"
    tab="html,result"
    */>}}
```

## Parameters

| Parameter  | Default  | Description |
| ---------- | -------- | ----------- |
| `id`       | —        | ID of your pen. You can get it from the URL of the pen |
| `author`   | —        | Username of an author on the Codepen |
| `height`   | `300`    | The height of the iframe with UI elements, not only your content |
| `theme`    | `"default"` | Codepen UI theme. May be `light`, `dark` or `default` |
| `tab`      | `"result"` | Tab or two which is shown by default. Possible values are: `result`, `html`, `css`, js` or two of them separated by comma, like this: `html,result` |
| `caption`  | —        | A caption to show under the pen |
| `title`    | `caption` if specified, otherwise `id` | Pen title to show when the iframe is not loaded yet |

## Site Parameters

You can set defaults in Site Parameters. For `config.toml`:

```toml
[params.HugoShortcodes.Codepen]
    Author = 'your_login_on_codepen'
    Theme = 'light'
    Height = '300'
```

For `config.yaml`:

```yaml
params:
  HugoShortcodes:
    Codepen:
      Author: "isqua"
      Theme: "light"
      Height: 300
```

## Installation

{{< install-shortcode name="codepen" >}}
