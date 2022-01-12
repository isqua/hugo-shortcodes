---
title: Call-to-Phone
---

# Hugo Shortcode for Call-to-Phone Link

When you click on Call-to-Phone (tel) link, your mobile phone or device will try to call the number which is set in this link.

Read more about this feature in [RFC 2806](https://datatracker.ietf.org/doc/html/rfc2806).

## Minimal example

For minimum usage you have to specify phone number: {{< tel number="+447911123456" />}}

Code:

```
{{</* tel number="+447911123456" /*/>}}
```

## Full example

You can change text of the link: {{< tel number="+447911123456" >}}call me{{</ tel >}}

Code:

```
{{</* tel number="+447911123456" >}}call me{{</ tel */>}}
```

## Parameters

| Parameter  | Default | Description |
| ---------- | ------- | ----------- |
| `number`   | —       | The phone number to call. Consider using an international phone code, because the Internet is worldwide :) |
| inner text | `number` param value | The text to show |
