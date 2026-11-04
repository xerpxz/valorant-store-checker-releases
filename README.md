# Valorant Store Checker: releases

This repository only hosts **release builds** (`ValorantStoreChecker.exe`) of the Valorant Store Checker app.

## What is here

- **Releases**: each release has the built `ValorantStoreChecker.exe`. That is the only file you need to download.
- **Source code**: not in this repository. The app's source is kept in a separate private repository.
- The "Source code (zip)" and "Source code (tar.gz)" links that GitHub shows on each release are generated automatically for every repository. They only contain this README.

## How automatic updates work

1. The app asks GitHub for the **latest release** of this repository. This is a public request, so no login or token is needed.
2. If the latest version is newer than the one running, an **UPDATE TO vX.Y.Z** button appears in the app's sidebar.
3. When you click it, the app downloads `ValorantStoreChecker.exe` from the release, replaces the running file, and reopens.
4. Your saved accounts are kept, because they live in `%APPDATA%\ValorantStoreChecker\accounts.json`, outside the exe.

The app only reads from this repository. It never uploads anything here.

## Notes

- Updates only work when you run the `.exe`, not the Python source.
- Session tokens are not saved. After an update or restart, accounts show as expired until you reconnect them.
- This is an unofficial project, not affiliated with Riot Games.
