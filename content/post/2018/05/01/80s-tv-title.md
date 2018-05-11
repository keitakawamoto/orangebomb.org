---
date: 2018-05-01
title: "Photoshopを使った80年代風のタイトル画像の作り方"
description: "ジョークコンテンツ向けの、昔懐かしい80年代「風」のテレビタイトル画像を作成する手順を紹介します。"
tags: ["チュートリアル","Photoshop"]
eyecatch: "/images/post/2018050180s-tv-title/ogp.jpg"
---

![君はあの瞬間を音で覚えているか！チキチキ MCUサントラクイズ 最初で最後の劇伴バトル傑作青春編](/images/post/2018050180s-tv-title/ogp.jpg)

Photoshopを利用した、昔懐かしい80年代風のテレビタイトル画像を作成する手順を紹介します。

<blockquote class="twitter-tweet" data-cards="hidden" data-lang="ja"><p lang="ja" dir="ltr">今度やるコンテンツを80年代のテレビタイトルを観察して再現してみた。国鉄方向幕書体は使ってないと思うし、チキチキはたぶん90年代だけど。 <a href="https://t.co/tuDdBbc3Oo">pic.twitter.com/tuDdBbc3Oo</a></p>&mdash; keita kawamoto (@keita_kawamoto) <a href="https://twitter.com/keita_kawamoto/status/982850743819382786?ref_src=twsrc%5Etfw">2018年4月8日</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

趣味仲間で集まり映画の上映会をしたあとに、ちょっとした出し物をする機会があったためジョーク気味に作成しました。

なので以下が注意内容になります。

- **80年代「風」なので、正確な再現ではないこと**
- 使用したフォントも本来の用途のものではなく、当時おそらくテレビには利用されていなかったフォントであること
- 雰囲気「だけ」であること
- 勝手なイメージから創作している部分があること
- あくまでジョークであること

この点にだけは気をつけてください。僕自身は85年生まれのため、ほとんど90年代以降の記憶しかありません。なので頭の中で生まれたイメージの側面が強いです。

では、具体的な手順を見ていきましょう。

## まずは観察と気づきをメモ

雰囲気を再現するためには、観察が欠かせません。Google検索を使って、それらしい画像を観察していきます。

![80年代 テレビ ロゴ で画像検索した結果](/images/post/2018050180s-tv-title/2018050180s-tv-title_01.png)
![80年代 タイトル で画像検索した結果](/images/post/2018050180s-tv-title/2018050180s-tv-title_02.png)

上記以外にもいろいろな観察を繰り返した結果、以下を気づきとしてメモしました。

- 実写以外では、アニメ作品中心に背景はベタ塗りであるケースが多い
  - セル画の性質か配信などそれ以外の理由か、最終的に彩度が低い
  - アニメ以外では彩度が高いものもある（高すぎるくらいに）
- 言い回しにユーモアさがあることが多い？
- ビックリマークはナナメであることが多い
- ブラウン管の性質か、画像が滲んでいる・ぼけている

80年代当時、アニメはセル画を使われており、テレビはブラウン管テレビが主流。観察でいろいろと発見。あくまでジョークコンテンツであるため **「観察」にとどめ、歴史的背景や事情の調査は行いませんでした。**

## 観察結果をもとに文言のチョイスとレイアウト

会場の参加者が楽しめるよう、ユーモアさが欲しい。観察して得た80年代の言い回しを参考に、ちょっと盛った文言を用意。

今回のコンテンツが「MCUサントラクイズ」というコンテンツですが、その前後に本来不要である文言を追加して雰囲気を出すことにしました。「君はあの瞬間を音で覚えているか！チキチキ MCUサントラクイズ 最初で最後の劇伴バトル傑作青春編」。このへんはだいぶ僕のイメージから生成された部分ですが、「問いかけ」「傑作」「青春編」という部分が80年代っぽいかな...と。お気に入りなのは、「最初で最後」と言っているのに「青春編」と付いていて辻褄が合っていないところです。ここは80年代関係なく、意味不明さの演出です。ほら、お楽しみコンテンツなので…。

ビックリマークをナナメにし、フォントもそれらしいものを選びました。国鉄（現在のJR）がまだ存在していた時代はちょうど80年代も含まれているため、国鉄方向幕書体を選択。配色も、観察時に集めたサンプルを参考に近い組み合わせを作りました。

## 一番重要な雰囲気加工

レイアウトした段階では、色が綺麗すぎます。これでは雰囲気が出ません。ここからは雰囲気を出す加工を行っていきます。
まず、**すべてのレイヤーを結合し、一枚の画像にします。**（バックアップとして必ず未結合のレイヤーデータは残してください。事前に.psdファイルを複製するか、同じファイル上でレイヤーをディレクトリにまとめ、非表示にしておくでもOKです）

![](/images/post/2018050180s-tv-title/2018050180s-tv-title_03.png)

### ブラウン管の再現：ぼかし小

現在主流の液晶テレビとは異なり、当時のブラウン管テレビでは「滲み」が大きい印象です（これはブラウン管の性質か、ブラウン管に伝わる信号の性質なのか詳しくは未調査です）。ここではその印象に従い、再現していきます。

再現するために、「ぼかし」を使います。メニューの「フィルタ」->「ぼかし」->「ぼかし（ガウス）」を選択し、半径 `1.3pixel` ほど適用します。

![](/images/post/2018050180s-tv-title/2018050180s-tv-title_04.png)

### ブラウン管の再現：ぼかし大->ソフトライト->半透過

続けてブラウン管の発光を再現。レイヤーを複製し、オリジナルの上で大きくぼかし、ソフトライトをかけ発光しているように見えるようにし、発光具合の調整のため半透明にします。

![](/images/post/2018050180s-tv-title/2018050180s-tv-title_05.png)

複製し、メニューの「フィルタ」->「ぼかし」->「ぼかし（ガウス）」を選択し、半径 `6.0pixel` ほどのぼかしをかけます。

![](/images/post/2018050180s-tv-title/2018050180s-tv-title_06.png)

そのまま、ぼかしたレイヤーに「ソフトライト」を適用します。

![](/images/post/2018050180s-tv-title/2018050180s-tv-title_07.png)

不透明度を50%にし半透明にします。

![](/images/post/2018050180s-tv-title/2018050180s-tv-title_08.png)

次の工程のために、複製したレイヤーはオリジナルと結合してしまいましょう。

### 当時の傾向の再現：彩度を大幅に低下させる

最後の仕上げに観察結果にある「彩度の低さ」を再現。

![](/images/post/2018050180s-tv-title/2018050180s-tv-title_09.png)

メニューの「イメージ」->「色調補正」->「色相・彩度」を選択し、「彩度」を `-40` ほどにします。

### さらに2010年代ならではの加工

今現在、正しく当時の再現をできるのは、録画データだけです。しかし、懐かしい動画や画像に関して、多くの人は録画データではなく、ネット上で出会うのではないでしょうか。それらのデータは往々にして、劣化しています。なので、**あえて劣化させることで、2010年代に出会う懐かしい画像というふうに再現します。**

jpegの質を5%に低下させるのは僕も初めてでした。

![](/images/post/2018050180s-tv-title/2018050180s-tv-title_10.png)

メニューの「ファイル」->「書き出し」->「Web用に保存（従来）」を選択し、形式はJPEG、画質を `5` にします。これで画質の劣化が再現できます。あとは「保存」をクリックし、保存しましょう。

これで完成。

## まとめ

工程をまとめると、以下のようになります。

- 観察し、それらしい言い回しを用意する
- ビックリマークはナナメに
- 配色についてもよく観察して再現
- ブラウン管テレビで映し出した状態を再現するためにあえてぼかす
- 最終的に彩度を落とす
- さらに、jpegの質を5%に落とし現代で出会う状態にする

イベントのお楽しみコンテンツを作成するときなど、試してみてください。