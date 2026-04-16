---
title: LLM講座の受講の仕方(案)
tags: LLM DoCAP ChatGPT URL
author: kaizen_nagoya
slide: false
URL: https://qiita.com/kaizen_nagoya/items/a49304c326a58c780565
---
大規模言語モデル講座 基礎編 2025 Autumn　敗因を勝因に
https://qiita.com/kaizen_nagoya/items/34ffd2b0c47a5f3665d9

を書いてから、受講はじめたら、本質的なことに気がついた。

# 1. 演習先に
プログラマなら、まず動かしてから考えた方がいい人が５割くらいいるのが経験則。
講義を聞いてから演習してもあまり身につかない。

動かしてから聞くと、演習のプログラムが、講義の一部なのか、講義の範囲外のことも扱えるプログラムなのかで、講義内容に対する、疑問、意見も湧きやすいかも。

講義と演習の担当が別だと、講義の調子と演習の調子が異なり、今、なにやってるんだっけって　なることがある。
いい悪いではなく、問題に対する姿勢の問題。ある人には会うけど、別の人には話ないってこと。

講義が先が合わない人は、事前に演習をやっておいてから、講義を聞けばいいってことだけ。

# 2. 資料の確認

## 2.0 Web
日程
https://weblab.t.u-tokyo.ac.jp/large-language-model/

### 2.0.1 内部Wiki
内部Wikiがあるらしい。
去年はあまり貢献できなかった。ごめんなさい。
外部に機密情報を除いて書いて、内部Wikiから外部のURLを書くといいかも。
理由は後日記載。

## 2.1 Notion
https://curved-rambutan-a71.notion.site/
ログイン画面を選びログインすると、主なリンクはNotionにある。
この記述がSlackにあるとうれしいかも。
あるいは、内部Wikiか。

自分に必要な情報が網羅されているとは限らず、追加したいものがあるかも。

## 2.2. Omnicampus
https://edu.omnicamp.us/dashboard/
自分が参加しているURLの一覧が出る。
宿題が、Omnicampusから出すことは、Notionのリンクのある宿題の出し方に記載がある。
NotionのOmnicampusの添え書きに、アンケートと宿題の提出と書いてあれば行方不明にならない。
宿題の提出は、Omnicampusにあるが、宿題の内容は


## 2.3 Google Drive
宿題のプログラムと講義資料はGoogleDriveにある。
このipynbというJupyterNotebookのプログラムをダブルクリックすると、Google Colabが起動するらしい。
2024年は、その動作がわかるのに３日かかった。
毎回行方不明になったりもしていた。

# 2.4 Google Colab
https://drive.google.com/drive/my-drive
自分のIDでログインすると自分のファイルが見える。
宿題は、
「上から順に回答していくと、提出用の CSV ファイル `LLM_Basic_day3_submission_pred.csv` が自動的に作成されます。 」

## 2.5 JupyterNotebook
一度でもJupyterNotebookを利用したことがある人なら、
[]が未実行であること。カーソルをその右に移動すると▶️があらわれ、押せば実行する。


## 2.6 Slack
いくつかの大事なURLはSlackに掲載されている。



# 雑記
アンケートで書いたこと＋かきがかったことを意味が通じるように編集しています。
日本語が不得意で、誰にでもわかる日本語がかけません。ごめんなさい。
### Day1 
アンケートの送信で、先頭と最後に「アンケートが送信されました」と出て、見落としが少ない。画面の色でもかわるともっとわかりやすいかも。

### Day2

### Day3
事前学習って、人間が事前に内容を学習しておけっていうことかと思った。機械学習、深層学習について補助講師を長年していたが、システムの導入方法とプログラミング言語のエラー取りを担当しており、基本用語はプログラミング言語の関数、定数、変数のまま表記しないとピンとこないかも。
Day2は、演習が追いつかなかった。Day3は、同時とは言えないが、なんとか演習をしながら聞けた。受講の姿勢としては、講義を聞く前に演習をしておけばよかったかもってなった。反省。
全体へのアナウンスで、事前に演習をすると講義がわかりやすい人がいるらしいって伝えてもらえると嬉しいかも。自分でも、もう少し時間があれば、事前演習をこころがけ、成果がみえてきたらSlackに報告予定。
講師のかたが丁寧にご説明してくださりたいへんありがたかった。講義と演習が同じ方だと、講義の方向性と演習の方向性のトーンが同じで理解しやすい。
初年度は受講していませんが、昨年と今年をくらべると、いろいろな意見を出したことが反映しており、すばらしいと思っています。皆様のご尽力に感謝します。

講義の中で、並列処理できるものがあることを明らかにしたことが、現在の機械学習の発展の原理の一つであることがわかった。
交差エントロピーは確率モデルの計算で扱ったことがある。
Causual Attentionは、LLMを勉強しはじめてから知った用語で、まだ十分理解できていない。
因果関係の時間順序を守るためのものとすると、並列処理しても、因果関係の時間順序をまおれば、結果として、交差エントロピー損失を小さくできるかなって思うんです。
# Ref


ISO IEC Artificial intelligence Standards
https://qiita.com/kaizen_nagoya/items/1d1ffe4ac8e1dc67501f



MCP入門 〜面倒なことはAIエージェントにやらせよう〜 by からあげ を聞きながら
https://qiita.com/kaizen_nagoya/items/54b648c838fae8d57e38

MCP入門 〜面倒なことはAIエージェントにやらせよう〜 by からあげ を聞きながら、補足と反論 by ChatGPT
https://qiita.com/kaizen_nagoya/items/0939d58d31666562090c

C言語を習得する３つの方法
https://qiita.com/kaizen_nagoya/items/84cab0888c193bba429b

Views上位６４記事　20250617現在
https://qiita.com/kaizen_nagoya/items/26dbbd04cf18b7742972

C言語(C++)が必要な人、必要ない人　with ChatGPT
https://qiita.com/kaizen_nagoya/items/a074cb8cd292d8d94bd4

C言語を習得する３つの方法　with ChatGPT
https://qiita.com/kaizen_nagoya/items/4a3518a18fa49f46787f

＜この記事は個人の過去の経験に基づく個人の感想です。現在所属する組織、業務とは関係がありません。＞
This article is an individual impression based on my individual experience. It has nothing to do with the organization or business to which I currently belong.
Este artículo es una impresión personal basada en mi experiencia personal. No tiene nada que ver con la organización o empresa a la que pertenezco actualmente.
### 文書履歴(document history)
ver. 0.01 初稿 　20251016
### 最後までおよみいただきありがとうございました。
いいね　💚、フォローをお願いします。
#### Thank you very much for reading to the last sentence.
Please press the like icon 💚　and follow me for your happy life.
#### Muchas gracias por leer hasta la última oración.
Por favor, haz clic en el ícono Me gusta 💚 y sígueme para tener una vida feliz.
