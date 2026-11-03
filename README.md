# audaxdm-tap

Homebrew tap for [Audax Data Manager](https://github.com/commandprompt/audax-data-manager).

## Install

The repository is not named `homebrew-audaxdm`, so tap it with its URL:

```
brew tap commandprompt/audaxdm https://github.com/commandprompt/audaxdm-tap
brew install --cask audaxdm
```

## Upgrade / uninstall

```
brew upgrade --cask audaxdm
brew uninstall --cask audaxdm        # add --zap to also remove app data
```

## Notes

- Both Intel (x86_64) and Apple Silicon (arm64) builds are supported; Homebrew picks the matching DMG automatically.
- The app is not yet signed or notarized. macOS blocks the first launch. Before opening the app, run `xattr -dr com.apple.quarantine "/Applications/Audax Data Manager.app"`. Alternatively, open the app once, then click "Open Anyway" in System Settings > Privacy & Security.
