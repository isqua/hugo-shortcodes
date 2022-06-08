---
title: Text Highlight
---

# Hugo Shortcode for Text Highlight

This shortcode allows you to highlight some text inside a paragraph.

## Minimal example

Highlight {{< highlighter >}}absolutely{{</ highlighter >}} any words you want.

Code:

```
Highlight {{</* highlighter >}}absolutely{{</ highlighter */>}} any words you want.
```

## Full example

Highlight {{< highlighter color="lime" >}}absolutely **any** words {{</ highlighter >}} you want.

Code:

```
Highlight {{</* highlighter color="lime" >}}absolutely **any** words {{</ highlighter */>}} you want.
```

## Parameters

| Parameter  | Default | Description |
| ---------- | ------- | ----------- |
| color      | yellow  | The color to highlight text |
| inner text | —       | The text (markdown) to highlight |

## Installation

{{< install-shortcode name="highlighter" >}}
