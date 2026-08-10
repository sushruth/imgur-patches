# 🧩 Imgur Morphe Patches

> ⚠️ **Experimental.** This is an unofficial, experimental Morphe patch bundle and is provided for
> **educational purposes only**. Use at your own risk. It is not affiliated with or endorsed by
> Imgur or Morphe. Violates Imgur's Terms of Service — do not use it to circumvent monetization in
> production.

Morphe patches that remove all ads from the Imgur Android app (`com.imgur.mobile`).

## How to use

Add this repo as a patch source in Morphe Manager:

https://morphe.software/add-source?github=sushruth/imgur-patches

## 🩹 Patches

- **Remove ads** — forces the app's no-ads (Emerald) entitlement flag, which gates every ad
  surface: feed ads, promoted tiles, sticky/banner/headliner/insertable/full-page ads, and
  sponsored reactions.

## 🚀 Get started

Requires a JDK 21 and the Morphe CLI. Everything runs through [devbox](https://www.jetify.com/devbox)
— see `AGENTS.md` for the locked-down workflow.

## 🛠️ Building

```sh
devbox run build       # builds patches/build/libs/patches-*.mpp
devbox run patch -- work/imgur.apk work/imgur-patched.apk
```

Building requires a GitHub PAT with `read:packages` scope (Morphe dependencies live on GitHub
Packages). See `AGENTS.md` → "GitHub Packages auth".

## 📜 License

Imgur Morphe Patches are licensed under the [GNU General Public License v3.0](LICENSE)
