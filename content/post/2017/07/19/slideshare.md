+++
date = "2017-07-19T05:34:18+09:00"
title = "アクセシブルにするならSlideShareを選ぶべき？SlideShareへのアップロード方法"
description = "Keynoteなどでスライドを作成し、スライドのSNSへアップロードし、シェアする。多くの人が行なっているこの行動、場合によってはスライドの中身にアクセスできないことがあるという事実を知った。そこで、そのようなことが起こらないようにアクセシブルなスライドにするにはどうすればよいのか？という部分に関し調査・検証を行なった。"
tags = ["アクセシビリティ"]
eyecatch = "/images/ogp.png"
+++

Keynoteなどでスライドを作成し、スライドのSNSへアップロードし、シェアする。多くの人が行なっているこの行動、場合によってはスライドの中身にアクセスできないことがあるという事実を知った。そこで、そのようなことが起こらないようにアクセシブルなスライドにするにはどうすればよいのか？という部分に関し調査・検証を行なったので記録する。

- [アクセシブルとは？](#170719SlideShare-1)
- [アクセシビリティと、スライドのアップロードに関する事情](#170719SlideShare-2)
  - [SpeakerDeckでは情報（スライドの内容）にアクセスできない](#170719SlideShare-2-1)
  - [SlideShareの場合は中身を読みテキストとしてWebページ上に表示される](#170719SlideShare-2-2)
- [Keynoteで作ったスライドをSlideShareにアップロードする手順](#170719SlideShare-3)
- [Adobe Acrobut Pro を使わない場合](#170719SlideShare-4)
- [完璧は難しい。「割り切ること」も重要なこと](#170719SlideShare-5)
- [余談１.SlideShareにアップロードしたスライドを削除する方法](#170719SlideShare-6)
- [余談２.一応ある？SpeakerDeckのスライドをスクリーンリーダーで読む方法](#170719SlideShare-7)
- [所感](#170719SlideShare-8)
- [【7/20追記】Acrobutでのトリミングなしで済む方法](#170719SlideShare-9)

<a name="170719SlideShare-1"></a>
## アクセシブルとは？

まずは `アクセシブル` という単語について。

> アクセシブルデザインは、高齢者・障害のある人々の利便性を配慮しつつ、健常者の利便性も確保することを目的として、従来の設計を高齢者や障害のある人々のニーズに合わせ拡張することによって、製品、サービス、建物などがそのまま利用できる潜在顧客数を最大限に増やすための設計ということができます。これにより、ビジネス拡大の効果を得ることが可能になりますが、ビジネスを最優先させるのではなく、高齢者や障害のある人々の利便性を高めることが主たるねらいです。
> アクセシブルデザインは、ISOにおける ガイド71 の議論において、高齢者・障害のある人々が健常者と同様に社会システムにアクセスできる言葉として定義されています。

出典：[共用品推進機構 - アクセシブルデザイン関連JIS・基本規格](http://www.kyoyohin.org/ja/research/japan/ad_jis_1.php)

このように書かれることが多いが、僕は **どのような条件であろうと誰しもが同じようにコンテンツにアクセスすることができること** という認識をしている。僕にとって「障害者対応」という言葉は本質的ではなく、目が見えなかったとしても、耳が聞こえなかったとしても、テクノロジーを利用すれば健常者と同じようにコンテンツを参照できるのだから、当然そうあるべきである、というもの。（似て非なるもの、というか。やっていることは同じかもしれないが、捉え方の問題）

<a name="170719SlideShare-2"></a>
## アクセシビリティと、スライドのアップロードに関する事情

ここからは、スライドとアクセシビリティの関係について。

<a name="170719SlideShare-2-1"></a>
### （１）SpeakerDeckでは情報（スライドの内容）にアクセスできない

以前、スライドを[SpeakerDeck](https://speakerdeck.com/)にて公開した時に、スクリーンリーダーユーザーである [@ma10](https://twitter.com/ma10?ref_src=twsrc%5Etfw&ref_url=http%3A%2F%2Flocalhost%3A1313%2Fblog%2F2017%2F07%2F19%2Fslideshare%2F) さんが以下のようなツイートをなされていた。

<blockquote class="twitter-tweet" data-lang="ja"><p lang="ja" dir="ltr">んー、Speaker Deckかあ。。。良いまとめだというツイートを見かけたけど、内容確認できないので紹介は断念。 <a href="https://t.co/oFzTw8NZ6W">https://t.co/oFzTw8NZ6W</a></p>&mdash; Max/なかね まさふみ (@ma10) <a href="https://twitter.com/ma10/status/803519996663992320">2016年11月29日</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

驚いていると、 [@magi1125](https://twitter.com/magi1125) さんからアドバイスのメッセージをいただいた。

- SpeakerDeckはスライドを画像として表示するのみである
- テキスト情報として内容にアクセスすることができない

なんてこった...

<a name="170719SlideShare-2-2"></a>
### （２）SlideShareの場合は中身を読みテキストとしてWebページ上に表示される

SpeakerDeckに関しショックを受けたところで、「SlideShareならばその問題が起こらない」という情報も得た。

- 文字を画像にしない等、適切な方法でSlideShareにアップロードすればスライド内のテキストを抜き出してくれるため、スクリーンリーダーユーザーでも内容を把握することができる
- スクリーンリーダーで読み上げることが可能＝視覚以外でアクセスが可能

しかし、SpeakerDeckだと起こる困ることは起こらなくても、SlideShareにはSlideShareならではの困ることがあるのであった。
僕はスライド作成には[Keynote](https://www.apple.com/jp/keynote/)を使っている。困る問題とは、Keynoteバージョン6以降で生成したPDFをSlideShareにアップロードすると、作ったスライド上からテキスト部分がすべて表示されなくなってしまう、という問題だ。実際はそこにあるけどただ映らないのみ。スライド外にテキスト出力はされていた。
今回、どのようにすれば問題なくSlideShareにアップロードすることができるのかを調べた。

<a name="170719SlideShare-3"></a>
## Keynoteで作ったスライドをSlideShareにアップロードする手順

そのうちSlideShare側がバグを解消してくれるのでは？という点に関して。[KeynoteのスライドをSlideShareにアップロードすると日本語が表示されない問題 - Qiita / 公式の回答 ](http://qiita.com/yasulab/items/49511c27179be454d568#%E5%85%AC%E5%BC%8F%E3%81%AE%E5%9B%9E%E7%AD%94) によると、残念ながら前述の文字が消える問題を解決する対応は時間がかかるようで、こちら側が頑張らないといけない…
 [@magi1125](https://twitter.com/magi1125) さんがツイートしていた解決策をベースに進める。

<blockquote class="twitter-tweet" data-lang="ja"><p lang="ja" dir="ltr">FAQぽいので。KeynoteからSlideShare用に(日本語表示されてテキストも抽出される)PDFを出力する方法。印刷メニューからカスタムサイズで160/90mm or 160/120mmに設定して「AcrobatでPDF保存」的なのを選ぶ。リンクは死ぬけどあとは大丈夫。</p>&mdash; Rikiya Ihara (@magi1125) <a href="https://twitter.com/magi1125/status/769361345892364288">2016年8月27日</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

この検証では以下のバージョンを使用する。

- `Keynote バージョン7.2（4582）`
- `Adobe Acrobut Pro DC バージョン 2017.009.20058`

結論から言うと、

> カスタムサイズで160/90mm or 160/120mmに設定して「AcrobatでPDF保存」的なのを選ぶ。

いろいろ試行錯誤したもののここがどうしても実現できなかった。
今回行なった手段は、

- Adobe Acrobat Proを用意（少なくとも2016年8月時点での最新版が必要？）
- Keynote `ファイル` &#8594; `プリント` &#8594; 形式で `Save as Adobe PDF` を選択
- Adobe PDFの設定は `標準` を選択・保存
- Adobe Acrobat Proで展開、無用な余白をトリミング・保存
- SlideShareへアップロード

という流れ。画面を見つつ解説すると

![keynoteの画面](/images/post/20170719slideshare/20170719slideshare_1.png)

まずはKeynoteメニューの `ファイル` &#8594; `プリント`。

<img src="/images/post/20170719slideshare/20170719slideshare_2.png" width="456" alt="keynoteメニュー">

左下にある `PDF` を `Save as Adobe PDF` に変更する。Adobe PDFの設定は `標準` を選択。

![プリント画面](/images/post/20170719slideshare/20170719slideshare_3.png)

Adobe Acrobat Proで先ほどのファイルを開き、右側の検索窓から `トリミング` と検索（どこにあるかわからなかったので検索した方が早かった）。その後 `ページをトリミング` を選択。

![Adobe Acrobat Proの画面](/images/post/20170719slideshare/20170719slideshare_4.png)

トリミング範囲を指定した後、詳細画面が表示される。16:9のスライド場合、 `余白の制御` は上下 `21ミリ` ほどで綺麗になった。ページ範囲の項目では `すべて` を選択。これで全ページに同じトリミングが適用される。その後保存すると、PDFの完成。

![トリミング詳細画面](/images/post/20170719slideshare/20170719slideshare_5.png)

完成したPDFをSlideShareへアップロードすると、文字も消えておらず無用な余白もない綺麗な状態かつアクセシブルなスライドにできる。
次に、Adobe Acrobut Proが手に入らず、使わないでやる必要がある場合の方法を記載する。

<a name="170719SlideShare-4"></a>
## Adobe Acrobut Pro を使わない場合

Adobe Acrobut Proを使わず、SlideShareへスライドをアップロードするにはどうするとよいか？

### （１）Keynoteの場合（文字が消えるバグの回避法）

- Keynoteの書き出しの `イメージ` を選び、すべてのページを画像で書き出した後、全ページにひとつずつ画像をかぶせ、通常のPDFで書き出し、アップロードする
  - 余白問題は解消され、スクリーンリーダーでも読める状態
  - しかし画像だと多少文字がギザる、大きな手間がかかると言うデメリット
  - とてもナンセンスな印象
- ヒラギノなどOS Xの標準フォント以外のフォントを使う（ [KeynoteのスライドをSlideShareにアップロードすると日本語が表示されない問題](http://qiita.com/yasulab/items/49511c27179be454d568#%E6%A1%885-os-x%E3%81%AE%E6%A8%99%E6%BA%96%E3%83%95%E3%82%A9%E3%83%B3%E3%83%88-%E3%83%92%E3%83%A9%E3%82%AE%E3%83%8E%E3%81%AA%E3%81%A9-%E4%BB%A5%E5%A4%96%E3%81%AE%E3%83%95%E3%82%A9%E3%83%B3%E3%83%88%E3%82%92%E4%BD%BF%E3%81%86) より ）
- 文字が消える事象が起こるKeynote6より前のKeynote5以前を使う？（手に入るかはわからないが…）

### （２）Keynote以外の場合（おそらく文字が消えるバグは起こらない）

- Googleスライド
- その他スライド作成アプリケーション

などの手段がある。

<a name="170719SlideShare-5"></a>
## 完璧は難しい。「割り切ること」も重要なこと

今回の件を調べるにあたり、SlideShareにアップロードできたと言っても、「それだけで完全にアクセシブルなのか？」という疑問を持っていた。

- SlideShareでは自動出力されたテキスト情報は改行や段落がなくなるので認識しにくいと思うが、テキスト情報だけで読む人は、どのように脳内補正している？
- テキスト情報の内容は重複してもいいのか？（差分表現で、差分箇所以外は同じものを何度も掲載することになる）
- 図解に関しどのようにテキスト化すればいい？
- 自分一人ならすごく気にすればこれらを解決できるかもしれないが、人に続いてもらえるようなフレームワーク化とか無理では…

などということについて頭を抱えおり、ちょうどそのころ参加した勉強会 [!important #04 -特盛！アクセシビリティスペシャル-](https://important.doorkeeper.jp/events/58580) でお会いした [@magi1125](https://twitter.com/magi1125) さんにこのことを相談させていただいた。すると、

- `全く読むことができない` という状況から `読めるようになった` それでけでも大きい変化だと割り切ることも大事
- `完璧` は難しいこと。そしてスライドの作成者次第な部分が大きすぎる

という回答をいただいた。割り切るという視点が欠けていたため、目が覚めたようだった。

<a name="170719SlideShare-6"></a>
## 余談１.SlideShareにアップロードしたスライドを削除する方法

テストで文字が消えてしまったスライドを削除しようとしたところ、消すまでにかなり迷った。（バグなのか、  `Edit` &#8594;  `Delete presentation` では消えないことがあった）
最終的には [SlideShare ファイルを削除する | LinkedInヘルプ](https://www.linkedin.com/help/linkedin/answer/55028/slideshare-?lang=ja) にたどり着くことで解消できた。

> - SlideShare にサインイン
> - 右上のプロフィール写真にマウスをポイントし、 `My uploads` を選択
> - 削除するプレゼンテーションの左上のチェックボックスをオンに
> - `削除` をクリック

とのこと。

<a name="170719SlideShare-7"></a>
## 余談２.一応ある？SpeakerDeckのスライドをスクリーンリーダーで読む方法

<blockquote class="twitter-tweet" data-lang="ja"><p lang="ja" dir="ltr">そういえば、SpeakerDeckだと、SlideShareみたいにテキストの書き出しをしてくれませんが、<a href="https://t.co/xRxKpHgSw7">https://t.co/xRxKpHgSw7</a>というサイトだとテキストの書き出しつけてくれるんですよね。他サイトのスライドをいただきマンモスって感じなのが気にはなりますが。</p>&mdash; まえぽん (@maepon) <a href="https://twitter.com/maepon/status/874119273949483010">2017年6月12日</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

こういう裏技も一応あるようだ。 [SSSSLIDE](http://sssslide.com)...スライド集約サイト？

<a name="170719SlideShare-8"></a>
## 所感

アクセシブルにするためにこのような努力が必要である今の状況には不満がある。
Keynoteの文字が消える問題の解決対応がまだ先になりそうなSlideShareも、テキストデータが出力されないためにスクリーンリーダーでは読むことができない状態であるSpeakerDeckも。ただPDFで出力してアップロードさえすればスライドの内容になんの無理もなく誰もがアクセスできるようになる未来を望んでいる。
…と言いつつ、自分の携わっているものがすべてアクセシブルかと言われると違う。もっと頑張らないといけない。もっと勉強と実験を繰り返し、関わるものを可能な限りアクセシブルにしなければ。

そして、この件で相談に乗っていただいた [@magi1125](https://twitter.com/magi1125) さんには本当に感謝しかありません。ありがとうございます！

<a name="170719SlideShare-9"></a>
## 【7/20追記】Acrobutでのトリミングなしで済む方法

<blockquote class="twitter-tweet" data-lang="ja"><p lang="ja" dir="ltr">記事みてわかりました。Keynoteでcmd+p➞[詳細を表示]➞ダイアログ右t中段のKeynoteと書かれたセレクトボックスで[ページ属性]を選択➞紙のサイズでカスタムサイズ➞90mm,160mmとしてください。これで余白が消えます。あとはSave as Adobe PDF!</p>&mdash; Rikiya Ihara (@magi1125) <a href="https://twitter.com/magi1125/status/887654118201806848">2017年7月19日</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

この記事を公開したところ、[@magi1125](https://twitter.com/magi1125) さんからフィードバックをいただけた。

> > カスタムサイズで160/90mm or 160/120mmに設定して「AcrobatでPDF保存」的なのを選ぶ。
>
> いろいろ試行錯誤したもののここがどうしても実現できなかった。

わからなかったこの部分の解決方法を教えていただけた...！圧倒的感謝。（僕は印刷画面UIが苦手っぽい。 `ページ属性` という項目の意味が理解できなかった）

Keynoteの以下の `プリント` の設定画面のところで下部にある `詳細を表示` から進む。

![プリント画面](/images/post/20170719slideshare/20170719slideshare_6.png)

ダイアログ中段の `Keynote` と書かれたセレクトボックスで `ページ属性` を選択。

![プリント詳細画面](/images/post/20170719slideshare/20170719slideshare_7.png)
<img src="/images/post/20170719slideshare/20170719slideshare_8.png" width="269" alt="ダイアログ中段のセレクトボックス">

`用紙サイズ`のセレクトボックスで`A4` になっているところを `カスタムサイズを管理...` に変更。

![用紙サイズの変更](/images/post/20170719slideshare/20170719slideshare_9.png)

新しいサイズを設定できるので、左側の `+` から新規サイズを追加する。
`90mm` `160mm` と指定すればOK。 （4:3のスライドの場合 `160mm` `120mm` と指定すればよい）

![用紙サイズの変更画面で専用のサイズを指定](/images/post/20170719slideshare/20170719slideshare_10.png)

こうすれば、Acrobatでトリミングせずとも余白がない状態で出力できる。形式は前述の通り `Save as Adobe PDF` ！ そのあとはSlideShareアップロードすればOK。
