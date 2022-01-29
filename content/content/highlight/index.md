---
title: Text Highlight
---

# Hugo Shortcode for Text Highlight

This shortcode allows you to highlight some text inside a paragraph.

## Minimal example

Highlight {{< highlight >}}absolutely{{</ highlight >}} any words you want.

Code:

```
Highlight {{</* highlight >}}absolutely{{</ highlight */>}} any words you want.
```

## Full example

Highlight {{< highlight color="lime" >}}absolutely **any** words {{</ highlight >}} you want.

Code:

```
Highlight {{</* highlight color="lime" >}}absolutely **any** words {{</ highlight */>}} you want.
```

## Parameters

| Parameter  | Default | Description |
| ---------- | ------- | ----------- |
| color      | yellow  | The color to highlight text |
| inner text | —       | The text (markdown) to highlight |

## Installation

{{< install-shortcode name="highlight" >}}
