# Marcus for Mac

The installers for **Marcus for Mac**, the desktop app of [Marcus, the PDF editor for lawyers](https://marcus.tkjglobalmedia.com), from TKJ Global Media Ltd.

**Download and instructions: [marcus.tkjglobalmedia.com/download](https://marcus.tkjglobalmedia.com/download)**

This repository holds the installers and nothing else. Each version is under [Releases](https://github.com/TKJGlobalMedia/marcus-desktop/releases). Marcus's source code is not here.

## The files

| File | For |
| --- | --- |
| `Marcus-<version>-mac-arm64.dmg` | Macs with Apple silicon (M1 or later) |
| `Marcus-<version>-mac-x64.dmg` | Macs with an Intel processor |

They need macOS 13 Ventura or later. You sign in with your firm's Marcus account.

## Checking a download

The app is signed with TKJ's Apple Developer ID, `Developer ID Application: TKJ GLOBAL MEDIA LTD (665CS52N48)`, and notarised by Apple. Each release lists the SHA-256 fingerprint of its files.

```sh
shasum -a 256 ~/Downloads/Marcus-0.0.1-mac-arm64.dmg
spctl -a -t exec -vv /Applications/Marcus.app
```

The first prints the file's fingerprint. The second answers `source=Notarized Developer ID`.

## Questions

marcus@tkjglobalmedia.com

© 2026 TKJ Global Media Ltd, registered in England and Wales, company number 08272919. All rights reserved.
