---
title: "Mac購入時に最低限やっておきたい初期設定"
emoji: "🛠️"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["mac", "m1"]
published: true
---

Mac を買い替えた際にやっておきたい初期設定を忘備録としてまとめていきます．
こういった設定はかなり個人的な好みが出ると思っているので，読者の皆々様はあくまで参考程度に．

基本的な初期設定や，ソフトウェアアップデートは起動時のフローに任せればいいので，ここでは割愛します．

> 実施環境
> ハード: MacBook Air (M2, 2022)
> OS: macOS Ventura 13.1

# システム環境設定

## サウンド

![](https://storage.googleapis.com/zenn-user-upload/feb4c682a804-20221219.png)

- 「起動時にサウンドを再生」をオフにする
  なぜこれがデフォルトでオンなのか未だに謎だと感じているのは私だけではないはず．

## コントロールセンター

メニューバーの表示

![](https://storage.googleapis.com/zenn-user-upload/d6247343e65b-20221219.png)

- Wi-Fi や Bluetooth は自動接続されるものが多いので，私は非表示にしておく派．
  頻繁に切り替えが必要な方は，表示にしておいてもいいと思います．

- 音量は事故防止のために表示にしておく．

![](https://storage.googleapis.com/zenn-user-upload/b08b33623dbc-20221219.png)

- バッテリーの%表示は欲しい人が多いのではなかろうか

![](https://storage.googleapis.com/zenn-user-upload/e454a4efb620-20221219.png)

- 時計はシンプルに便利なのと，「時刻内の":"を点滅」をオンにしておくとフリーズ時に確かめられる．

- Spotlight と Siri は使わないので非表示にしてます．
  Spotlight より，Alfred の方が使いやすい．
  (iPhone の Siri は頻繁に使うけど，Mac の Siri を使おうと思ったこと無いな...)

## Siri と Spotlight

![](https://storage.googleapis.com/zenn-user-upload/1736250a15f6-20221219.png)

使わないので，オフにしておく．
Spotlight の検索候補も全てオフにしておく．

## デスクトップと Dock

![](https://storage.googleapis.com/zenn-user-upload/9f71c98f45a4-20221219.png)

とりあえず初期状態で設定されている Dock のアイコンを全てゴミ箱に向かってドラッグ&ドロップして消す．
Dock から開くのに慣れている方は，よく使うアプリだけ Dock に追加しておくといいと思います．
私は Alfled からコマンドで呼び出すことが多いので，Dock は空にしておく派．

![](https://storage.googleapis.com/zenn-user-upload/883b36c83d19-20221219.png)

- Dock の「画面上の位置」は右にしておく派
  デフォルトの下だと，基本的に横長のディスプレイに対してわざわざ縦方向のスペースを邪魔することになる．
  左だと，コンテンツのメニューバーなどの邪魔になることも．
  右なら，スクロールバーはほぼ使わないし，邪魔になることはあまりない．

- 「自動的に表示/非表示」を ON にして，普段は隠しておく．
  そもそも滅多に使わないし．

- ホットコーナー
  ![](https://storage.googleapis.com/zenn-user-upload/1824decc091b-20221219.png)
  比較的短時間，一時的に席を立つ時などにはマウスカーソルを左上にサッと動かしてスクリーンセーバーを起動させたい．
  ある程度長時間離席しそうなときは，Alfled から「Sleep」を呼び出すようにしている．

## ディスプレイ

![](https://storage.googleapis.com/zenn-user-upload/c49c05f6f183-20221219.png)

内蔵ディスプレイの解像度について「スペースを拡大」させておくことで，より多くのコンテンツを表示できるようにしておく．

## キーボード

![](https://storage.googleapis.com/zenn-user-upload/4e564b6b5ea6-20221219.png)

- キーリピートの速度は，「最速」にしておく．
  連打はだるいので．

- 🌐 キーを押して「絵文字と記号を表示」はデフォルトだったっけ？まあ個人的にこれが慣れている．

- 入力ソースは「Google 日本語入力」をインストール・設定している．
  デフォルトのソースだと，日本語の変換予測が全然違うものになることが多い．Google は比較的優秀．

- 音声入力はうっかり起動すると面倒くさいので切っておく．

ちなみに，入力ソースから「英数」が消せない( - が効かない)ときは，日本語を追加して，入力モードの「英字」にチェックを入れておくと，消せるようになる．
![](https://storage.googleapis.com/zenn-user-upload/2f539d992168-20221219.png)

## トラックパッド

![](https://storage.googleapis.com/zenn-user-upload/977b7ef0aa91-20221219.png)

- 「軌跡の速さ」は最速にして，小さい動きで大きく動作できるようにしておく．すぐに慣れます．
- 「副ボタンのクリック」(いわゆる右クリック)は 2 本指タップ
- 「タップでクリック」をオンにしておくと楽．ポンっと．

![](https://storage.googleapis.com/zenn-user-upload/aa15cb6ccf65-20221219.png)

- 「ナチュラルなスクロール」は Windows 派と感覚が逆？

![](https://storage.googleapis.com/zenn-user-upload/41f16f30491c-20221219.png)

- デスクトップ全体似影響する「フルスクリーンアプリケーション間をスワイプ」「Mission Control」「Launchpad」「デスクトップを表示」は全て 4 本指を使うものを指定．
- 3 本指でドラッグを使いたいから．

# その他

## スクリーンショットの保存場所

![](https://storage.googleapis.com/zenn-user-upload/be72d4f88f35-20221219.png)

「⌘+Shift+5」でクリッピングツールが起動する．
オプション > 保存場所 がデフォルトで(多分)デスクトップになっているので，ピクチャなどにしておく．
あとは今後，「⌘+Shift+3」の全画面キャプチャや「⌘+Shift+4」の部分選択キャプチャも自動的にピクチャに保存される．

## Microsoft Office 系アプリ 規定フォント設定

特に Power Point を例に．
Office 系のアプリはテンプレート内でフォントの指定ができる．PowerPoint のスライドマスターなどはよく使うと思う．
ただし，例えばスライドマスターで規定のフォントをカスタマイズしたい場合，Windows 版だと存在する
`(リボンメニュー)表示 > スライドマスター > フォント > フォントのカスタマイズ` という項目が存在せず，ユーザ定義が出来ない．

![](https://storage.googleapis.com/zenn-user-upload/803cfab81f46-20221219.png)

そこで，以下のような`CustomFontset.xml`ファイルを作成する(ファイル名は任意)．

```xml
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
 <a:fontScheme xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main" name="Custom Font Set">
  <a:majorFont><a:latin typeface="英字見出しフォント"/><a:ea typeface="日本語見出しフォント"/><a:cs typeface=""/></a:majorFont>
  <a:minorFont><a:latin typeface="英字本文フォント"/><a:ea typeface="日本語本文フォント"/><a:cs typeface=""/></a:minorFont>
 </a:fontScheme>
```

typeface に好みのフォント名を指定しておく．個人的にはヒラギノ・Helvetica や Noto Sans などが好み．

これを，`/Users/<<userName>>/Library/Group Containers/UBF8T346G9.Office/User Content.localized/Themes.localized/Theme Fonts/`に保存する．

すると，フォントに「ユーザ定義」としてフォントセットが選択できるようになる．

![](https://storage.googleapis.com/zenn-user-upload/5d40276cf275-20221219.png)

## NAS との接続

### 手動マウント

![](https://storage.googleapis.com/zenn-user-upload/72e1b618cc40-20221219.png)

Finder から，`移動 > サーバへ接続`を開き，
`smb://<<NASのIPアドレス>>/<<共有フォルダ名(任意)>>`を入力して接続する．

### 自動マウント

毎回手動マウントをするのは面倒なので，自動マウントを設定する．
毎回同じ NAS にマウントするのであれば，一番簡単な方法としては`設定 > 一般 > ログイン項目`から，+ を押して NAS のディレクトリを選択しておくと，ログイン時に自動的にマウントされる．

ただし，研究室に設置された NAS など，「自宅では接続しないが研究室では接続する」といった場合，この方法だと自宅では毎回エラーメッセージが表示されることになる．それはダルい．

そこで，接続しているネットワークを判別して，NAS に接続するかどうかを切り替えるスクリプトを準備する．
プリインストールされている「スクリプトエディタ.app」を開いて，以下のようなスクリプトを作成する．

```applescript
repeat 10 times
  set MySSID to do shell script "/System/Library/PrivateFrameworks/Apple80211.framework/Versions/Current/Resources/airport -I"
  if (MySSID contains "NASに接続可能なWi-FiのSSID") then
    tell application "Finder"
      try
        mount volume "smb://<<ユーザ名>>:<<パスワード>>@<<NASのIPアドレス>>/<<共有フォルダ名(任意)>>"
        delay 1
      end try
    end tell
    exit repeat
  else
    delay 3
  end if
end repeat
```

> 3 秒に一度，10 回，NAS に接続可能な Wi-Fi に接続しているかを確認し，接続していれば NAS に接続する．
> 30 秒間で接続できなければ，接続できないと判断して静かに諦めるため，これなら自宅でエラーは出ない．

このスクリプトを app ファイルとして保存する．
`設定 > 一般 > ログイン項目`から，+ を押して，保存した app ファイルを選択・追加すると，起動時にこのスクリプトが動作するようになる．

![](https://storage.googleapis.com/zenn-user-upload/b09ffacfd188-20221219.png)

# おすすめアプリ

## ランチャー

- [Alfred](https://www.alfredapp.com/)

  既に何度も名前を挙げているが，これは必須級．
  アプリを開くのも，ファイルを探すのも，シャットダウンすらも，全部できます．そう，Alfred ならね．

## 入力システム

- [Google 日本語入力](https://www.google.co.jp/ime/)

  予測変換が比較的優秀．論文書く人は，句読点の設定も「，．」に変えておくといい．

- [Paste](https://apps.apple.com/jp/app/paste-clipboard-manager/id967805235)

  クリップボードの履歴を簡単に呼び出せる．
  一気にコピーを続けてから，一気にペーストしていく...という快感は一度体験すると戻れない．
  Clippy という無料アプリもあるが，バグがあるらしいのと，圧倒的に Paste の方が使いやすいと感じている．まあお好みで．

## ブラウザ

- [Side kick](https://join.meetsidekick.com/wnhjg)

  Safari も大分使いやすくなったが，拡張機能慣れしていると Chromium も捨てがたい．
  サイドバーにタブを常駐させたり，ウィンドウ内分割が便利だなと．

- [Brave](https://brave.com/ja/)

  広告ブロックで有名？
  後輩たちはこれで YouTube 見てるらしい．収益に影響しないか...

## 効率化

- [Rectangle](https://rectangleapp.com/)

  ウィンドウのディスプレイ内分割が簡単にできる．Magnet という有料アプリを使っていたが，似たような機能が無料で使えるとボスに紹介された．

- [Fig](https://fig.io/)

  開発者向け．ターミナルのコマンドを予測してくれる．コマンドのタイプミスが減る．

- [AnyDesk](https://anydesk.com/ja)

  遠隔操作用．PC はもちろん，モバイルアプリからも接続できるのは中々便利．
  iPad だけ持ち歩いて，自宅の Mac を遠隔操作することも．

# まとめ

個人的な初期設定の流れをつらつらと書いてみました．
初めて Mac を買った人にも，お役に立てると嬉しいです．
また，よりおすすめな設定や，便利なツールがあればぜひ教えて下さい．
