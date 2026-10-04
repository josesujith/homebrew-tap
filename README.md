# josesujith/homebrew-tap

Homebrew tap for josesujith's tools.

```
brew tap josesujith/tap
```

## displayctl

Menu bar app and CLI to connect, disconnect and control macOS displays.
See [josesujith/displayctl](https://github.com/josesujith/displayctl).

Prebuilt app and CLI:

```
brew install --cask displayctl
xattr -dr com.apple.quarantine /Applications/DisplayCtl.app
```

The build is ad-hoc signed rather than notarized, so the quarantine flag has to
be cleared before Gatekeeper lets it run.

Or build the CLI from source (needs current Xcode) and run the menu bar app as
a service:

```
brew install displayctl
brew services start displayctl
```
