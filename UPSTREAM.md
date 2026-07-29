# Google Play Games Unity Plugin

This package is vendored from the official `playgameservices/play-games-plugin-for-unity` release `v2.1.0` (`f6d79e0ecb9c5fe8fbe383b7b8bef98938dfc632`).

It intentionally excludes the release's bundled External Dependency Manager because `AMimir` already pins a newer copy through `com.google.external-dependency-manager`.

The upstream unitypackage installs the plugin below `Assets/GooglePlayGames`. This project uses an embedded package at `Packages/com.google.play.games`, so `Editor/GPGSUtil.cs` and `Editor/GooglePlayGamesPluginDependencies.xml` contain focused path adjustments. They keep generated Google Play Games Android manifest data under `Assets/Plugins/Android/GooglePlayGamesManifest.androidlib` and Maven resolution within this package.

To upgrade, start from the matching official release package, preserve this document and the path adjustment, then run the Google Play Games Android setup window in Unity.
