---
title: Buy Me a Coffee Button
---

# Hugo Shortcode for Buy Me a Coffee

## Minimal example

Here is a simple embedded button for getting a donation via the [Buy Me a Coffee](https://www.buymeacoffee.com) service:

{{< bmc-button slug="isqua" >}}

Code:

```
{{</* bmc-button slug="isqua" */>}}
```

## Full example

You can customize colors and text:

{{< bmc-button
    slug="isqua"
    text="Buy me a milk"
    font="Bree"
    button-color="614484"
    coffee-color="FFFFFF"
    cup-color="FFDD00"
    font-color="FFFFFF"
    >}}

Code:

```
{{</* bmc-button
    slug="isqua"
    text="Buy me a milk"
    font="Bree"
    button-color="614484"
    coffee-color="FFFFFF"
    cup-color="FFDD00"
    font-color="FFFFFF"
    */>}}
```

Or use any emoji instead of the cup:

{{< bmc-button
    slug="isqua"
    text="Buy me a croissant"
    emoji="🥐"
    font="Lato"
    button-color="F5F5EA"
    font-color="C2410C"
    >}}

Code:

```
{{</* bmc-button
    slug="isqua"
    text="Buy me a croissant"
    emoji="🥐"
    font="Lato"
    button-color="F5F5EA"
    font-color="C2410C"
    */>}}
```

## Parameters

| Parameter      | Default  | Description |
| -------------- | -------- | ----------- |
| `slug`         | —        | Slug of your Buy Me a Coffee account. You can get it from the URL of your page url on Buy Me a Coffee |
| `emoji`        | —        | If you don’t want coffee, you can draw some emoji instead of the cup |
| `text`         | Buy me a coffee | The text on the button |
| `font`         | Cookie   | The font family of the button text. See all the available fonts at the Buy Me a Coffee [buttons page](https://www.buymeacoffee.com/button-and-graphics) |
| `button-color` | `ffdd00` | The color of the button |
| `font-color`   | `000000` | The color of the text |
| `coffee-color` | `ffffff` | The color of the drink in the cup |
| `cup-color`    | `000000` | The color of the cup |

## Site Parameters

You can set defaults in Site Parameters. For `config.toml`:

```toml
[params.HugoShortcodes.BuyMeACoffee]
    Slug = 'isqua'
    Text = 'Buy me a croissant'
    Font = 'Lato'
    Emoji = '🥐'
    ButtonColor = 'ffdd00'
    FontColor = '000000'
    CoffeeColor = 'ffffff'
    CupColor = '000000'
```

For `config.yaml`:

```yaml
params:
  HugoShortcodes:
    BuyMeACoffee:
      Slug: "isqua"
      Text: "Buy me a croissant"
      Font: "Lato"
      Emoji: "🥐"
      ButtonColor: "ffdd00"
      FontColor: "000000"
      CoffeeColor: "ffffff"
      CupColor: "000000"
```

## Installation

{{< install-shortcode name="bmc-button" >}}
