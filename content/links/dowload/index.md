---
title: Download File
---

# Hugo Shortcode for Download File Link

Sometimes browsers are too smart and they open files instead of downloading them. If you want to allow your readers to download a file in one click, this shortcode will help you.

## Minimal example

For minimum usage you have to specify URL of file: {{< download url="./file.txt" />}}

Code:

```
{{</* download url="./file.txt" /*/>}}
```

## Full example

{{< download url="./file.txt" filename="Test File.txt" >}}Download this “Test File.txt”{{</ download >}}

## Parameters

| Parameter  | Default | Description |
| ---------- | ------- | ----------- |
| `url`      | —       | The URL to download file |
| `filename` | original filename | The name to save the file. Useful if your file has some weird URL but you want to provide a readable name for users. |
| inner text | `url` param value | The text to show |
