<div align="center">
  <img alt="Depensa" src="./icon.png" width="96" />
  <h1>Depensa releases</h1>
</div>

Depensa is the expense tracker that reads your orders for you. Connect the shops you already buy from, and it reads your order history, so your spending adds up without typing in a single expense. No bank or card linking. Website: [depensa.techwithanirudh.com](https://depensa.techwithanirudh.com).

This repository holds Depensa's release builds and nothing else. The app's source code is not here.

## iPhone

Depensa isn't on the App Store. You install it yourself with SideStore or AltStore, which sign it with your own Apple Account. Each IPA here is **unsigned**: SideStore or AltStore re-signs it on your phone, and Depensa never sees your Apple Account.

**Install steps: [depensa.techwithanirudh.com/ios](https://depensa.techwithanirudh.com/ios)**

The source to add in SideStore or AltStore (Sources, then +):

```text
https://depensa.techwithanirudh.com/ios/source.json
```

That address serves [`source.json`](./source.json) from this repository. With Sideloadly, download the `.ipa` from the [latest release](https://github.com/techwithanirudh/depensa-releases/releases/latest) and install it from a Mac or Windows PC.

On a sideloaded iPhone, Depensa can't receive notifications and has no Sign in with Apple; sign in with your email or Google. It needs iOS 16.4 or later.

## Android

Depensa is on [Google Play](https://play.google.com/store/apps/details?id=com.techwithanirudh.depensa).

## Checking a download

Every version in `source.json` lists the IPA's size in bytes and its SHA-256. On a Mac:

```sh
shasum -a 256 Depensa-*.ipa
```

## Licence

The builds are covered by the Depensa project's licence, the GNU Affero General Public License v3.0 or later. Its text is in [LICENSE](./LICENSE).

Questions: depensa@techwithanirudh.com
