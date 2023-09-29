# カードテンプレート
<!-- # Card Templates -->

カードテンプレートは、カードの表面と裏面にどのフィールドを表示するかをAnkiに指示したり、特定のフィールドにテキストがある場合にどのカードを生成するかを制御したりします。 カードテンプレートを調整することで、一度に多くのカードのデザインやスタイルを変更することができます。
<!-- Card templates tell Anki which fields should appear on the front and back of your card,
and control which cards will be generated when certain fields have text in them.
By adjusting your card templates, you can alter the design and styling of many of your
cards at once. -->

カードテンプレートについての解説は、次の動画にもあります。
<!-- Card templates are covered in some of the intro videos: -->

- [カードの表裏反転](http://www.youtube.com/watch?v=DnbKwHEQ1mA&yt:cc=on)

- [カードのスタイリング](http://www.youtube.com/watch?v=F1j1Zx0mXME&yt:cc=on)

- [回答のキーボード入力](http://www.youtube.com/watch?v=5tYObQ3ocrw&yt:cc=on)

<!-- - [Switching Card Order](http://www.youtube.com/watch?v=DnbKwHEQ1mA&yt:cc=on)

- [Styling Cards](http://www.youtube.com/watch?v=F1j1Zx0mXME&yt:cc=on)

- [Typing in the Answer](http://www.youtube.com/watch?v=5tYObQ3ocrw&yt:cc=on) -->


## テンプレート画面
<!-- ## The Templates Screen -->

編集画面内の「カード...」ボタンをクリックすると、カードテンプレートの内容を変更できます。
<!-- You can modify card templates by clicking the "Cards..." button inside the
editing screen. -->

古いバージョンのAnkiでは、左上に表面のテンプレート、左下に裏面のテンプレート、その間にカード全体のスタイル設定欄が表示されます。Ankiのバージョン2.1.28以降では、表面、裏面、スタイルの各欄は同時には表示されなくなりました。<kbd>Ctrl</kbd>+<kbd>1</kbd>、<kbd>Ctrl</kbd>+<kbd>2</kbd>、<kbd>Ctrl</kbd>+<kbd>3 で表示を切り替えることができます。
<!-- For older Anki versions, on the top left is the front template, on the bottom left is the back
template, and in between them is the card styling section. For Anki versions
2.1.28+ the front, back, and styling are no longer shown at the same time.
You can switch between them with <kbd>Ctrl</kbd>+<kbd>1</kbd>, <kbd>Ctrl</kbd>+<kbd>2</kbd>, and <kbd>Ctrl</kbd>+<kbd>3</kbd>. -->

Ankiでは、テンプレートはWebページ用の記述言語であるHTMLで記述されています。スタイルは、Webページのスタイリング（装飾・レイアウトなどの指定）に使われる言語であるCSSで記述されています。
<!-- In Anki, templates are written in HTML, which is the language that web
pages are written in. The styling section is CSS, which is the language
used for styling web pages. -->

画面の右側には、現在選択されているカードの表面と裏面のプレビューが表示されます。ノートを追加しようとしているときにこのウィンドウを開いた場合、プレビューは「追加」ウィンドウ内に入力したテキストに基づいて表示されます。ノートの編集中にこのウィンドウを開いた場合、プレビューはそのノートの内容に基づいて表示されます。[ツール]→[ノートタイプの管理] からウィンドウを開いた場合、Ankiは実際のノートのコンテンツの代わりに各フィールドの名前をかっこで囲んで表示します。
<!-- On the right is a preview of the front and back of the currently
selected card. If you opened the window while adding notes, the preview
will be based on the text you had typed into the Add Notes window. If
you opened the window while editing a note, the preview will be based on
the content of that note. If you opened the window from Tools → Manage
Note Types, Anki will display each field’s name in parentheses in place
of content. -->

ウィンドウの右上には「オプション」ボタンがあり、カードタイプの名前の変更や並び替えのオプションのほか、次の2つのオプションが用意されています：
<!-- At the top right of the window is an Options button that gives you
options to rename or reorder the cards, as well as the following two
options: -->

- 「デッキ選択を上書き」オプションを使うと、現在のカードタイプから生成されたカードを配置するデッキを変更することができます。デフォルトでは、カードは ノートの「追加」ウィンドウで指定したデッキに配置されます。このオプションでデッキを指定すると、そのカードタイプから生成されたカードは、「ノートを追加」ウィンドウに記載されているデッキではなく、ここで指定したデッキに配置されます。これは、カードタイプごとにカードを別々のデッキに振り分けたい場合に便利です（例：英語学習の際に、「英→和」カードと「和→英」カードを別々のデッキに入れる）。カードの行き先が現在どのデッキになっているかは、「デッキの上書き」オプションを再度選択することで確認できます。
<!-- - The 'Deck Override' option allows you to change the deck that cards
  generated from the current card type will be placed into. By
  default, cards are placed into the deck you provide in the Add Notes
  window. If you set a deck here, that card type will be placed into
  the deck you specified, instead of the deck listed in the Add Notes
  window. This can be useful if you want to separate cards into
  different decks (for instance, when studying a language, to put
  production cards in one deck and recognition cards in another). You
  can check which deck the cards are currently going to by choosing
  Deck Override again. -->

- 「検索リストでの表示設定」オプションを使うと、検索ウィンドウのカード一覧の質問列と解答列での表示用に、簡略化したテンプレートを設定できます。詳細については、[検索リストでの表示設定](styling.md#browser-appearance) を参照してください。
<!-- - The 'Browser Appearance' option allows you to set different (perhaps
  simplified) templates for display in the Question and Answer columns
  of the browser; see [browser appearance](styling.md#browser-appearance) for more
  information. -->
