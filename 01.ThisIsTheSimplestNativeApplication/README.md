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

* `src`・・・ソースコードを置く場所
  * `HelloWorld.java`・・・今回のソースコード
* `README.md`・・・このファイル
* `dist`・・・バイナリファイル達を格納する場所。`build`って名前のことも多い
  * `HelloWorld.java`・・・`HelloWorld.java`から作られるバイナリファイル
* `build.xml`・・・`Ant`の設定ファイル
* `hello`・・・アプリを呼び出すコマンド

## Ant使わずにビルド

```sh
$ cd src
$ javac HelloWorld.java
```
`HelloWorld.class`っていうバイナリファイルができてる！

## テスト(動作確認)

```sh
$ java HelloWorld
Hello World!
```

## デプロイ！

```sh
cd ..
$ mkdir dist
$ mv src/HelloWorld.class dist/
```

## ひとつの問題点

* ソースファイルの数がすごく増えたらどうする？？
  毎回、全部に`javac`やって全部移動して配置するのは大変…

## Antを使ってビルド！

`build.xml`に、コンパイルするファイルとか配置構造とかを記述する
```
$ ant
```
これで`dist`ディレクトリとバイナリファイルができる！
