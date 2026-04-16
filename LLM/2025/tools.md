---
title: 大規模言語モデル講座 基礎編 2025 Autumn 2024年の敗因を2025年の勝因に 35ツールと33の対応
tags: LLM 松尾研 corab ChatGPT Omnicanpus
author: kaizen_nagoya
slide: false
URL:https://qiita.com/kaizen_nagoya/items/34ffd2b0c47a5f3665d9
---
二度目まして。2024年は、大規模言語モデル講座最後まで参加したものの納得いく処理ができず、道具にふりまわされた感が残っています。去年の敗因を今年の勝因にすべく道具類について整理しています。去年と今年の違いは、職業訓練校でUML講座を担当するようになり、PlantUMLとChatGPTを使った図からPlantUMLの生成とソースコードの生成に取り組むようになり、来年の講座へ向けて、ここで使う道具類を使い倒そうという感じです。2024年の敗因を記録し、ふりかえりながら、勝因へ変えようとしています。出たエラーは記録し、対策をたてようと思います。よろしくお願いします

講座の詳しい内容によっては、非公開を原則としている事項があり、間違って記載していた場合には、slackでコメントいただけると幸いです。
ここへのコメントは、システムの制約で見えません。ログアウトしてコメントを見れば読めますが、コメントへの返事は書けない状況です。機密、著作権関係の事項については、編集リクエストをいただけると幸いです。

提供側の視点でのツールの調整についてと、システム権限のない利用者でもできることを分けて書き足すように努力中です。どちらの立場での記述か不明な場合は、突っ込み、突撃をお願いします。

LLM演習の資料をChatGPTで作成中。

この資料をもとに、実際に受講する際に、見る順番を示した資料を作りはじめました。

LLM講座の受講の仕方(案)
https://qiita.com/kaizen_nagoya/items/a49304c326a58c780565

## 困りごと 
ダウンロードファイルを用意したといいつつ、次のいくつかのエラーが出てファイルがダウンロードできない。
404 Not Found Where the page should be, Empty space and missing words— A void in the code.
コード インタープリターのセッションの有効期限が切れました
原因と対策がたてれていない。

ChatGPT ダウンロードエラー
https://qiita.com/kaizen_nagoya/items/74dffaaeb80bf4da6681

ChatGPTでダウンロードできなかった（２）
https://qiita.com/kaizen_nagoya/items/0699f73b405e155da6ee

珍プレーがいろいろ収集できています。好プレーが披露できるかはこれからの努力次第かも。

<この項は書きかけです。順次追記します。>
This article is not completed. I will add some words and/or centences in order.
Este artículo no está completo. Agregaré algunas palabras en orden.
## 前提
非常勤講師をしていた岐阜大学で、全学共通言語がpythonになり、こりゃ自分もpythonしゃべらなきゃってなって。東北大学の１００本ノックをやった。

言語処理100本ノックをdocker(19)で。python(1)覚えるのに最適。
https://qiita.com/kaizen_nagoya/items/7e7eb7c543e0c18438c4

企業の新人教育、機械技術者のプログラマへの転向教育などで利用した。

深層学習の教育の補助講師をしていて、WindowsへのPythonの導入などをお手伝いした。

「ゼロから作るDeep Learning ２自然言語処理編」読書会に参加する前に読んで置くとよい資料とプログラム, python(8)
https://qiita.com/kaizen_nagoya/items/537b1810265bbbc70e73

自分たちのやった深層学習の勉強会の脱落者の半分がWindowsに必要なpythonのインストールができなかった人たち。
その記事が、Qiitaでの自己最大Viewsを得た。

Windows(MS)にPython(Anaconda)を導入する（7つの罠）
https://qiita.com/kaizen_nagoya/items/7bfd7ecdc4e8edcbd679

さまざまなpythonの版でためすため、dockerを利用し、同時に多数の版の試験をできるようにした。

なぜdockerで機械学習するか 書籍・ソース一覧作成中 (目標100)
https://qiita.com/kaizen_nagoya/items/ddd12477544bf5ba85e2

量子コンピュータの講師をしながら、python教育を担当した。

「量子(13)アニーリングの基礎」を読む
https://qiita.com/kaizen_nagoya/items/29580dc526e142cb64e9

pythonとjupyternotebookは、一応教える側っていう。

## Web/ブラウザ
ブラウザが一番最初の道具かも。

### 対応0 ブラウザ

pythonを使うにあたってブラウザは何がお勧めですか。　with ChatGPT
https://qiita.com/kaizen_nagoya/items/b6cc75edfe3798018e86

バーチャルソフトウェア研究所というサイトに掲載した「検索の哲人」に関する記事を雑誌に掲載されたくらいにはつかてちたかも。
所属の大同大学の学生が、名古屋市のホームページコンテストで優勝した。くらいにはすごいかも。

松尾研AIコミュニティ
https://qiita.com/organizations/matsuolab-aicommunity/items

「大規模言語モデル(LLM)講座2025 基礎編・応用編」募集開始
https://weblab.t.u-tokyo.ac.jp/news/「大規模言語モデルllm講座2025-基礎編・応用編」募集/

大規模言語モデル講座 基礎編 2025 Autumn
https://weblab.t.u-tokyo.ac.jp/large-language-model/

LLM 2024 仕様
https://weblab.t.u-tokyo.ac.jp/llm_contents_2024/
### 対応 1 Web類
Web作業の調整 with ChatGPT
https://qiita.com/kaizen_nagoya/items/1fae382e859f9d4e5ddf

### 対応 2 python
pythonのエラーが取れないとうまくいかないこともある。
python初心者への対応を考えたい。

python, JupyterNotebook 初心者へ with ChatGPT
https://qiita.com/kaizen_nagoya/items/ea4d2024568b147c1be8

### 対応 3 jupyter notebook
jupyternotebookはどこにありますか。
https://qiita.com/kaizen_nagoya/items/2b9c2b4c9b4ee186ba9c

### 対応 4 git(github)
Githubに登録されているものを利用することがあるかもしれない。
一行コピペすれば、エラーがでないことがある。エラーがでると、たいへん。

LLM @ GitHub with ChatGPT
https://qiita.com/kaizen_nagoya/items/bc29150ad6054ac1adfb

### 対応 5 shell command/shell script
コマンドプロンプトは、いろいろな局面で使えると便利なことがある。GUIだと手間がかかることを一発。
cd
ls
mkdir
cat
rm
mv
unzip
pip
conda

LLM開発におけるShell Command例 with ChatGPT
https://qiita.com/kaizen_nagoya/items/61dcdc84f4b7848b0e2b

### 対応 6 docker
dockerで実行した結果を、hub等に置いて共有するとすごく楽。

なぜdockerで機械学習するか 書籍・ソース一覧作成中 (目標100)
https://qiita.com/kaizen_nagoya/items/ddd12477544bf5ba85e2

dockerでLLM with ChatGPT
https://qiita.com/kaizen_nagoya/items/e0f93d2c3eca3969c896

# 敗因１ 行事、資料、AIツール、意思疎通方法が、たくさんあり、めまぐるしく、今、どこで、何をやっているのかさっぱり。

slackは、それなりに使っているつもりでも、slackにどう情報を展開するかの文化が違うと、路頭に迷うことがわかった。

新たな利用システムが5つあった。それまで使ったことがあるシステムは6つだった。
こりゃだめだ。新たなシステムが２つでもPerformanceは50%になるって。

今年の４月から職業訓練校でUMLと構造化プログラミングを教えることになった。
UMLツールでは、いろいろ使いながらPlantUMLを使い始めた。
ChatGPTで、図からPlantUMLを生成したり、図からソースコード生成などをしてきた。

今年のUML講座のふりかえりと、昨年のLLM講座の反省になって、LLM講座で使っていたツールをUML講座でも使うとなったらどうしたらいいかを調べ始めた。

職業訓練(IT)
https://qiita.com/kaizen_nagoya/items/95368b63fa21d64271ec

# Tool群
(new)というのは、自分が初めて使ったツール。
一つの資料に他の資料のありかが書いてなかったり、リンクがなかったりも迷子になった理由かもってなった。
ツールのそれぞれの機能と、使い方を確認していこうかなって思うんです。最後の３つは、自分では使おうと思っているもので、去年使ったかどうかの記憶はないかも。

0. ブラウザ(Chrome, Safari, Edge, ...)
1. Notion.site(new)
2. Omnicanpus(new)
3. Google Colab(new)
4. Hugging Face(new)
5. sli.do(new)
6. slack
7. Google form
8. Google drive
9. Zoom
10. Web
11. Mail
12. python
13. JupyterNotebook
14. git(github)
15. shell
16. docker
17. Canvas LMS(new)
18. Google Classroom(new)
x 19. Youtube
x 20. Qiita
x 21 arXiv
x 22 bioRxiv(new)
x 23. X(Twitter)
X 24. Gemini(new)
X 25. Open AI ChatGPT(new)
X 26. Claude(new)
X 27. Google Calendar
X 28. Stack Overflow
X 29. Researchmap
X 30. Discord
X 31. IEEE
X 32. ACM
X 33. Facebook
X 34. Line
x 講義で正式に用いていないはず。arXivは、参考文献には頻出する。Paper & Hacksでも。
X 正式対応ツールではないかも。

## 1.notion.site(new)
https://notion.site/
詳細非公開。

### 対応 7. Notion.site
Notion.siteを理解するより、自分が担当している講義の資料をNotion.siteで作るにはという視点で調べた。

Notion.siteの使い方 UML講座を例に with ChatGPT
https://qiita.com/kaizen_nagoya/items/0007ddb0417900d3d531

### 対応 8 Canvas LMS 
Canvas LMS 使ったことがありません。with ChatGPT
https://qiita.com/kaizen_nagoya/items/e35fed50c9c4f3d4875a

### 対応 9 Google Classroom
使ったことがありません。これはなんですか。
https://qiita.com/kaizen_nagoya/items/1cf08f04118075c8f550

## 2.Omnicampus (new)
初めて利用するシステム。

アンケートを送っても、画面が大きく切り替わらず、送れたのか送れなかったのかがわかりにくい。
不足事項は赤になるが、画面からはずれていると気がつかない。
送信できたというMSGは、一番上に現れ、画面からはずれていると気がつかない。

去年も送信をなん度も押したことを思い出した。

### 対応 10 Omnicumpus
Omnicanpus でUML講座 with ChatGPT
https://qiita.com/kaizen_nagoya/items/a33f99510e56a9b113e8

## Google Colab(new)
演習の土台

### 対応 11  Google Colab
はじめてのGoogle Colab with ChatGPT, JuyterNotebook知ってる人向け
https://qiita.com/kaizen_nagoya/items/a7452b9ba9f2d8036341

### 対応 12 Gemini Colab連携
Gemini Colab連携
https://qiita.com/kaizen_nagoya/items/8765136bd360d6aeca1c

### 対応 13 Claude と Google Colabの連携
Claude と Google Colabの連携
https://qiita.com/kaizen_nagoya/items/e9348a4ab496ef96c58e

### 対応 14 Colab ChatGPT連携
Google Colab ChatGPT連携と3, 10 AI比較Script with ChatGPT
https://qiita.com/kaizen_nagoya/items/800039b91981919e4155

## Hagging face(new)
演習の展開
### 対応 15 Hugging face
はじめてのHugging Face with ChatGPT
https://qiita.com/kaizen_nagoya/items/2bd8d603acc09517e34a

## slido(new)
質疑のうけつけ(Paper & Hacks)

https://app.sli.do/
投票により優先順位が変わるのはいいかも。

### 対応 16 sli.do
sli.do　使いやすいですか？ with ChatGPT
https://qiita.com/kaizen_nagoya/items/c3fb03cb38055240208c

## slack
コミュニティの参加そのものがslack。
資料URLの展開もここ。
基本質疑もここ。
毎日いれば、そのうちわかる。

### 対応 17 slackのローカルルールでよさげなものを厳選し、交通整理を誰かがやる
slackってなんですか。with ChatGPT
https://qiita.com/kaizen_nagoya/questions/87cfcf30a694cf93e30a

slackをプログラマが使う場合のよい使い方と課題
https://qiita.com/kaizen_nagoya/items/5ee6983d78c706f94771

## Google form 
本講座の質疑。月１くらいは使う。
会社によっては、Google formでのアンケート回答を許可していない場合がある。
業務上は他の方法を取ることがあるらしい。

### 対応 18 Google form slackとの連携など
google form 使いやすいか with ChatGPT
https://qiita.com/kaizen_nagoya/items/41471016506b32ba08ac

## Google Drive
教材置き場。前年の資料は公開。今年は非公開。
知らないうちに週１くらいは使っているかも。

### 対応 19 Google Drive
会社によってはGoogleのサービスのうち、利用しないことを決めている場合がある。
業務上は他の方法を取ることがあるらしい。

Google Drive with ChatGPT
https://qiita.com/kaizen_nagoya/items/88b20b2598f96c960b25

## Zoom
オンライン講義。
Paper & Hacksもzoomだから毎週利用。この１年間。

### 対応 20  Paper & Hacks 
毎週火曜にある別行事 Paper & Hacksに参加し、できるだけ自分の感想、調査を追加しよう。

ある回の報告が、Qiitaのviews自己５位。Views 80,000以上。
MCP入門 〜面倒なことはAIエージェントにやらせよう〜 by からあげ を聞きながら
https://qiita.com/kaizen_nagoya/items/54b648c838fae8d57e38

松原研の講座を受けようと思ったのは、からあげさんがいるから。
地元のコミュニティでお世話になった。単なるおっかけです。
からあげさんのコミュニティからあげ帝国へもおいでください。

###  対応 21 Reserchmap
Researchmapは、学術利用であれば、研究データを置くことが可能かも。

researchmapサービス基本規約　の根拠法　探索
https://qiita.com/kaizen_nagoya/items/e4697b9d5c1b9cc399c2

Researchmap 研究データ置き場 with ChatGPT
https://qiita.com/kaizen_nagoya/items/be7fd30c06203431f43a

### 対応 22 Qiita
自己記事が多いと、下記のようなサイトにアクセスできない。なにしてくれちゃうのQiita。
表示しない仕様はこの２年くらい変化はない。
502: Bad Gateway

Qiitaは講座の内容を展開する公式対応サイトではないっぽい
関係者のIDを特定して、連携、相談するのがいいかも。

松尾研AIコミュニティ
https://qiita.com/organizations/matsuolab-aicommunity/items

松尾研AIコミュニティ@Qiita
https://qiita.com/kaizen_nagoya/items/6b904eacbbd9a55185cf

### 対応 23 X(twitter)
東京大学 松尾・岩澤研究室 X(Twitter)における with ChatGPT
https://qiita.com/kaizen_nagoya/items/d4859ecafe6dda7c4aff

## Youtube
Youtubeは便利。わかりやすい動画を選べばもうばっちり。

### 対応 24 Youtube
見た動画の感想、疑問、参考文献などを整理したい。今のところは原則Qiita

東京大学 松尾・岩澤研究室
https://qiita.com/kaizen_nagoya/items/a17b82951a60dbb32103

## メール
登録完了はメールで来る。
きたらきがつく。こないときがつかない。あたりまえ。

### 対応 25 mail 
mailで来た情報は、自分のPrivate Webに記載している。
slack, Google Drive, Notion, Zoomなど４箇所以上に同じ情報があると嬉しいかも。

mail アラカルト with ChaatGPt
https://qiita.com/kaizen_nagoya/items/6ae2ad4a16fa2bfc82cc

## Google Calendar
行事をGoogle Calendarで管理している人は、LLM講座もGoogle Calendarに登録するだろう。

### 対応 26 Google Calenar
Google Calendar with ChatGPT
https://qiita.com/kaizen_nagoya/items/51933aad72f8088980f5

# 敗因2 毎日のわからないことを、どこで、どう投げればいいかがわからず。
この記事を書いていることも勝因の一つっていう。
課題は、作研も、同じような記事をかきながら進もうとした。

はじめて触るツールが２つ以上あると、もう闇雲になるっていうr。

先頭に当時のQiitaへの記事を記録。
Slackに気軽に書き込めるといい。指揮者がいれば、誰がどういう能力があるから、どこに聞くといいよってわかるかもってなった。自分が指揮者にならなきゃ。

それぞれの節では、ていねいな説明がある。
講義と演習が同一講師だとつながりがわかるが、別の方だと方向性がやや違うのか、話の仕方が違う感じで、自分で誤解するか、どつぼにはまっていく感じ。

コンペティションの課題がわかりにくいだけでなく、エラーが初出だったりして、誰が、どう聞くと、誰が応えてくれるかって勘所がうろうろ。

### 対応 27 stackoverflow
今年は、エラーをいろいろ記録し、その対応を可能な限りでChatGPTなどに頼って解しよう。
Slackでの質問には、正解がわからなくても自分のやったことを回答してみよう。
じゃまだったらごめんなさい。

QAは、StackOverflowが楽。
公開できることは、StackOverflowで聞くのも手かも。

stack overflow連携の利点と課題 with ChatGPT
https://qiita.com/kaizen_nagoya/items/ecfe851fd98fa17a9397

今年の目標はまだない。

ここまでお読みいただきありがとうございます。
一つひとつの記事は、どんどん複雑になり役に立たないと思います。

slackでご質問いただければご回答さしあげれるように努力します。
Qiitaにコメントでご質問いただいても、著者には表示されず、コメントへのQiitaでの返事ができず、回答に時間がかかってしまいます。

### 対応 28 Discor連携
全然違う視点の取り組みも大事かも。

discord連携の利点と課題 with MCP by ChatGPT
https://qiita.com/kaizen_nagoya/items/879b807c19ed67b6ef24

discor利用されていない方は、次をご参照ください。。
からあげマニアのためのコミュニティ「からあげ帝国」が誕生しました
https://karaage.hatenadiary.jp/entry/2022/11/30/073000

### 対応 29 QA　アラカルト
macOSにおける文字化け with ChatGPT
https://qiita.com/kaizen_nagoya/items/44d82fd97614b5923d0a

# 理論・道具
理論は道具と表裏一体かも。上記ツール以外に、汎用的な概念で抑えられるところは抑えたい。
## arXiv
LLMの論文をかたっぱしから読みつつ、プログラムを動かしつつ、データを工藤しつつ、、、

### 対応 30 arXiv LLM
LLM @ arXiv with ChatGPT
https://qiita.com/kaizen_nagoya/items/91191ea22577ae18778e

Transformers

## Robot Transformer
### 対応 31 arXiv MCP

robot transformer @arXiv
https://qiita.com/kaizen_nagoya/items/bb68899be7d985b56222
## MCP

### 対応 32 arXiv MCP
MCP論文 @arXiv with ChatGPT
https://qiita.com/kaizen_nagoya/items/8ba05d667673ff98af28

## 領域固有の知識・手法


# 参照
MCP入門 〜面倒なことはAIエージェントにやらせよう〜 by からあげ を聞きながら
https://qiita.com/kaizen_nagoya/items/54b648c838fae8d57e38

MCP入門 〜面倒なことはAIエージェントにやらせよう〜 by からあげ を聞きながら、補足と反論 by ChatGPT
https://qiita.com/kaizen_nagoya/items/0939d58d31666562090c

C言語(C++)が必要な人と必要ない人
https://qiita.com/kaizen_nagoya/items/2afe9e846b55b24cb6f1

C言語(C++)が必要な人、必要ない人　with ChatGPT
https://qiita.com/kaizen_nagoya/items/a074cb8cd292d8d94bd4

C言語を習得する３つの方法
https://qiita.com/kaizen_nagoya/items/84cab0888c193bba429b

C言語を習得する３つの方法　with ChatGPT
https://qiita.com/kaizen_nagoya/items/4a3518a18fa49f46787f

20241009 memo LLM AI
https://qiita.com/kaizen_nagoya/items/80f00b3d6b44e00fec05

Colab の生成 AI(24) warning 理解
https://qiita.com/kaizen_nagoya/items/34ffd2b0c47a5f3665d9

スケーリング法則が何故 スケーラブルなのか? LLM memo 2024100802
https://qiita.com/kaizen_nagoya/items/b5a27b0a41a80b3feaa6

「スケーリング法則が何故スケーラブルなのか?」 LLM memo 2024100801
https://qiita.com/kaizen_nagoya/items/88bf53ed79c554e94688

ModuleNotFoundError python(41) error(138)
https://qiita.com/kaizen_nagoya/items/d364dd7e31d8853f37da

＜この記事は個人の過去の経験に基づく個人の感想です。現在所属する組織、業務とは関係がありません。＞
This article is an individual impression based on my individual experience. It has nothing to do with the organization or business to which I currently belong.
Este artículo es una impresión personal basada en mi experiencia personal. No tiene nada que ver con la organización o empresa a la que pertenezco actualmente.
### 文書履歴(document history)
ver. 0.01 初稿 　20251001
### 最後までおよみいただきありがとうございました。
いいね　💚、フォローをお願いします。
#### Thank you very much for reading to the last sentence.
Please press the like icon 💚　and follow me for your happy life.
#### Muchas gracias por leer hasta la última oración.
Por favor, haz clic en el ícono Me gusta 💚 y sígueme para tener una vida feliz.
