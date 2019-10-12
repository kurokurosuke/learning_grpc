# 本リポジトリの目的
WEB DB vol.110速習gRPCを学習するためのリポジトリです。

## 開発環境構築手順

### Goのインストール
右記リンクにて記載(http://golang.jp/install)
### gRPCのインストール
```
go get -u google.golang.org/grpc
```

### Protocl Buffersのインストール
以下リンクより、対象のOSにあったZIPをダウンロード
(https://github.com/google/protobuf/release)

展開したディレクトリ直下のbinディレクトリにprotoコマンドがあり、includeディレクトリによく使用するprotobufの方を定義した.protoファイルがあります。
これらの２つのディレクトリを任意の同じディレクトリに設置してください。


設置後、次のコマンドでprotocコマンドのバイナリファイルへのパスを環境変数のPATHに追加してください

```
$ export PATH=$PATH:<protocコマンドへのパス>
```

### Go用のprotocプラグインのインストール
Goのコードを生成するために必要なprotocのプラグインとして、protoc-gen-goをインストールします。

```
$ go get -u github.com/golang/protobuf/protoc-gen-go
```

### Modulesの有効化
```
$ export GO111MODULE=on
```
