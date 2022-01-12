---
title: SMS-to-Phone
---

# Hugo Shortcode for SMS-to-Phone Link

When you click on SMS-to-Phone link, your mobile phone or device will open the SMS draft to the specified number.

Read more about this feature in [RFC 5724](https://datatracker.ietf.org/doc/html/rfc5724).

## Minimal example

For minimum usage you have to specify phone number: {{< sms number="+447911123456" />}}

Code:

```
{{</* sms number="+447911123456" /*/>}}
```

## Full example

You can change text of the link: {{< sms number="+447911123456" >}}text me{{</ sms >}}

Code:

```
{{</* sms number="+447911123456" >}}text me{{</ sms */>}}
```

## Parameters

| Parameter  | Default | Description |
| ---------- | ------- | ----------- |
| `number`   | —       | The phone number to call. Consider using an international phone code, because the Internet is worldwide :) |
| inner text | `number` param value | The text to show |
