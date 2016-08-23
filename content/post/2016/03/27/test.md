+++
date = "2016-03-27T20:29:18+09:00"
title = "blog.orangebom.org is @keita_kawamoto ’s blog"
tags = ["blog"]
+++

![](https://cloud.githubusercontent.com/assets/1661325/13044802/8b32ee84-d413-11e5-893c-ba4f64ac6950.png)

仮説検証ツール `Javelin Experiment Board` がよさそうだったのでまとめます。

<blockquote class="twitter-tweet" data-lang="ja"><p lang="ja" dir="ltr">カップヌードル   たまに食べたくなる   魅力   謎    心理   [検索]</p>&mdash; keita kawamoto (@keita_kawamoto) <a href="https://twitter.com/keita_kawamoto/status/767297926783639556">2016年8月21日</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

### 日本語訳ボード

作りました。

![](https://cloud.githubusercontent.com/assets/1661325/13044802/8b32ee84-d413-11e5-893c-ba4f64ac6950.png)

## ジャベリンボードとは？

**仮説検証ツール。**

アイデアの前提となるユーザーの課題が本当に存在するか、アプローチ方法が間違った前提に立脚していないかを検証する。
「誰の」「どんな問題を」「どうやって解決するか」と、それらの大前提となっている「仮説」をボード上にセットし、実際にオフィスの外に出て顧客と対話し、その仮説が本当に正しいのかを検証する。
http://growthhack.vasily.jp/2015/01/startup-roadmap/ より

『誰のどんな問題をどのように解決するかの理想を描き、描いた仮説が実在するか、
事前に検証できないかを検討し、現実とのギャップに学びながら軌道修正していく必要がある』
http://mtl.recruit.co.jp/ux-sketch-vol4/ より

<script async class="speakerdeck-embed" data-id="3aa195056add46a4a1ada25338538df1" data-ratio="1.33333333333333" src="//speakerdeck.com/assets/embed.js"></script>

## 使い方

- 1.どんどん左側に書き出していく（全員で）
 - 想像できるもの “このプロダクトの顧客は誰か？問題は何か？解決策は何か？最も問題なのは何か”
- 2.下部のヒントは書き方サンプルなので気にしなくて良い
- 3.次に書き出したものの中から最もリスクの高いものを「１」のラインに移す。

サンプルでいうと

項目|サンプル内容
---|---
顧客|スタートアップの創業者
抱えている問題|UXのフィードバックを受けたくても受けられない（人脈も資金もツールもない）
解決策|なし（現時点では）
最も問題なのは|信頼できる情報源がない(前述ゆえに)
方法・達成基準|ここまでの仮説を10人にインタビューして6人その通りだと答えたらこの仮説は正しいとする
結果&決定|結果を書く “その通りだった”
学習|これらの検証によって学んだこと “意外と〜〜だった”

- 4.満たしたら「１」そのまま残し「２」に移る
- 5.満たしていなければ（10人中6人み満たなかったら）「１」を他の仮説に差し替えて繰り返す

## “リスク”とは？

**“女性は全員料理をする” などの仮説。そのまま利用すると失敗する確率が高いもの。**
「本当に？例外なく全員料理するのか？」などのリスクがある状態で検証なしにこのままプロダクトを進めると（間違っているかもしれないゆえに）失敗するかもしれない。検証してリスクをなくしていく必要がある。

```

<!DOCTYPE html>
<html>
  <head>
  <meta http-equiv="content-type" content="text/html; charset=utf-8">
  <meta name="viewport" content="width=device-width">
  <meta name="author" content="keita_kawamoto">

    <title>Javelin Experiment Board &middot; Orangebomb</title>

  <meta property="og:title" content="Javelin Experiment Board">
  <meta property="og:url" content="http://localhost:1313/blog/2016/03/27/test/">
  <meta property="og:image" content="http://blog.orangebomb.org/images/ogp.png">
  <link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/font-awesome/4.6.3/css/font-awesome.min.css">
  <link rel="stylesheet" href="/css/base.css">
  <link rel="stylesheet" href="/css/header.css">
  <link rel="stylesheet" href="/css/contents.css">
  <link rel="stylesheet" href="/css/footer.css">
  <link rel="stylesheet" href="/css/archives.css">
  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Karla|Source+Code+Pro">

  <link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/8.6/styles/ir_black.min.css">

  <link rel="apple-touch-icon-precomposed" sizes="57x57"   href="/images/apple-touch-icon-57-precomposed.png">
  <link rel="apple-touch-icon-precomposed" sizes="114x114" href="/images/apple-touch-icon-114-precomposed.png">
  <link rel="apple-touch-icon-precomposed" sizes="72x72"   href="/images/apple-touch-icon-72-precomposed.png">
  <link rel="apple-touch-icon-precomposed" sizes="144x144" href="/images/apple-touch-icon-144-precomposed.png">
  <link rel="shortcut icon" href="/images/favicon.ico">
  <link rel="canonical" href="http://localhost:1313/blog/2016/03/27/test/">
</head>

  <body>
    <div class="header">
  <div class="header-inner">
    <header>
      <h1 class="logo"><a href="http://localhost:1313/"><img src="http://localhost:1313/images/logo.svg" alt="Orangebomb"></a></h1>
      <nav>
        <ul class="menu">
          <li><a href="/post">ARCHIVES</a></li>
          <li><a href="/tag">TAG</a></li>
          <li><a href="#profile">PROFILE</a></li>
        </ul>
      </nav>
    </header>
  </div>
</div>

```

## 使用するタイミング

- Q. すでに存在するもので行ったほうがよいのか、作り出す前に行ってもいいのか
- A. どちらでも利用可能

## 関連記事

関係ありそうな記事・サイト一覧

- [Lean Startup Machine Tokyo December 2013](http://www.dnp.co.jp/cio/servicedesignlab/publicity-lsmt.html)
- [スタートアップロードマップ：リーンやグロースハックの概念を俯瞰して整理する](http://growthhack.vasily.jp/2015/01/startup-roadmap/)
- [「機能するデザイン」を考えるために、必要なこと。 UX Sketch Vol.4](http://mtl.recruit.co.jp/ux-sketch-vol4/)
- [amana tech night vol.3「達人たちから学ぶ。グロースハックとUI/UX」開催レポート≪前編≫](http://amanatech.org/amana-tech-night-vol-3_report-1)
- [TECH VALLEY#4グロースハックパーティ！ イベントレポ](http://suidenoti.hatenablog.com/entry/2015/04/27/214630)
- [なんとなく参加した講演会で、今までグロースハックは胡散臭いだけのバズワードと思っていたことを反省した](http://ojisan-a.hatenablog.com/entry/2015/04/15/233236)

[Javelin](http://vip.javelin.com/)は現在アーリーアクセスの人しか使えないようになっている模様。
