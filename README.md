# CompilingAndTestingJava7WithGradleInWindows
Windows  の Gradleで Java 7 でビルドするための設定です。

- <a href="https://docs.gradle.org/current/userguide/java_plugin.html#sec:java_cross_compilation" target="_blank">The Java Plugin - Gradle User Manual の Compiling and testing Java 6/7</a>

のコード通りでは動かないため、Windows 用に修正したものとなります。

解説等は以下のページ参照

- <a href="http://oki2a24.com/?p=10449" target="_blank">【Gradle】Windows 環境で、Java 7 でプロジェクトをビルド、テストする方法を少し掘り下げる ? oki2a24</a>

## 環境
- Windows 10 Pro 64 bit バージョン 1709
- jdk7 jdk8 をインストール済み。
- Gradle をインストール済み。

## 本リポジトリの Gradle プロジェクトについて
次のコマンドで作成したプロジェクトです。
```bash
gradle init --type java-library
```

## ビルドの実施方法
以下コマンドでビルドしました。

Gradle は Java 8 で動かしつつ、Java コンパイルは Java 7 で実行しています。

```bash
gradlew.bat build
```
