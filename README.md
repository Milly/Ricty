# おことわり

本リポジトリは [Ricty](http://www.rs.tus.ac.jp/yyusa/ricty.html) をライセンス(2 clause BSD license)に従って適切に fork し再頒布するものです。本リポジトリに関するいかなる責任もライセンスに従います。

# プログラミング用フォント Ricty

[![Ricty screenshot of GNU Emacs on Ubuntu](/screenshots/ricty_screenshot_emacs_thumbnail.png?raw=true)](/screenshots/ricty_screenshot_emacs.png?raw=true)
[![Ricty screenshot of GVim on Ubuntu](/screenshots/ricty_screenshot_gvim_thumbnail.png?raw=true)](/screenshots/ricty_screenshot_gvim.png?raw=true)

Ricty (リクティ) は Linux 環境での研究・開発に適したフリーなプログラミング用 TrueType フォントです。
Emacs や Vim を用いた C、C++、FORTRAN、Python、Perl、Ruby、AWK、sed、シェルスクリプト、LaTeX などのコーディングにおける使用を想定しています。
以下の 2 つの等幅フォントの合成、および、プログラミング用フォントとしてのいくつかのチューニングを行う生成スクリプトの配布を行なっています。

* [Inconsolata](http://levien.com/type/myfonts/inconsolata.html): 「[Top 10 Programming Fonts](http://hivelogic.com/articles/top-10-programming-fonts/)」や「[プログラミング時に最適なフォント『Inconsolata』](http://weboo-returns.com/blog/inconsolata-as-a-programming-font/)」などで高い評価を受けているサンセリフ体等幅欧文フォント
* [Migu 1M](http://mix-mplus-ipa.osdn.jp/): [M+ 1M](http://mplus-fonts.osdn.jp/) と [IPA ゴシック](http://ipafont.ipa.go.jp/) の合成フォント (旧称 M+1VM+IPAG circle/M+2VM+IPAG circle) であり、「[Windows でプログラミングに最適なフォントを探す](http://blog.blueblack.net/item_121)」などで高い評価を受けているゴシック体等幅和文フォント

Inconsolata 作者の Raph Levien 氏、Migu 1M 作者の itouhiro 氏、M+ 1M 作者の coz 氏、IPA ゴシックのベースとされている [TB ゴシック](http://www.typebank.co.jp/fonts/gothic/tbg.html) 作者の林隆男氏、[Ricty 生成スクリプト](http://www.rs.tus.ac.jp/yyusa/ricty.html) 作者の遊佐泰紀氏のイニシャルから **Ricty** と命名されました 。

# ハイライト

* ラテン文字には Inconsolata が適用されます。
* それ以外の文字には Migu 1M が適用されます。M+ M Type-1 の美しいグリフと IPA ゴシックの JIS 第四水準漢字、そして、Migu 1M の判読性の高い和文文字 (半濁音など) が使用できます。
* 半角文字と全角文字の横幅の比が 1:2 に調整されています。
* 全角スペースが可視化されます。
* いくつかの全角グリフが対応する半角グリフと差別化されています。
* en ダッシュ、em ダッシュが破断線のようになります (LaTeX での入力ミス防止のため)。

# 派生フォント Ricty Discord

Ricty では、調和・統一感の維持のため、プログラミング用フォントのコアである Inconsolata 由来の ASCII 文字に手を入れないようにしています。一方、Discord (不協和音) 版は、判読性向上のため、調和・統一感を犠牲にして以下の ASCII 文字に手を入れた Ricty の派生フォントです。

* `"`: ダブルクオートを拡大する。
* `'`: クオートを拡大する。
* `*`: アスタリスクをやや下方に移動する。
* `+`: プラスをやや下方に移動する。
* `,`: コンマを拡大する。
* `-`: ハイフンをやや下方に移動する。
* `.`: ピリオドを拡大する。
* `0`: 0 をドットゼロ (Inconsolata の不使用グリフ) にする。
* `7`: 7 にクロスバーを付ける。
* `:`: コロンを拡大する。
* `;`: セミコロンを拡大する。
* `< および >`: 不等号をやや下方に移動する。
* `=`: 等号をやや下方に移動する。
* `D`: D を Eth にする (D にクロスバーを付ける)。
* `Z`: Z にクロスバーを付ける。
* `^`: サーカムフレックスを拡大する。
* <code>\`</code>: グレイブを拡大する。
* `l`: l の左下のセリフを切り落とす。
* `r`: r をセリフ体 (Inconsolata の不使用グリフ) にする。
* `z`: z にクロスバーを付ける。
* `|`: 縦線を破断線にする。
* `~`: チルダを上方に移動する。

# ライセンス

* Ricty 生成スクリプトは二条項 BSD ライセンスに従うものとします。
* Ricty 生成スクリプトにより生成されたスクリプトは [SIL Open Font License (OFL) Version 1.1](http://scripts.sil.org/ofl) および [IPA Font License Agreement v1.0](http://ipafont.ipa.go.jp/ipa_font_license_v1.html) に従うものとします。
  特に、OFL 1.1 section 5 に従い、生成されたフォントの再配布は禁止とします

# スクリプト

* `ricty_generator.sh`: Ricty 生成スクリプト
* `os2version_reviser.sh`: 生成されたフォントの文字間隔が不自然に大きくなったときにフォントを修正するスクリプト

# 生成方法

1. FontForge のインストール
2. Inconsolata の入手
3. Migu 1M の入手
4. Ricty の生成
5. Ricty のインストール

## FontForge のインストール

Debian/Ubuntu

    # apt-get install fontforge

Fedora/CentOS

    # yum install fontforge

OpenSUSE

    # zypper install fontforge

その他の Linux

[FontForge Open Source Font Editor](https://fontforge.github.io/) より入手します。

## Inconsolata の入手

[Google Fonts Inconsolata](https://fonts.google.com/specimen/Inconsolata) (リリース) もしくは [GitHub google/fonts/ofl/inconsolata](https://github.com/google/fonts/tree/master/ofl/inconsolata) (アップストリーム) から Inconsolata (2.000 以降) を入手します。

## Migu 1M の入手

[M+ と IPA の合成フォント](http://mix-mplus-ipa.osdn.jp/) から Migu 1M (2015.0712 以降) を入手します。

## Ricty の生成

Ricty 生成スクリプトを以下のように実行します。

    % ./ricty_generator.sh auto

もしくは

    % ./ricty_generator.sh Inconsolata-{Regular,Bold}.ttf migu-1m-{regular,bold}.ttf

## Ricty のインストール

    % cp -f Ricty*.ttf ~/.fonts/
    % fc-cache -vf

# Ricty 生成スクリプトのオプション

## 使用法

    ricty_generator.sh [オプション] auto
    ricty_generator.sh [オプション] Inconsolata-{Regular,Bold}.ttf migu-1m-{regular,bold}.ttf

## オプション

* `-h`: ヘルプを表示する。
* `-V`: バージョン番号を表示する。
* `-f /path/to/fontforge`: fontforge コマンドのパスを指定する。
* `-v`: fontforge の警告メッセージを表示する。
* `-l`: 生成の過程で生じる中間ファイルを削除せずに残す。
* `-n string`: フォントファミリ名を「Ricty」ではなく「Ricty ○○○」として生成する。
* `-w`: 行間を広くする。
* `-W`: 行間をかなり広くする。
* `-Z unicode`: 他のグリフのコピーすることで全角スペースを可視化する (たとえば `-Z 2668` とすると、全角スペースが &#x2668; になる)。
* `-z`: 全角スペースを可視化しない。
* `-a`: Inconsolata のグリフを優先し、Ambiguous 文字を全角化しない。
* `-s`: Migu 1M のグリフを縮小しない (`-w` オプションとの併用を推奨)。
* `-d characters`: Ricty Discord で Discord 化しない文字を指定する (たとえば "7DZz"、"\"\`")。

# エディタの設定

Emacs

    (set-face-attribute 'default nil
                        :family "Ricty Discord"
                        :height 120)
    (set-fontset-font (frame-parameter nil 'font)
                      'japanese-jisx0208
                      (cons "Ricty Discord" "iso10646-1"))
    (set-fontset-font (frame-parameter nil 'font)
                      'japanese-jisx0212
                      (cons "Ricty Discord" "iso10646-1"))
    (set-fontset-font (frame-parameter nil 'font)
                      'katakana-jisx0201
                      (cons "Ricty Discord" "iso10646-1"))

GVim (Linux)

    set guifont=Ricty\ Discord\ 12
    set guifontwide=Ricty\ Discord\ 12

GVim (Mac OS X/Windows)

    set guifont=Ricty\ Discord:h12
    set guifontwide=Ricty\ Discord:h12

# 既知の問題

* Ricty Discord の `0`、`r` が異なるグリフになることがあります。
  * Inconsolata や Migu 1M のバージョンが合っていないことが原因です。
* Gnome-terminal のフォントに Ricty を設定できないことがあります。
  * `gconf-editor` などで `~/.gconf/apps/gnome-terminal/profiles/Default/%gconf.xml` の `font` を直接編集します。
* 半角文字と全角文字の横幅比が 1:2 にならないことがあります。
  * ピクセル値 (px) が偶数でないとき、どのフォントでも起こりうる問題です。一般的な 96 DPI のフォントレンダリングでは 9 pt、10.5 pt、12 pt、13.5 pt、15 pt など、1.5 の倍数を指定すると 1:2 で表示されます。

# メモ

* Cocoa Emacs でフレーム幅が意図した幅の倍になってしまうときは、本末転倒気味ですが、`misc/ricty_ascii_extractor.pe` で ASCII 文字のみを分離したフォントを生成する方法が有効です。
* `misc/ricty_greek_regenerator.pe` でアクセント付きギリシア文字を全角幅にすることができます。
  現時点ではギリシア文字拡張グリフには対応していません。

# バージョン

## 4.1.1 (2017 年 12 月 3 日)

* 斜体生成スクリプトの Ricty 生成スクリプトへの統合

## 4.1.0 (2016 年 12 月 30 日)

* Ricty Discord 生成スクリプトの Ricty 生成スクリプトへの統合
* Inconsolata 2.000 対応

## 4.0.1 (2016 年 1 月 28 日)

* ヒンティング情報の付与

## 4.0.0 (2015 年 12 月 31 日)

* Inconsolata.otf から Inconsolata-Regular/Bold.ttf への切り替え
* Inconsolata をボールド化するオプションの廃止

## 3.2.4 (2014 年 12 月 7 日)

* ライセンス変更 (public domain → 二条項 BSD)

## 3.2.3 (2014 年 5 月 4 日)

* ASCII グリフのボールド体の太さの変更 (以前の太さにするときは `-b`)

## 3.2.2 (2013 年 6 月 9 日)

* 全角括弧を半角括弧と差別化

## 3.2.1 (2012 年 11 月 6 日)

* M+ FONTS LICENSE 記述の除去 (Migu 1M の更新に追従)
* いくつかの環境で等幅でなくなる問題に対処
* em ダッシュ処理の修正

## 3.2.0 (2012 年 4 月 16 日)

* 行間の調整
* コマンドラインオプションの追加

## 3.1.3 (2011 年 11 月 24 日)

* Ricty Discord のコマンドラインオプション
* コマンドラインオプションの追加

## 3.1.2 (2011 年 10 月 3 日)

* Migu 20111002 に同期 (後方互換を担保せず)
* コマンドラインオプションの追加

## 3.1.1 (2011 年 7 月 8 日)

* コマンドラインオプションの追加

## 3.1.0 (2011 年 6 月 19 日)

* Mac OS X で Regular と Bold が異なる高さで表示される問題に対処

## 3.0.2 (2011 年 6 月 2 日)

* 生成スクリプトへの auto オプションの追加

## 3.0.1 (2011 年 5 月 20 日)


## 3.0.0 (2011 年 5 月 17 日)

* 生成スクリプトの配布開始
* TrueType フォントの配布中止

# Authors

* [遊佐泰紀 (Yasunori Yusa)](http://www.rs.tus.ac.jp/yyusa/index.html.ja): [Ricty 生成スクリプト](http://www.rs.tus.ac.jp/yyusa/ricty.html)

*Please do not ask to original author about this repository.*

# Contributors

* Raph Levien: [Inconsolata](http://levien.com/type/myfonts/inconsolata.html)
* itouhiro: [Migu 1M](http://mix-mplus-ipa.osdn.jp/)
* coz: [M+ 1M](http://mplus-fonts.osdn.jp/)
* 林隆男: [TB ゴシック](http://www.typebank.co.jp/fonts/gothic/tbg.html)
