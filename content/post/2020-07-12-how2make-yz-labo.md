---
title: YZ-LABOができるまで
author: ゆずりょー
type: post
date: 2020-07-12T09:21:21+00:00
url: /article/how2make-yz-labo@86/
classic-editor-remember:
  - classic-editor
autopostToMastodon-post-status:
  - off
site-sidebar-layout:
  - default
site-content-layout:
  - default
theme-transparent-header-meta:
  - default
autopostToMastodonshare-lastSuccessfullTootURL:
  - https://best-friends.chat/@YuzuRyo61/104500145883130311
categories:
  - 技術系
  - 日記
tags:
  - Discord
  - YZ-LABO

---
ゆずりょーです。

YZ-LABOを開設してから早1か月近く経とうとしていますが、YZ-LABOができるまでの記録をこの記事にまとめてみようかな～と。

<!--more-->

## 1. テストサーバーを作成

Discordサーバーを作成し、YZ-LABO本番環境の原型を作ります。

これは主にロールの作成やチャンネルのテンプレートの作成をして、ロールの権限設定が正しいかを確認します。

## 2. BOT(YZ-LABOT)の作成

テストサーバーを作成したら、ロールの自動付与といった管理支援BOTの作成を行います。

サードパーティのBOTを用いればこのような管理支援機能はいくらでもできますが、  
独自性に欠けてしまったり、Pythonを使い慣れていることから、ライブラリを用いて1から作成することにしました。

スクリプトが完成したらDiscordのデベロッパーコンソールにてBOTアカウントを作成し、YZ-LABOのテストサーバーに参加させます。

設定項目を設定し、本番さながらの動作チェックを行います。

## 3. オブザーバーアカウントでの動作確認

オブザーバーアカウント（一般のDiscordアカウント）を作成して、一般ユーザーの動作具合を確認します。

ロール設定が見込んだ動作でなかった場合はロール設定を見直し、見込んだ通りの権限設定にします。

&nbsp;

主に2~3のステップを繰り返し、実戦投入しても問題ないと判断したらサーバーテンプレートを作成し、  
そのテンプレートから本番環境のサーバーを作成し、YZ-LABOTの本番用BOTアカウントを作成します。

これがYZ-LABOができるまでのステップです。

&nbsp;

YZ-LABOは誰でも入れるパブリックサーバーですので、お気軽にご参加くださいませ。いつでもお待ちしております。



参加はこちらから。→ <a href="https://yz-labo.yuzulia.com/" target="_blank" rel="noopener noreferrer">https://yz-labo.yuzulia.com/</a>