---
title: ASCII Cast from asciinema
---

# Hugo Shortcode for asciinema cast

Embed any casts from [asciinema](https://asciinema.org) to demonstrate your terminal sessions or any cli app.

## Minimal example

Here is a simple cast recorded with asciinema:

{{< asciicast id="AyrL49ZCvbvICGRmMT8Q9rz5B" >}}

Code:

```
{{</* asciicast id="AyrL49ZCvbvICGRmMT8Q9rz5B" */>}}
```

## Full example

With parameters you can override speed, theme, etc.

{{< asciicast
    id="AyrL49ZCvbvICGRmMT8Q9rz5B"
    theme="monokai"
    startAt="10"
    speed="3"
    loop=true
    autoplay=true
    columns="90"
    rows="10"
    >}}

Code:

```
{{</* asciicast
    id="AyrL49ZCvbvICGRmMT8Q9rz5B"
    theme="monokai"
    startAt="10"
    speed="3"
    loop=true
    autoplay=true
    columns="90"
    rows="10"
    */>}}
```

## Parameters

| Parameter  | Default  | Description |
| ---------- | -------- | ----------- |
| `id`       | —        | ID of your cast. |
| `theme`    | —        | One of available asciinema themes, full list you can find in [asciinema docs](https://asciinema.org/docs/embedding). |
| `startAt`  | `0`      | The time at which the playback should start. |
| `speed`    | `1`      | The speed of cast playback. `2` means 2 times faster. |
| `loop`     | `false`  | If true, the cast will be played in a repeat mode. |
| `autoplay` | `false`  | If true, the cast will start automatically, else it will start only after click. |
| `preload`  | `true`   | If true, the cast will be prefetched before user interaction. |
| `columns`  | —        | The width of cast in symbols. If don’t passed, it will be equal the size of your terminal when you recorded the cast. |
| `rows`     | —        | The height of cast in rows. |

## Site Parameters

You can set defaults in Site Parameters. For `config.toml`:

```toml
[params.HugoShortcodes.Asciicast]
    Theme = 'monokai'
    Speed = 2
    Loop = true
    AutoPlay = true
    Preload = true
    Columns = 80
    Rows = 25
```

For `config.yaml`:

```yaml
params:
  HugoShortcodes:
    Asciicast:
      Theme: 'monokai'
      Speed: 2
      Loop: true
      AutoPlay: true
      Preload: true
      Columns: 80
      Rows: 25
```

## Installation

{{< install-shortcode name="asciicast" >}}
