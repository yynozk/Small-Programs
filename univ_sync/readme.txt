rsync を使用した同期を簡単化するプログラム。

upload_config.yaml に
- バックアップ元ディレクトリ
- バックアップ先ホスト
- バックアップ先ディレクトリ
- excludeディレクトリ
- includeディレクトリ
を記述すると、同期に適した "-av", "--delete" オプションをつけて、
それに従ったrspecコマンドを返してくれる。
詳しい使用方法はコード参照。

出力してコピペしてコマンドのオプションを弄って使うも良し、
exec()に渡してスクリプトから実行してしまうも良し。
