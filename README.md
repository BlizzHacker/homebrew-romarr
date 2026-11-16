# ROMarr for Homebrew

[ROMarr](https://github.com/BlizzHacker/romarr) is the *arr for games: request a
title, and ROMarr finds it through Prowlarr, downloads it with your client,
verifies it and files it into your game library.

```bash
brew install blizzhacker/romarr/romarr
romarr                       # http://127.0.0.1:6868; the first visit sets the password
brew services start romarr   # keep it running at login
```

- macOS and Linux. Builds from the release tarball into a private Python 3.14
  environment.
- Listens on 127.0.0.1 until you set `ROMARR_HOST=0.0.0.0` (after claiming it).
- Settings live in `~/Library/Application Support/ROMarr` (macOS) or
  `~/.local/share/romarr` (Linux). Games go into `~/Games/ROMs`, or into
  `ROMARR_LIBRARY` if you set it before the first start.

The formula's source of truth is
[`packaging/homebrew`](https://github.com/BlizzHacker/romarr/tree/main/packaging/homebrew)
in the ROMarr repository. Report problems in the
[ROMarr issues](https://github.com/BlizzHacker/romarr/issues).
