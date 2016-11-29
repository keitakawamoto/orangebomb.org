+++
date = "2016-11-29T13:51:11+09:00"
title = "目が見えない状態を想定したUI設計"
tags = ["インターフェイス/インタラクション","アクセシビリティ"]
+++

視覚がない、弱い人はどのようにサイトを利用しているのか、使っているのはどんなインターフェイスなのか。ずっと気になっていたというのもあり、「目が見えない状態を想定したUI設計」という内容で、主催した勉強会 [Design Casual Talks #1](https://dct.connpass.com/event/36278/) で発表をしました。

インターフェイスとは目で見えるものだけではなく、音声だけで構成されるインターフェイスもある。では僕らがページを作るとき、具体的にどうすればいいのか？

## 構成とスライド

- 調べるきっかけ
- 「知らない」問題
- 視覚障害者の概要
- 弱視者の見え方の例
- 視覚障害者の割合・補足
- ネットの利用方法と、見え方とそれぞれのニーズ
- スクリーンリーダー？
- 視覚なしで得られる情報はどんなものなのか試す
- 文字列の構造化の必要性
- jsなどのリッチコンテンツに対応できない問題
- WAI-ARIA
- 所感
- まとめ：目が見えない状態を想定したUI設計

<script async class="speakerdeck-embed" data-id="39edc3f5462245518ae1ed06e0d1898d" data-ratio="1.77777777777778" src="//speakerdeck.com/assets/embed.js"></script>

## 出典・参考文献

すべて2016年9月時点（スライド作成時）の情報を参考にしました。


- [視覚障害者 - Wikipedia](https://ja.wikipedia.org/wiki/視覚障害者)
- [視覚障害とは - 公益財団法人 関西盲導犬協会](http://www.kansai-guidedog.jp/knowledge/disease/)
- [視覚障害とは - 高知県立盲学校](http://www.kochinet.ed.jp/mo-s/mt/post-28.html)
- [２－１　視覚障害とは - 秋田県立視覚支援学校](http://kagayaki.akita-pref.ed.jp/shikaku-s/detail.html?id=361&category_id=61)
- [厚生労働省 統計情報・白書 平成18年身体障害児・者実態調査結果](http://www.mhlw.go.jp/toukei/list/108-1b.html)
- [視覚障害者 全盲者と弱視者の割合 統計みたいなものが欲しい... - Yahoo!知恵袋](http://detail.chiebukuro.yahoo.co.jp/qa/question_detail/q1049785990)
- [WAI-ARIA の基礎知識 — Website Usability Info](http://website-usability.info/2014/04/entry_140415.html)
- [WAI-ARIA | HTMLリファレンス](http://www.webcreativepark.net/html/wai-aria/)


## まとめ終えて

イベントを前に、とにかくアクセシビリティに関する多くの情報を得たくて、[コーディングWebアクセシビリティ](https://www.amazon.co.jp/%E3%82%B3%E3%83%BC%E3%83%87%E3%82%A3%E3%83%B3%E3%82%B0Web%E3%82%A2%E3%82%AF%E3%82%BB%E3%82%B7%E3%83%93%E3%83%AA%E3%83%86%E3%82%A3-WAI-ARIA%E3%81%A7%E5%AE%9F%E7%8F%BE%E3%81%99%E3%82%8B%E3%83%9E%E3%83%AB%E3%83%81%E3%83%87%E3%83%90%E3%82%A4%E3%82%B9%E7%92%B0%E5%A2%83%E3%81%AEWeb%E3%82%A2%E3%83%97%E3%83%AA%E3%82%B1%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3-%E3%83%98%E3%82%A4%E3%83%89%E3%83%B3%E3%83%BB%E3%83%94%E3%82%AB%E3%83%AA%E3%83%B3%E3%82%B0/dp/4862462669)を購入しチェックしました。買ってよかった。

スクリーンリーダーをどのように使っているのか、WAI-ARIAの具体的な実装はどのように進んでいくのか、まだまだわかっていないので今後も調査・学習を続けていきたい。
