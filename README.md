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
- The app is not yet signed or notarized. If macOS blocks the first launch, right-click the app and choose Open, or run `xattr -dr com.apple.quarantine "/Applications/Audax Data Manager.app"`.
