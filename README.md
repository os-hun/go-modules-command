# Go言語 依存モジュール管理ツール Modules
Modulesを使うには Golang 1.1以上

## 初期化
引数としてモジュール名(`example.com/go-test`)を指定
```
$ go mod init sample.com/go-test
```
`go.mod`ファイルが作成される。

## インストール
`go build`などのビルドコマンドで依存モジュールを自動インストールする。

## 依存モジュールを表示
現在の依存モジュールを確認できる。
```
$ go list -m all
```

## 追加またはバージョンアップ
```
$ go get github.com/golang/glog
```

## 使用していない依存モジュールを削除
```
$ go mod tidy
```
