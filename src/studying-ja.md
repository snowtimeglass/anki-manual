# 学習 (Studying)
<!-- # Studying -->

<!-- toc -->

気に入ったデッキを見つけてダウンロードしたり、自分でノートをいくつか追加したりしたら、いよいよ学習を始めましょう。
<!-- When you have found a deck you like or entered some notes in, it’s time
to start studying. -->

## デッキ (Decks)
<!-- ## Decks -->

Ankiの学習は、現在選択しているデッキと、そのデッキに含まれるデッキ（サブデッキ）の範囲で行われます。
<!-- Study in Anki is limited to the currently selected deck as well as any
subdecks it contains. -->

「デッキ」画面では、あなたのデッキとサブデッキのリストが表示されます。
<!-- On the decks screen, your decks and subdecks will be displayed in a list: -->


![Decks screen](media/decks_screen.png)

各デッキの名前が表示された列の右側に、さらに３つの列があります。
* 「新規」の数字は、その日に学習できる状態にある、まだ学習していないカードの枚数を表しています。
* 「習得中」の数字は、現在集中的に学習しているカードの枚数を表しています。
* 「期日」の数字は、集中的な学習を終えた後の復習に適したタイミングを迎えたカードの枚数を表しています。
<!-- There are three columns. 'New' is the number of new
cards that are ready to be learnt that day. 'Learn' shows
the number of cards currently in learning. 'Due' is the count of waiting
reviews. -->

デッキをクリックすると、そのデッキが「現在のデッキ」として選択され、そのデッキの概要画面に切り替わります。
メインウィンドウ上部の「デッキ」をクリックすれば、いつでも、別のデッキを選ぶために「デッキ」画面に戻ることができます。
* メニューバーの「ツール」→「デッキを選択」のアクションを使えば、キーボード操作によって別のデッキを選ぶこともできます。
* <kbd>S</kbd> キーを押せば、「現在のデッキ」の概要画面に戻ることができます。
<!-- When you click on a deck, it will become the 'current deck', and Anki
will change to the study screen. You can return to the deck list to
change the currently selected deck at any time by clicking on “Decks” at
the top of the main window. (You can also use the Study
Deck action in the menu to select a new deck from the keyboard, or you
can press the <kbd>s</kbd> key to study the currently selected deck.) -->

<!-- ※※※※※※※※※※※※※※※※※※※※※※※※※
原文誤？）When you click on a deck, it will become the 'current deck', and Anki will change to the study screen. 
正？）When you click on a deck, it will become the 'current deck', and Anki will change to the deck overview screen.  
※※※※※※※※※※※※※※※※※※※※※※※※※※※※-->

各デッキの行の右端に表示される歯車マークのボタンをクリックすると、次の各操作を行うことができます。
* デッキの名前の変更
* デッキの削除
* デッキの[オプション](deck-options.md)（設定）の変更
* デッキの[エクスポート](exporting.md)


<!-- You can click the gears button to the right of a deck to rename or
delete a deck, change its [options](deck-options.md), or [export](exporting.md) it. -->

## 学習の概要
<!-- ## Study Overview -->

学習するデッキをクリックすると、その日に学習する予定のカードが何枚あるかを示す画面が表示されます。
この画面のことを「デッキ概要 (deck overview)」画面とよびます。
<!-- After clicking on a deck to study, you’ll see a screen that shows you
how many cards are due today. This is called the 'deck overview' screen: -->

![Study overview](media/study_overview.png)

その日に学習する予定のカードは上図のように「新規」「習得中」「復習」という[３つのタイプ](getting-started.md#types-of-cards)に分けられています。

もし、デッキのオプションで[「カードの兄弟を翌日に延期する」](#siblings-and-burying)が有効になっていて、実際に延期するカードがある場合、そのカードの枚数が下図のように灰色の数字で表示されます。

<!-- The cards are split into [three types](getting-started.md#types-of-cards): New, Learning, and To Review. 
If you have [Bury siblings](#siblings-and-burying) activated in your deck options, you 
may see how many cards will be buried in grey: -->

![Study overview (Buried Cards)](media/study_overview_buried_cards.png)

学習を始めるには、「**学習開始**」 ボタンをクリックしてください。その日に学習する予定のカードがなくなるまで、カードが表示され続けます。
<!-- To start a study session, click the **Study Now** button. Anki will
proceed to show you cards until the cards to be shown for the day have
run out. -->

学習中にキーボードの <kbd>S</kbd> キーを押すと、「デッキ概要」画面に戻ることができます。
<!-- While studying, you can return to the overview by pressing the <kbd>s</kbd> key
on your keyboard. -->

## 問題
<!-- ## Questions -->

カードが最初は問題だけが表示されます。問題に対する答えを考えた後、**解答を表示** ボタンをクリックするか、スペースキーを押すと、解答が表示されます。答えを思い出すのに少し時間がかかってもかまいせんが、一般的な目安としては、 10秒以内ぐらいに答えられなければ、思い出そうと努力し続けるよりも、解答を見るほうがよいでしょう。

解答を表示してから、自分で思い浮かべた答えと解答とを比べて、自分がどれぐらい覚えていたかを自己評価してAnkiに回答してください。もし、自分が思い浮かべた答えが不確かになってしまうようなら、[答えをキーボードで入力](templates/fields.md#checking-your-answer)して解答と見比べられるよう設定するこ

## 習得中カード / 再習得中カード
<!-- ## Learning/Relearning Cards -->

新規カードを学習するときや、答えを忘れてしまったカードをあらためて学習するとき、Ankiは、あなたがそのカードの内容を記憶するのを助けるために、そのカードを1回またはそれ以上の回数表示（出題）します。この各回の表示（出題）のことを「習得ステップ」といいます。習得ステップは初期設定では2段階（1分間隔を空けた表示と10分間隔を空けた表示）です。習得ステップの段階数と、各ステップまでの時間間隔は、 [デッキオプション](deck-options.md#new-cards)で変更できます。　

<!-- When learning new cards, or when relearning cards that you have
forgotten, Anki will show you the cards one or more times to help you
memorize them. Each time is called a 'learning step'. By default there
are two steps: 1 minute and 10 minutes. You can change the number of
steps and the delays between them in the [deck options](deck-options.md#new-cards). -->

習得ステップのカードでは、評価を回答するボタンは4種類あります:
<!-- There are four rating buttons when learning: -->

- **やり直し**：そのカードの最初のステップに戻ります。
<!-- - **Again** moves the card back to the first step. -->

- **難しい**：現在のステップをもう一度繰り返します。 
  - 最初のステップでは、次のステップまでの時間間隔は「やり直し」と「正解」の各間隔の平均値となります。
  - 最初のステップ以外では、次のステップまでの時間間隔は、現在のステップまでの時間間隔と同じとなります。
<!-- - **Hard** repeats the current step. 
  - If the card is on the first step, the delay will be the average of Again and Good.
  - After the first step, Hard repeats the previous delay. -->

- **正解**：そのカードを [次のステップ](deck-options.md#learning-steps)に進めます。
  - カードが最後のステップにある場合は、習得中カードを「卒業」し、「復習カード」に変わります。
  - 初期設定では、最後の習得ステップで正解したカードは、復習カードとして翌日に表示（出題）され、 その後、徐々に間隔を延ばしながら繰り返し表示されます（次のセクションを参照してください）。
<!-- - **Good** moves the card to the [next step](deck-options.md#learning-steps). If the card was on the final
step, the card is converted into a review card (it 'graduates'). By
default, once the card has reached the end of the learning steps, the
card will be shown again the next day, then at increasingly long delays
(see the next section). -->

- **簡単**：そのカードが最終ステップにない場合でも、そのカードを復習カードに変えます。 [初期設定](deck-options.md#easy-interval)では、そのカードは復習カードとして4日後に再び表示（出題）され、その後、徐々に間隔を延ばしながら繰り返し表示されます。
  - v1スケジューラーでは、再習得ステップ中は、「簡単」ボタンは表示されません。「簡単」と「正解」が同じ間隔であるためです。
  - [v2スケジューラー以降](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html)では、再習得ステップの間は、「簡単」を選ぶと、復習カードとして再び表示（出題）されるまでの期間が、「正解」を選んだ場合よりも1日増えます。

<!-- - **Easy** immediately converts the card into a review card, even if there
were steps remaining. [By default](deck-options.md#easy-interval), the card will be shown again 4 days
later, and then at increasingly long delays. In the v1 scheduler, the "Easy" button will not be
shown if you are in relearning mode as it would give the same interval
as “Good.” With the [v2 scheduler+](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html),
when cards are in relearning, the "Easy" button boosts the interval by 1 day. -->

あるカードを初めて学習するとき、その学習は1段階目の習得ステップとして位置づけられます。

つまり、初期設定では、カードの初回学習時に「**正解**」と回答すると、そのカードは10分後に再表示されます（2段階目の習得ステップ）。1段階目の習得ステップまでの時間間隔（1分）は出番のないまま、次の習得ステップに進むことになります。

一方、カードの初回学習時に「**やり直し**」と回答すると、そのカードは1分後に再表示されます（1段階目の習得ステップ）。このように、1段階目の習得ステップまでの時間間隔（1分）は、「**やり直し**」と回答した場合に使用されます。
<!-- ※※※※※※※※※※※※※※※※※※※※※※※※※
最後の文は独自。
※※※※※※※※※※※※※※※※※※※※※※※※※※※※-->
<!-- When cards are seen for the first time, they start at step one. This
means answering **Good** on a card for the first time will show it one
more time in 10 minutes, and the initial 1 minute step will be skipped.
If you push Again, though, the card will come back in 1 minute. -->
<!-- ※※※※※※※※※※※※※※※※※※※※※※※
原文改案
If you push Again
↓
If you push **Again**
※※※※※※※※※※※※※※※※※※※※※※※※※※※※-->

回答ボタンの選択には、キーボードの<kbd>1</kbd>、<kbd>2</kbd>、<kbd>3</kbd>、<kbd>4</kbd>キーを使うこともできます。例えば<kbd>1</kbd>キーを押すと「**やり直し**」を選択します。<kbd>Space</kbd>キーまたは <kbd>Enter</kbd>キーを押すと「**正解**」を選択します。
<!-- You can use the <kbd>1</kbd>, <kbd>2</kbd>, <kbd>3</kbd> and <kbd>4</kbd> keys on your keyboard to select a particular
button, where <kbd>1</kbd> is **Again**. Pressing <kbd>Space</kbd> or <kbd>Enter</kbd> will select
**Good**. -->

他に表示するカードがなくなれば、次のステップまでの時間間隔が完全に経過していなくても、前倒し許容時間まで経過した段階で習得中カードが再表示されます。次のステップまでの時間間隔を厳格に確保したい場合は、[[ツール]→[設定]→[学習]→[習得学習の前倒しの限度]](preferences.md)を0分に設定してください。
<!-- If there are no other cards to show you, Anki will show learning cards
again even if their delay has not elapsed completely. If you’d prefer to
wait the full learning delay, you can change this behaviour in
[Preferences>Scheduling>Learn Ahead Limit](preferences.md). -->

## 復習カード
<!-- ## Review Cards -->

習得ステップを終えたカードを復習するとき、評価を回答するボタンは4種類あります:
<!-- When a card has been previously learnt and is ready to be reviewed
again, there are four buttons to rate your answer: -->

- **やり直し** : あなたが正しく答えられなかった場合に押すボタンです。この回答によって、今後、そのカードが表示される頻度が上がります。
  - 復習カードに「やり直し」と回答する状態のことを、「忘却」といいます。 忘却したカードがどのように取り扱われるかについての詳細は、[「忘却」](deck-options.md#lapses)の項を参照してください。
<!-- - **Again** marks your answer as incorrect and asks Anki to show the card
more frequently in the future. The card is said to have 'lapsed'. Please
see the [lapses](deck-options.md#lapses) section for more information about how lapsed
reviews are handled. -->

- **難しい** : 初期設定では、この回答をすると、今回の表示までの間隔と比べて、次回の表示までの[間隔が少しだけ広がります](deck-options.md#hard-interval)。
  - 少ししか広がらない、とも言え、この後説明する「正解」の回答をした場合と比べて、そのカードが表示される頻度が上がることになります。
<!-- - **Hard** by default, shows the card at a [slightly longer delay](deck-options.md#hard-interval)
than last time, and tells Anki to show the card more frequently in the future. -->

- **正解** : この回答をすると、Ankiは今回の復習までの時間間隔が適切だったと判断し、そのカードの難易度を示す「易しさ」の数値を上げたり下げたりして調整する必要がないと判断します。 [「易しさ」の初期値](deck-options.md#starting-ease)は250％で、カードは次回、今回の復習までの間隔の約2.5倍の間隔を空けて表示されます。
  - 例えば、今回の復習までの間隔が10日間だった場合、次の復習までの間隔は約25日間となります。
<!-- - **Good** tells Anki that the last delay was about right, and the card
easiness doesn’t need to be adjusted down or up. At the [default starting
easiness](deck-options.md#starting-ease), the card will be shown again approximately 2 1/2 times longer
than the previous time, so if you had waited 10 days to see the card
previously, the next delay would be about 25 days. -->

- **簡単** : この回答をすると、Ankiは、今回の復習までの間隔が短すぎた（＝もっと長くても問題ない）と判断し、次の復習までの間隔は[「正解」を回答した場合よりも広がります](deck-options.md#easy-bonus)。その結果、「正解」の回答をした場合と比べて、そのカードが表示される頻度は下がることになります。
  - 「簡単」の回答は復習間隔を急激に延ばすので、本当に簡単すぎるカードに対してだけ使うのがよいでしょう。通常は、「正解」ボタンを使うことを強くおすすめします。

習得中カードの場合と同様に、キーボードの<kbd>1</kbd>、<kbd>2</kbd>、<kbd>3</kbd>、<kbd>4</kbd> キーで回答を選択することができます。<kbd>Space</kbd>キーまたは<kbd>Enter</kbd>キーを押すと、「正解」が選択されます。
<!-- As with learning cards, you can use <kbd>1</kbd>, <kbd>2</kbd>, <kbd>3</kbd> and <kbd>4</kbd> on the keyboard to select an
answer. Pressing the <kbd>spacebar</kbd> or <kbd>Enter</kbd> will select **Good**. -->

アルゴリズムがどのように働いているかについての詳細は、[「デッキオプション」](deck-options.md)の項目と[FAQ（よくある質問）](https://faqs.ankiweb.net/what-spaced-repetition-algorithm.html)を参照してください。
<!-- See [Deck Options](deck-options.md) and the [FAQ](https://faqs.ankiweb.net/what-spaced-repetition-algorithm.html)
to learn more about how the algorithm works. -->

## 課題カウント
<!-- ## Due Counts -->

質問側（表面）だけが表示されている場合、Ankiは画面の下部に例えば「 6 + 9 + 59 」のような3つの数字を表示します。これらはそれぞれ、新規カード（青）、習得中カード（赤）、復習カード（緑）を表しています。この数字を表示させたくない場合は、Ankiの[設定](preferences.md)でオフにすることができます。
<!-- When only the question is shown, Anki shows three numbers like 6 + 9 + 59
at the bottom of the screen. These represent the new cards (blue), cards in
learning (orange), and cards to review (green). If you’d prefer not to see the numbers,
you can turn them off in Anki’s [preferences.](preferences.md) -->

![Due Counts](media/due_counts.png)

v1スケジューラーでは、_カードの枚数_ ではなく、そのキュー内のすべてのカードを終了させるために必要な　_学習回数_ をカウントしています。間違えた（＝やり直す）カードに対して複数の習得ステップを設定している場合、そのカードを複数回表示する必要があるため、カードに「やり直し」と回答すると数字が2つ以上増えることになります。
<!-- In the v1 scheduler, the numbers count _reviews_ needed to finish all the
cards in that queue, not the number of _cards_. If you have multiple
steps configured for lapsed cards, the number will increase by more than
one when you fail a card, since that card needs to be shown several times. -->

v2スケジューラー以降では、各数字は　_カードの枚数_ を示しているため、カードに「やり直し」と回答すると、残りの習得ステップ数にかかわらず数字が1つ増えます。
<!-- From the v2 scheduler, the numbers count _cards_, so the number will always
increase by one regardless of the steps remaining. -->

解答を表示すると、各回答ボタンの上に、カードが次回表示されるまでの時間間隔（例. 3分、1時間、2日）が表示されます。時間間隔を表示したくない場合は、 [設定](preferences.md)で表示を無効にできます。
<!-- When the answer is shown, Anki shows an estimate of the next time a card
will be shown above each button. If you’d prefer not to see the
estimates, you can disable them in Anki’s [preferences](preferences.md). -->

## ファズの要素
<!-- ## Fuzz Factor -->

同じタイミングで学習を開始し、同じ評価を受けたカードどうしがまとまったままで常に同じ日に表示されてしまうことを防ぐために、Ankiではカード学習で回答ボタンが選択された際、少量のランダムな「ファズ（ゆらぎ）」を学習時間の間隔に適用します。このファズは、[v3スケジューラー](https://faqs.ankiweb.net/the-2021-scheduler.html)が有効な場合に回答ボタンの上に表示されます。以前のバージョンを使用していて、選択した時間間隔と実際にカードが表示される時間間隔に若干の不一致がある場合は、この機能が原因である可能性があります。
<!-- When you select an ease button on a review card, Anki also applies a small amount of random “fuzz”
to prevent cards that were introduced at the same time and given the same ratings
from sticking together and always coming up for review on the same day. This fuzz
will appear on the answer buttons when the [v3 scheduler](https://faqs.ankiweb.net/the-2021-scheduler.html) is enabled, so if
you are using a previous version and you’re noticing a slight discrepancy between
what you select and the intervals your cards actually get, this is probably the
cause. -->

また、習得中カードについても、常に同じ順番で表示されないように最大5分の遅延が追加されますが、回答ボタンの上の時間間隔には反映されません。この機能をオフにすることはできません。
<!-- Learning cards are also given up to 5 minutes of extra delay so that they
don’t always appear in the same order, but answer buttons won't reflect that. It
is not possible to turn this feature off. -->

## 「編集」と「その他」
<!-- ## Editing and More -->

学習画面左下の「**編集**」ボタンをクリックすると、現在のノートを編集することができます。編集が終わると、学習に戻ります。編集画面は、「[ノートを追加](editing.md)」画面とよく似ています。
<!-- You can click the **Edit** button in the bottom left to edit the current
note. When you finish editing, you’ll be returned to study. The editing
screen works very similarly to the [add notes](editing.md) screen. -->

学習画面の右下の「**その他**」ボタンをクリックすると、現在のカードまたはノートに対して実行できる操作が表示されます：
<!-- At the bottom right of the review screen is a button labeled **More**.
This button provides some other operations you can do on the current
card or note: -->

- [**カードにフラグをつける**](edit.md#using-flags)：カードに色のついたマーカーを追加したり、それを解除したりします。フラグは学習画面で表示され、ブラウザ画面ではフラグのついたカードを検索することができます。これは、帰宅後に単語を調べるなど、後でカードに対して何らかの対応をしたい場合に役立ちます。Anki 2.1.45以降では、[ブラウザ](browsing.md)でフラグの名前を変更することもできます。
<!-- - [**Flag Card**](editing.md#using-flags): Adds a colored marker to the card, or toggles it off. Flags will appear during
  study, and you can search for flagged cards in the Browse screen. This is useful
  when you want to take some action on the card at a later date, such as looking
  up a word when you get home. If you're using Anki 2.1.45+, you can also rename flags
  from the [browser](browsing.md). -->

- **カードを今日はパス / ノートを今日はパス**：現在のカード または 現在のノートのすべてのカード を翌日まで学習画面から隠します。（当日中にパスを解除したくなった場合は、[デッキ概要](studying.md#study-overview)画面の「パスを解除」ボタンをクリックしてください。）この機能は、そのカードに今すぐ答えられない場合や、別の機会に答えたい場合に役立ちます。なお、カードを学習した場合に[同じノートから生成された別のカードを自動的に翌日にパスする](study.md#siblings-and-burying)よう設定しておくことも可能です。

  旧スケジューラーでは、習得中のカードをパスする場合は、そのカードはパスされる前に新規カードのキューまたは復習カードのキューに戻されます。

  しかし、[2.1スケジューラー](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html)では、カードをパスしても、カードの習得ステップはリセットされません。

<!-- 
- **Bury Card / Note**: Hides a card or all of the note’s cards from review until the next day.
  (If you want to unbury cards before then, you can click the “unbury”
  button on the [deck overview](studying.md#study-overview) screen.) This is useful if
  you cannot answer the card at the moment or you want to come back to it
  another time. Burying can also [happen automatically](studying.md#siblings-and-burying) for
  cards of the same note.

  With the old scheduler, if cards were in learning when they are buried,
  they are moved back to the new card queue or review queue prior to being
  buried.

  With the [2.1 scheduler](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html),
  however, burying cards does not reset a card's learning steps.
   -->

- **カードの学習進度をリセット**: 現在のカードを[新規カードの最後](browsing.md#cards)に移動します。
<!-- 
- **Forget card**: Move current card to [the end of the new queue](browsing.md#cards).
 -->

  Anki 2.1.50以降、AnkiはV3スケジューラーで新規カードを初めて学習した時、そのカードの位置（順序）を記憶します。「可能な限り元の位置を復元」オプションを有効にすると、カードをリセットしたときに元の位置に戻すことができます。
  <!-- ※※※※※※※※※※※※※※※※※※※※※※※※※
  原文："Restore original position"
  訳文；pontoonの"Restore original position where possible"を反映。ただし機能の説明内容には反映されていない。
   -->
  <!-- 
  From Anki 2.1.50+, Anki will remember the original order of a new card when it is first studied
with the V3 scheduler. The "Restore original position" option allows you to reset the card back
to its original position when you forget it.
 -->

  「学習回数と忘却回数をリセット」オプションを有効にすると、カードの学習回数と忘却回数のカウントが0に戻ります。このオプションを有効にしても、カード情報画面の下部に表示される学習履歴自体は削除されずに残ります。
  <!-- 
  The "Reset repetition and lapse count" option, if enabled, will set the review and failure counters
for the card back to zero. It does not remove the review history that is shown at the bottom of the
card info screen.
 -->

- **期日を設定**: カードを復習キューに入れ、[特定の日に期日を指定](browsing.md#cards)します。
<!-- 
- **Set Due Date**: Put cards in the review queue, and [make them due on a certain date.](browsing.md#cards)
 -->

- **カードを休止 / ノートを休止**: カード または ノートのすべてのカード を、手動でその休止を解除しない限り、学習画面から隠し続けます。（解除方法は、[検索]→[カード]→[休止/休止解除 を切り替える]）

  これは、しばらくそのカード または ノート の学習をしたくないいが削除はしたくない、という場合に便利です。
  - 旧スケジューラーでは、カードを習得中（または再習得中）に休止した場合、カードは休止の前に新規カードキュー（または復習キュー）に戻ります。
  <!-- ※※※※※※※※※※※※※※※※※※※※※※※※※
  しばらくそのカード または ノート の学習を・・・
  →原文では、単に「ノート」。実際は「カード」の方が適切か。：This is useful if you want to avoid reviewing the note for some time,
   -->

  - [2.1スケジューラー](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html)では、カードを休止してもカードの習得ステップはリセットされません。
<!-- 
- **Suspend Card / Note**: Hides a card or all of the note’s cards from review until they are
  manually unsuspended (by clicking the suspend button in the browser).
  This is useful if you want to avoid reviewing the note for some time,
  but don’t want to delete it.
  With the old scheduler, if cards were in learning when they are
  suspended, they are moved back to the new card queue or review queue
  prior to being suspended.

  With the [2.1 scheduler](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html),
  however, suspending cards does not reset a card's learning steps.
 -->

- **オプション**: 現在のデッキの[オプション](deck-options.md)を編集します。
<!-- - **Options**: Edit the [options](deck-options.md) for the current deck. -->

- **カード情報**: カードの[統計情報](stats.md#card-info)を表示します。
<!-- - **Card Info**: Displays [statistical information](stats.md#card-info) about the card. -->

- **直前カード情報**: 一つ前のカードの[統計情報](stats.md#card-info)を表示します。
<!-- - **Previous Card Info**: Displays [statistical information](stats.md#card-info) about the previous card. -->

- [**ノートにマーク**](editing.md#the-marked-tag): 現在のノートに “marked” というタグを付けます。こうすることで、ブラウザで検索しやすくなります。個々のカードにフラグを付けるのと似ていますが、この機能はノートにタグを付けるので、もしそのノートが複数のカードを持っている場合、それらのカードすべてが検索されます。ほとんどのユーザーは、このマーク機能よりも、フラグ機能の方が使いやすいと思うでしょう。
<!-- - [**Mark Note**](editing.md#the-marked-tag): Adds a “marked” tag to the current note, so it can be easily found in the
  browser. This is similar to flagging individual cards, but works with a tag
  instead, so if the note has multiple cards, all cards will appear in a search
  for the marked tag. Most users will want to use flags instead. -->

- **コピーを作成**: 現在のノートの[複製](browsing.md#finding-duplicates)をエディタで開きます。内容に少し手を加えるだけで簡単にカードのバリエーションを増やすことができます。デフォルトでは、複製したカードは元のカードと同じデッキに作成されます。
<!-- - **Create Copy**: Opens a [duplicate](browsing.md#finding-duplicates) of the current
  note in the editor, which can be slightly modified to easily obtain variations of your cards.
  By default, the duplicate card will be created in the same deck as the original. -->

- **ノートを削除**: ノートと そのノートから作成されたすべてのカード を削除します。
<!-- - **Delete Note**: Deletes the note and all of its cards. -->

- **オーディオを再生**: カードの表面または裏面にオーディオ（音声データ）がある場合に、再び再生します。
<!-- - **Replay Audio**: If the card has audio on the front or back, play it again. -->

- **オーディオを一時停止**: 再生中のオーディオを一時停止します。
<!-- - **Pause Audio**: Pauses the audio if it is playing. -->

- **オーディオ-5秒 / オーディオ+5秒**: 現在再生中のオーディオの再生位置を5秒前/後ろに移動します。
<!-- - **Audio -5s / +5s**: Jump backwards / forward 5 seconds in the currently playing audio. -->

- **自分の声を録音**: 自分の発音を確認するためにマイクから録音します。この録音は一時的なもので、次のカードに移動すると消えます。オーディオをカードに永続的に追加したい場合は、編集ウィンドウ（エディタ）で行うことができます。
<!-- - **Record Own Voice**: Record from your microphone for the purposes of checking your
  pronunciation. This recording is temporary and will go away when you
  move to the next card. If you want to add audio to a card permanently,
  you can do that in the edit window. -->

- **自分の声を再生**: 先に録音しておいた自分の声を再生します（解答を表示した後などに）。
<!-- - **Replay Own Voice**: Replay the previous recording of your voice (presumably after showing
  the answer). -->

## Display Order
<!-- ## Display Order -->

学習を開始すると、選択したデッキのカードと、そのデッキに含まれているデッキのカードを表示します。つまり、「英語」デッキを選択すると、そのサブデッキ「英語::単語」のカードや、同じくサブデッキ「英語::教科書::レッスン1」のカードも表示されます。
<!-- Studying will show cards from the selected deck and any decks it
contains. Thus, if you select your “French” deck, the subdecks
“French::Vocab” and “French::My Textbook::Lesson 1” will be shown as
well. -->

Ankiがデッキからカードを取り出す方法は、使用するアルゴリズムによって異なります：
<!-- The way Anki fetches cards from the decks depends on the algorithm used: -->

- v1スケジューラーでは、<span>選択した</span>デッキにサブデッキがある場合、[各<span>サブ</span>デッキごとに順番に](studying.md#display-order)カードが表示されます。
<!-- - With the v1 scheduler, when a deck has subdecks, the cards will appear from [each deck in
  turn](studying.md#display-order). -->

- [v2スケジューラー](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html)では、
  <span>選択した</span>デッキにサブデッキがある場合、表示するカードはすべてのサブデッキから一度に取り出されます。サブデッキの出題枚数上限は無視され、<span>選択した</span>デッキの出題枚数上限のみが適用されます。
<!-- - With the [v2 scheduler](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html),
  when a deck has subdecks, reviews are taken from all children decks
  at once. The review limit of the child decks is ignored - only the limit of the
  deck you clicked on applies. -->

- [v3スケジューラー](https://faqs.ankiweb.net/the-2021-scheduler.html)では、
  各サブデッキの出題枚数上限も適用されるため、<span class=unsure >カードをデッキの順序で見る必要はありません。</span>詳しくはデッキオプションの[出題カードの順序の並び替え](deck-options.md#review-sort-order)の項目を参照してください。
  <span class=unsure></span><!-- ↑リンク先が妥当かどうか疑問 -->
<!-- - With the [v3 scheduler](https://faqs.ankiweb.net/the-2021-scheduler.html)
  each child deck's limit is also enforced, and you do not need to see the cards
  in deck order either. See the [deck options](deck-options.md#review-sort-order) section of the manual for more information. -->

By default, for new cards, Anki fetches cards from the decks in
alphabetical order. So in the above example, you would get cards first
from “French”, then “My Textbook”, and finally “Vocab”. You can use this
to control the order cards appear in, placing high priority cards in
decks that appear higher in the list. When computers sort text
alphabetically, the “-” character comes before alphabetical characters,
and “\~” comes after them. So you could call the deck “-Vocab” to make
them appear first, and you could call the other deck “\~My Textbook” to
force it to appear after everything else.

New cards and reviews are fetched separately, and Anki won’t wait until
both queues are empty before moving on to the next deck, so it’s
possible you’ll be exposed to new cards from one deck while seeing
reviews from another deck, or vice versa. If you don’t want this, click
directly on the deck you want to study instead of one of the parent
decks.

Since cards in learning are somewhat time-critical, they are fetched
from all decks at once and shown in the order they are due.

To control the order reviews from a given deck appear in, or change new
cards from ordered to random order, please see the [deck
options](deck-options.md). For more fine-grained ordering of new cards, you
can change the order in the [browser](browsing.md).

## Siblings and Burying

Recall from [the basics](getting-started.md) that Anki can create more than one
card for each thing you input, such as a front→back card and a
back→front card, or two different cloze deletions from the same text.
These related cards are called 'siblings'.

When you answer a card that has siblings, Anki can prevent the card’s
siblings from being shown in the same session by automatically 'burying'
them. Buried cards are hidden from review until the clock rolls over to
a new day or you manually unbury them using the “Unbury” button that’s
visible at the bottom of the [deck overview](studying.md#study-overview) screen. Anki
will bury siblings even if the siblings are not in the same deck (for
instance, if you use the [deck override](templates/intro.md) feature).

You can enable burying from the [deck options](deck-options.md) screen -
there are separate settings for new cards and reviews.

Anki will only bury siblings that are new or review cards. It will not
hide cards in learning, as time is of the essence for those cards. On
the other hand, when you study a learning card, any new/review siblings
will be buried.

Note: A card cannot be buried and suspended at the same time. Suspending a
buried card will unbury it. Burying a suspended card does not work on Anki
2.1.49+, whereas on earlier versions, it will unsuspend the card.

## Keyboard Shortcuts

Most of the common operations in Anki have keyboard shortcuts. Most of
them are discoverable in the interface: menu items list their shortcuts
next to them, and hovering the mouse cursor over a button will generally
show its shortcut in a tooltip.

When studying, either <kbd>Space</kbd> or <kbd>Enter</kbd> will show the answer. When the
answer is shown, you can use <kbd>Space</kbd> or <kbd>Enter</kbd> to select the Good button.
You can use the <kbd>1</kbd>-<kbd>4</kbd> keys to select a specific ease button. Many people
find it convenient to answer most cards with <kbd>Space</kbd> and keep one finger
on <kbd>1</kbd> for when they forget.

The "Study Deck" item in the Tools menu allows you to quickly switch to
a deck with the keyboard. You can trigger it with the '/' key. When
opened, it will display all of your decks and show a filter area at the
top. As you type characters, Anki will display only decks matching the
characters you type. You can add a space to separate multiple search
terms, and Anki will show only decks that match all the terms. So “ja 1”
or “on1 ja” would both match a deck called “Japanese::Lesson1”.

## Falling Behind

If you fall behind in your reviews, Anki will prioritize cards that have
been waiting the longest. It does this by taking the cards that have
been waiting the longest and showing them to you in a random order up
until your daily review limit. This ordering ensures that no cards will
be left waiting indefinitely, but it means that if you introduce new
cards, their reviews won’t appear until you’ve gotten through your
backlog.

If you wish to change the order of the overdue reviews, you can do so by
creating a [filtered deck](filtered-decks.md).

When you answer cards that have been waiting for a while, Anki factors
in that delay when determining the next time a card should be shown.
Please see the section on Anki’s spaced-repetition
[algorithm](https://faqs.ankiweb.net/due-times-after-a-break.html) for more information.
