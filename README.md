# WDchocopie Extensions

A self-hosted extension store for [Mihon](https://mihon.app).

**[Tiếng Việt](README.vi.md)**

---

## What this is

Mihon is a manga reader that ships with no sources built in. Sources come from *extensions*, and extensions come from an *extension store* — a URL you add to the app. This repository is one of those stores.

Adding the URL below tells Mihon where to find the extensions listed here, and lets it notify you when a new version is published.

## How to install

**1. Install Mihon**

Download it from [mihon.app](https://mihon.app) or the [GitHub releases page](https://github.com/mihonapp/mihon/releases).

**2. Add this store**

In the app, go to **More → Settings → Browse → Extension stores → Add**, then paste:

```
https://raw.githubusercontent.com/wdchocopie/mihon-extensions/main/repo.json
```

The store should appear as *WDchocopie Extensions*.

> The URL must point directly at `repo.json`. Pasting the folder URL without the filename returns `HTTP error 404`.

**3. Install an extension**

Go to **Browse → Extensions**, find the extension, and tap the download icon.

**4. Enable the language**

Mihon hides sources whose language you have not enabled, and Vietnamese is off by default. If the list looks empty, go to **Browse → Extensions → ⋮ → Filter** and turn on **Tiếng Việt**.

## Available extensions

| Extension | Language | Version | Site |
|---|---|---|---|
| TruyenQQ VN | Vietnamese | 1.6.1 | https://truyenqq.com.vn |

## Troubleshooting

**"HTTP error 404" when adding the store**
The URL is missing `/repo.json` at the end.

**The extension list is empty**
The language filter is hiding it. See step 4 above.

**The extension list is still empty after that**
Pull down to refresh the list, or reopen the app.

**Chapter images do not load**
The site blocks images requested from outside its own pages. The extension already sends the header needed to work around this, so if images break, the site itself has likely changed — please open an issue.

## Notes

Extensions here are signed with a private key belonging to this store. Mihon checks that signature against the fingerprint published in the index, which is why extensions installed from this store are trusted automatically instead of showing an "untrusted extension" warning.

Because the signature must match, an extension installed from this store cannot be upgraded over a copy installed from somewhere else. Uninstall the old copy first.

## Source code

The extension source lives in [wdchocopie/extensions-source](https://github.com/wdchocopie/extensions-source), a fork of the [Keiyoushi](https://github.com/keiyoushi/extensions-source) repository.

## Credits

Built on [Mihon](https://github.com/mihonapp/mihon) and the extension framework maintained by [Keiyoushi](https://github.com/keiyoushi/extensions-source).
