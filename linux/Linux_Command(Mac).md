## 複数ファイル内の文字列一斉置換
[sedコマンドでディレクトリ内の全ファイルをテキスト全置換するには](https://suzuki-navi.hatenablog.com/entry/2020/10/10/185131#find%E3%82%B3%E3%83%9E%E3%83%B3%E3%83%89%E3%81%A8xargs%E3%82%B3%E3%83%9E%E3%83%B3%E3%83%89%E3%82%92%E4%BD%B5%E7%94%A8)

```cmd
find ~/<>/<> -name "*.*" | xargs grep -rl "置換対象の文字列" | xargs gsed -i "" -e "s/置換対象の文字列/置換後の文字列/g"
```
grepコマンドを併用することで、置換対象の文字列があるファイルのみをsedコマンドに渡す
```cmd
$ find . -type f -name "*.txt" | xargs grep -rl BEFORE | xargs sed -i 's/BEFORE/AFTER/g'
```

# Vim
https://zenn.dev/mo_ri_regen/articles/vim-four-modes

# WSL Linux インターネット設定
https://qiita.com/kotauchisunsun/items/71fae973afa00ebb871a

# sedコマンドについて
https://hydrocul.github.io/wiki/commands/sed.html

## システムログの特定の文字列抽出
```cmd
log stream --style syslog | grep 文字列
```

# Macのキーチェーンアクセスで自己署名証明書を作成する
https://support.apple.com/ja-jp/guide/keychain-access/kyca8916/mac

自社の証明書は下記の場所にあります。
\Iwana\Server\自社製品\Macドライバ証明書

PwdはMacと同じパスワードを使用

# Linuxのインストールログを確認する
