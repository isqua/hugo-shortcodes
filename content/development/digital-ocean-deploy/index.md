---
title: Digital Ocean Deploy Buttons
---

# Hugo Shortcode for Deploy to Digital Ocean Buttons

Allow users to start your Application hosted on GitHub with a click with official **Deploy to DigitalOcean** buttons.

Do not forget to prepare your repository following [the official DigitalOcean guide](https://docs.digitalocean.com/products/app-platform/how-to/add-deploy-do-button/).

Add your [referral code](https://docs.digitalocean.com/products/accounts/referrals/) to get some benefits from DigitalOcean, if someone will register by your link.

## Minimal example

This is just an example of a button, my project is not configured to easy deploy yet:

{{< deploy-to-do owner="isqua" repo="docker-koken" >}}

Code:

```
{{</* deploy-to-do owner="isqua" repo="docker-koken" */>}}
```

## Full example

{{< deploy-to-do
    owner="isqua"
    repo="docker-koken"
    branch="master"
    theme="blue-ghost"
    alt="Deploy Koken"
    refcode="a67fb72fe5ce"
    >}}

Code:

```
{{</* deploy-to-do
    owner="isqua"
    repo="docker-koken"
    branch="master"
    theme="blue-ghost"
    alt="Deploy Koken"
    refcode="a67fb72fe5ce"
    */>}}
```

## Parameters

| Parameter  | Default  | Description |
| ---------- | -------- | ----------- |
| `owner`    | —        | Username or organization name who owns the repository |
| `repo`     | —        | The repository name |
| `branch`   | `"main"` | The repository branch to deploy |
| `theme`    | `"blue"` | One of button theme: `blue`, `blue-ghost`, `white-ghost`, or `white` |
| `alt`      | `"Deploy to Digital Ocean"` | The text alternative to image for screen readers |
| `refcode`  | —        | The code of Digital Ocean [referral program](https://docs.digitalocean.com/products/accounts/referrals/).
