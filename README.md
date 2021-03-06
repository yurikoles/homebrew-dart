# Dart for Homebrew

This is the official [Dart][] tap for [homebrew][].

Mac users can use these formulae to easily install and update Dart SDK. Both dev and stable channels are supported.

## Initial setup

If you don't have homebrew, install it from their [homepage][homebrew].

Then, add this tap:

```
brew tap dart-lang/dart
```

## Installing

To install the Dart SDK:

```
brew install dart
```

Tip: Once installed, homebrew will print the path to the Dart SDK. Use this path to configure Dart support
in your IDE (like WebStorm).

## Updating

Simply run:

```
brew update
brew upgrade dart
```

## Dev Releases

To install dev channel releases, instead of the stable ones, add a `--head`
flag after the brew commands:

```shell
brew install dart --head
```

Note, when updating dev releases, homebrew doesn't always update to the latest version
(see https://github.com/Homebrew/legacy-homebrew/issues/13197). In order to upgrade to
the latest dev release, run:

```shell
brew reinstall dart
```

## SDK path

Many tools, such as editors, ask you to specify the Dart SDK installation directory.
After installing via homebrew you can use the path `HOMEBREW_INSTALL/opt/dart/libexec`,
where `HOMEBREW_INSTALL` is the path to your homebrew installation directory (running
`brew --prefix` on the command line will display it).

[homebrew]: http://brew.sh/
[dart]: https://dart.dev
