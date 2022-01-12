---
title: Mail-To
---

# Mail-To Link

When you click on a Mail-To link, your default email app opens, and there will be a draft of a new email. You can set email address, subject, body, cc (email for getting a copy), and bcc (email for getting hidden copy).

Read more about this feature in [RFC 6068](https://datatracker.ietf.org/doc/html/rfc6068).

## Minimal example

For minimum usage, you have to specify at least an email address. So you get a link to email to this address: {{< mailto email="isqua@example.org" />}}

Code:

```
{{</* mailto email="isqua@example.org" /*/>}}
```

## Full example

You can specify additional parameters like subject, body, cc, and bcc, and also change the link text. Like this: {{< mailto
    email="isqua@example.org"
    subject="Hugo Shortcodes"
    body="Hi, isqua"
    cc="alex@example.org,lana@example.org"
    bcc="bigboss@example.org"
    >}}email me{{</ mailto >}}

Code:

```
If you have any questions, {{</* mailto
    email="isqua@example.org"
    subject="Hugo Shortcodes"
    body="Hi, isqua"
    cc="alice@example.org,bob@example.org"
    bcc="bigboss@example.org"
    >}}email me{{</ mailto */>}}
```

## Parameters

| Parameter  | Default | Description |
| ---------- | ------- | ----------- |
| `email`    | —       | The address to send email to |
| `subject`  | —       | The subject of the email. Any text but not too long |
| `body`     | —       | The body of the email. Any text but not too long |
| `cc`       | —       | The copy recipient’s email. If you need to send copies for multiple emails, add them separated by a comma: `alice@example.org,bob@example.org` |
| `bcc`      | —       | The hidden copy recipient’s email. The same rules as for `cc` |
| inner text | `email` field value | The text to show |
