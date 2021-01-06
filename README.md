# カリキュラム初級編


まずはじめに  
カリキュラム受講前の基礎知識の取得、および使用ツールの概要と導入を行っていただきます。  
コーディングの経験やここで紹介するツールの使用経験がある場合は読み飛ばしてもらって構いません。


### HTML, CSSの基礎知識について
ドットインストールの視聴  
https://dotinstall.com/

視聴レッスン
- はじめてのHTML
- はじめてのCSS


*ブラウザインストール*  
以下のリンク先からインストールしてください。(どちらでもいいです)

Google Chrome  
https://www.google.com/intl/ja_jp/chrome/

Fire Fox  
https://www.mozilla.org/ja/firefox/new/


*テキストエディタインストール*  
以下のリンク先から自分のOSにあったソフトをインストールしてください。

Visual Studio Code  
https://code.visualstudio.com/


*拡張機能*  
下記拡張機能をインストールしてください。

| 名前 | 概要 |
| -- | -- |
| .ejs | ejsファイルをハイライトする|
| Editor Config for VS Code | Editor Configファイルを適用させる|
| ESLint | ESLintの補完ツール |
| Prettier | Prettierの補完ツール |


設定ファイル  
下記を設定ファイル（User Settings）に追加してください。

```
{
  "editor.formatOnSave": true,
    "[javascript]": {
      "editor.formatOnSave": true
  },
  "emmet.includeLanguages": {
    "ejs": "html",
    },
  "files.associations": {
    "*.ejs": "html"
  }
}
```


*Git参考サイト（必読）*  
https://techracho.bpsinc.jp/hachi8833/2017_03_14/36735
http://www.backlog.jp/git-guide/


困ったらエラーログをコピペして調べましょう  
その際、英文のみで調べると英語のサイトが優先的に出てくるので、英語が苦手な人は文章と一緒に「エラー」というカタカナも入れて検索しましょう
ただ、今後スキルアップしていくと、そもそも公式ドキュメントが英語しかなかったり、自分が直面している問題が英語の質問サイト（stackoverflow）とかにしかないなどの状況が多々あるので、あんまり忌避するのもよくないと個人的には思っています



**ここからカリキュラムの内容に触れていきます。必ず読んでください**

### カリキュラムの進め方

1 カリキュラム受講者の名前でgithubのアカウントを作成する。

2 該当のカリキュラムのdesignフォルダからデザイン、注意点、理解すべきことなどを確認する

#### 実装開始  
・提出前にHTMLをW3Cバリデーターツールにかけて、「error」を0にしておくこと（warnは無視してください）  
・修正があれば対応する（コミットの際、修正コメントを引用し、どう直したのかをしっかり記述すること）

3 提出時はgithubにコミットとプッシュした後スラックで課題完成の報告をいれる

4 FB対応などはスレッドを活用して行うこと

教育担当者にOKをもらい次第次のカリキュラムに進む



### *初級カリキュラム*
--------------------------------------
*概要*

HTML  
基本的なHTMLの記述を理解する  
セマンティックマークアップの理解  
基本的なPCサイト、SPサイト、レスポンシブサイトのHTML実装


CSS  
基本的なCSSの記述を理解する  
float, flexboxを使った横並びの実装  
positionを使った要素配置  
基本的なPCサイト、SPサイト、レスポンシブサイトのCSS実装


---
## よく言うこと（内容はそのうち理解できると思います）  
- 親子関係はpadding、兄弟要素はmarginで余白を取りましょう  
- クラス名はhtml上のどの要素なのかをざっくり意味するような命名にしましょう  
  - 枝番（__1, -2）、位置情報（--left, __right）はNG  
- scssのディレクトリ構造とプレフィックスの関係  
  - 一つのscssファイルに、複数のプレフィックスが混在してはならない  
   - p-はprojectのp  
     - ページ名をいれてページ固有であると見えるようにする  
   - c-はコンポーネントのc  
   - l-はlayoutのl  
- floatは必ず個別にclearfixで打ち消す  
- インデントはしっかりつける  
- head, bodyは左ベタ付けでよい
