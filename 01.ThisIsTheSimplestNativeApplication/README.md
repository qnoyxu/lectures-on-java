# 01.ThisIsTheSimplestNativeApplication

ハローワールド！コマンド

## このアプリの使い方

```sh
$ export PATH=$PATH:.
$ hello
Hello World!
```

## リリース先

あなたのPCです！！

## 構成

* `HelloWorld.java`・・・ソースコード
* `README.md`・・・このファイル
* `dist`・・・アプリ本体を格納する場所
* `build.xml`・・・`Ant`の設定ファイル
* `hello`・・・アプリを呼び出すコマンド

## Ant使わずにビルド

```sh
$ javac HelloWorld.java
```
`HelloWorld.class`っていうバイナリファイルができてる！

## テスト(動作確認)

```sh
$ java HelloWorld
```

## デプロイ！

```sh
$ mv HelloWorld.class dist/
```
