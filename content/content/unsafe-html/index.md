---
title: Unsafe HTML
---

# Hugo Shortcode for Unsafe HTML

This shortcode allows you to insert plain HTML in your markdown file. Use wisely. For security reasons, it’s not recommended to use code you don’t understand.

## Example

{{< unsafe-html >}}
<div style="background: crimson; color: #fff; padding: 1em; border-radius: 2em;">
    This block is rendered with plain HTML
</div>
{{</ unsafe-html >}}


Code:

```
{{</* unsafe-html >}}
<div style="background: crimson; color: #fff; padding: 1em; border-radius: 2em;">
    This block is rendered with plain HTML
</div>
{{</ unsafe-html */>}}
```

## Parameters

| Parameter  | Default | Description |
| ---------- | ------- | ----------- |
| inner code | —       | The code to render |

## Installation

{{< install-shortcode name="unsafe-html" >}}
