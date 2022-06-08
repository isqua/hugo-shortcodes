---
title: GitHub Buttons
---

# Hugo Shortcode for GitHub Buttons

Add buttons to star, watch, or fork [Github](https://github.com/) repository or to follow/sponsor user.

The buttons are provided by [Unofficial GitHub Buttons](https://ghbtns.com/).

## Minimal example

By default it shows a small star button with a stars counter for the repository you specified:

{{< github-button owner="isqua" repo="bureau" >}}

Code:

```
{{</* github-button owner="isqua" repo="bureau" */>}}
```

## Full example

You can set different button types, large size, disable count and set the desired width:

{{< github-button type="watch" owner="isqua" repo="bureau" large=true width=170 >}}

Code of watch button:

```
{{</* github-button
    type="watch"
    owner="isqua"
    repo="bureau"
    large=true width=170
*/>}}
```

Following and sponsorship buttons do not require repo:

{{< github-button type="follow" owner="isqua" large=true >}}

Code of following button:

```
{{</* github-button type="follow" owner="isqua" large=true */>}}
```

## Parameters

| Parameter  | Default  | Description |
| ---------- | -------- | ----------- |
| `type`     | `"star"` | One of: `star`, `watch`, `fork`, `follow`, `sponsor` |
| `owner`    | —       | Username or organization name who owns the repository |
| `repo`     | —       | The repository name |
| `large`    | `false` | If true, the button is about 30px height. If false, about 20px. |
| `count`    | `true`  | Whether to show or not counter |
| `width`    | every button has its own default width | The width of the button. Perhaps if you see too much empty space on the right of the button, you may set a lower value of width |

## Site Parameters

You can set defaults in Site Parameters. For `config.toml`:

```toml
[params.HugoShortcodes.Github]
    Owner = 'your_github_login_or_org_name'
    Repository = 'your_repository_name'
```

For `config.yaml`:

```yaml
params:
  HugoShortcodes:
    Github:
      Owner: your_github_login_or_org_name
      Repository: your_repository_name
```

## Installation

{{< install-shortcode name="github-button" >}}
