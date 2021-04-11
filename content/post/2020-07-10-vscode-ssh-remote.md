---
title: VSCodeをWindowsホストのSSH経由でリモート繋げたら問題が起きた件
author: ゆずりょー
type: post
date: 2020-07-10T05:24:24+00:00
url: /article/vscode-ssh-remote@81/
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
  - https://best-friends.chat/@YuzuRyo61/104487889523014406
categories:
  - 技術系
  - 日記
tags:
  - VSCode

---
ゆずりょーです。

VSCodeを使ってSSH経由でリモート開発、便利ですよね。

Windowsをホストとして、SSH経由でVSCodeのリモート開発をしようと思ったら大きな落とし穴。

結論から言ってしまうと、**ウイルス対策ソフトが悪さしていました。**

cmd.exeが不正変更したというログが出たので、例外許可にしたのですが、それでも問題が発生。

リモート用のVSCodeパッケージのインストール中に文字化け（だと思う）が発生して接続に失敗してしまう問題がありました。

常駐を切ってみたら問題なく動きました。これはどうなんだ・・・。

でも結局はWindowsをSSH経由でVSCodeなんてあまりおすすめできないのであれなのですが、  
このようなケースがあったらウイルス対策ソフトに引っかかっているっていう可能性も視野に入れてみてくださいね。