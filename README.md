# Auto-Debugger

## 目次
|番号|項目|
|:--|:--|
|00|[概要](#00-概要)|
|01|[利用方法例](#01-利用方法例)|
|02|[設定ファイル](#02-設定ファイル)|

<br>

## 00-概要
gdb を用いて、ある特定の処理を動的に行わせ、開発速度を向上させるためのもの

<br>

## 01-利用方法例
```bash
# ヘルプを表示させる
auto-dbg [-h | --help]

# バージョンを表示させる
auto-dbg [-v | --version]

# セグフォが起こっている場所をソースコードから求める (カレントディレクトリに .c ファイルがあるものとする)
auto-dbg [-m | --mode] segmentation-fault [実行可能ファイルのパス]

# 設定ファイルの編集を行う
auto-dbg [-c | --config]
```

<br>

## 02-設定ファイル
```toml
[log]
info=""
error=""
```

