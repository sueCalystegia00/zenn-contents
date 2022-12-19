---
title: "Dockerを使ってみよう！for Windows"
emoji: "🐳"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["docker", "windows"]
published: true
---

最近，Docker を使い始めて便利さを布教したくなったにわかユーザの私ですが，どうやら Windows の方は利用までに一手間あるらしい．

ということで，ここでは，Docker をインストールすることだけにフォーカスして，Windows 向けに解説します．
後輩向けにまとめた資料の移行版なので，初心者向けのつもりです．

# Docker Desktop をダウンロード・インストール

CLI 版もあるのですが，初利用の方にとっては GUI が存在するほうが何かと安心感があるでしょう．
ここではデスクトップ版をインストールします．

https://www.docker.com/products/docker-desktop/

インストールを進めていくと，このようなウィンドウが表示されると思います．

![](https://storage.googleapis.com/zenn-user-upload/945546001e15-20221219.png)

この **Use WSL2 instead of Hyper-V(recommended)** というのが，何気に重要項目なのですが，recommended(推奨)されてるので，チェックを入れておきましょう．
デスクトップへのショートカットはお好みで．私はデスクトップには何も置かない派なので外しますが．

そのまま進めていくと，このようなエラーメッセージが表示されるかもしれません．

![](https://storage.googleapis.com/zenn-user-upload/40004f1ccaa4-20221219.png)

これが，Windows で Docker を利用する上で恐らく最初に躓くであろう問題で，この記事の本題でもあります．

私もざっくりとした理解ですが，要は
**「お前の Windows だと Linux コマンドが使えねぇから Docker は動かせねぇよ．WSL2 を有効化してから出直してきな！」**
ということです．多分．

# WSL 2 を有効化する

WSL とは"Windows Subsystem for Linux"のことで，Linux の仮想環境を動かすための仕組みです．
WSL 2 は，WSL の新しいバージョンで，WSL 1 と比べて高速化されています．

## サブシステムを有効化する

スタートから Windows PowerShell を検索し，右クリック →「管理者として実行」します．
ターミナルが開いたら，以下の 2 つのコマンドを順に実行します．

```shell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

dism.exe は Windows のシステムファイルを弄ることができるものらしい．
一応，コントロールセンターから「プログラムと機能」からもチェックできるっぽい．

## WSL2 へアップデート

[Microsoft の解説ページ](https://learn.microsoft.com/ja-jp/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package)にもある，Linux カーネル更新プログラムをダウンロードしてきます．

↓ こちらにアクセスするとダウンロードされます．
https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi

ダウンロードができ次第，もちろん起動．

![](https://storage.googleapis.com/zenn-user-upload/7d02ab2fb5f5-20221219.png)

こんな感じでセットアップが完了すれば OK

ここまで進めたら，PC 本体を再起動しましょう
大体こういうのインストールしたら再起動するでしょう？

## WSL2 を規定のバージョンに指定

またまた，PowerShell を管理者権限で起動し，以下のコマンドを実行．

```shell
wsl --set-default-version 2
```

「WSL2 との違いを~~」みたいなの出るかも．それだけ．
これで，WSL2 の有効化は完了です．

# Docker Desktop を立ち上げてみよう！

チュートリアルをやってみよう！的な画面になったら成功．
それでも Docker コマンドが上手く動かないという場合は，一度 Docker Desktop をアンインストール・再インストールしてみましょう．
