# デッキオプション
<!-- # Deck Options -->

<!-- toc -->

デッキオプションは主に、Ankiがカードをスケジュールする方法を調整します。調整を開始する前に、デフォルトの設定を数週間試し、Ankiがどのような働きをしているかの感覚をつかむことをお勧めします。不用意にオプションをいじるとAnkiの効果が低下してしまうおそれがあるので、オプションの変更は、必ずそのオプションの機能を理解してから行うようにしてください。
<!-- 
Deck options primarily control the way Anki schedules cards. It is recommended
that you spend a few weeks with the defaults to get a feel for how Anki works
before you start adjusting options. Please make sure you understand the options
before changing them, as mistakes could reduce Anki's effectiveness.
 -->

デッキオプションへのアクセス方法は次の通りです：

- `デッキ`画面の各デッキにカーソルを合わせたときに表示される歯車ボタンをクリックする。
- `デッキ`画面でデッキを選択し, デッキ概要画面の下側にある`オプション`をクリックする。
- 学習中に`その他` > `オプション` をクリックする。
- 学習中に `o` キーを押す。
<!-- 
Deck options are accessed by:

- Clicking the gear icon on the `Decks` screen.
- Selecting a deck on the `Decks` screen, and then clicking `Options`
  at the bottom of the screen.
- Clicking on `More` > `Options` while in review mode.
- Pressing `o` while in review mode. -->

このページでは、Anki 2.1.45以降でV2またはV3スケジューラーを有効にした場合に表示されるオプションについて説明します。

- それより古いバージョンでは、一部のオプションは利用できなかったり、別のセクションに表示されていたりします。
- Anki2.1.50以降では、V1スケジューラはサポートされなくなりました。まだV2またはV3にアップデートしていない場合、2.1.50以降でカードを学習しようとすると、アップデートを促すプロンプトが表示されます。
- デッキオプションについて理解を深めるためには、Ankiフォーラム内の次の内容も役立ちます。
  - [Deck Options Explained（デッキオプションの説明）](https://forums.ankiweb.net/t/deck-options-explained/213)
  - [Deck options in a Mental Map（デッキオプションのメンタルマップ）](https://forums.ankiweb.net/t/deck-options-in-a-mental-map/15757)

<!-- 
This page describes the options shown in Anki 2.1.45+, when you have the v2 or
v3 scheduler enabled. On older versions, some options will not be available, or
will appear in a different section. Please keep in mind that the V1 scheduler
is no longer supported in Anki 2.1.50+. If you have not yet updated to V2 or V3,
you will be prompted to update when you attempt to review cards in 2.1.50+.

For more info on deck options, please check:

- [Deck Options Explained](https://forums.ankiweb.net/t/deck-options-explained/213)
- [Deck options in a Mental Map](https://forums.ankiweb.net/t/deck-options-in-a-mental-map/15757) -->

## プリセット
<!-- ## Presets -->

Ankiでは、異なるデッキ間でデッキオプションの設定内容を共有できるので、多くのデッキオプションの設定内容を一度に簡単に更新することができます。デッキ間での共有を行うために、デッキオプションの一連の設定を一つのグループとして扱い、これを「**プリセット**」といいます。デフォルトでは、新しく作成されたデッキはすべて同じプリセットを使用します。
<!-- Anki allows you to share options between different decks, to make
updating options in many decks at once easy. To do this, options are
grouped into _presets_. By default, all newly created decks use
the same preset. -->

「あるデッキの設定を変更したいが、他のデッキの設定は変更したくない」という場合は、デッキオプション画面の右上にある下向き矢印（∨）ボタンをクリックしてください。選択肢は以下の通りです：
<!-- If you’d like to alter the settings on one deck but not other decks, click the
arrow icon in the top right of the Deck Options window. The options are: -->

- **保存**: デッキオプション画面を開いてから変更した内容をすべて保存します。
- **プリセットを新規作成**: 新しいプリセットを作成します。内容はデフォルトのデッキオプションと同じです。
- **このプリセットを複製**: 現在表示しているプリセットを複製します。「一部のオプションの設定内容を変更したいが、大多数のオプションの設定内容をそのままにしておきたい」という場合に選択すると便利です。
- **このプリセットの名前を変更**: 現在表示しているプリセットの名前を変更します。
- **このプリセットを削除**: 現在表示しているプリセットを削除します。これを行うと、次回の同期で一方向の同期を行う必要があります。
- **保存してサブデッキにも適用**: 上記の「**保存**」の操作に加え、保存したプリセットを、現在選択中のデッキのすべてのサブデッキに対しても適用します。
<!-- - **Save**: Saves all modifications you've made since opening the deck options screen.
- **Add**: Add a new preset, with the default options.
- **Clone**: Clone your current present, which is useful if you
  just want to modify certain options, keeping the rest as they are.
- **Rename** Changes the name of the current preset.
- **Delete** Deletes the current preset. This will require that the next sync is
  a one-way sync.
- **Save to all subdecks**. Like _Save_, but also assigns the selected preset to all
  subdecks of the currently selected deck. -->

デッキオプションで設定した内容は、遡っては適用されません。例えば「もう一度」と回答した後の学習ステップを調整するオプションを変更しても、オプションを変更する前に「もう一度」と回答したカードには、変更後の学習ステップではなく、変更前の学習ステップが適用されたままとなります。
<!-- Deck Options are not retroactive. For example, if you change an option that
controls the delay after failing a card, cards that you failed prior to
changing the option will have the old delay, not the new one. -->

## サブデッキ
<!-- ## Subdecks -->

デッキにサブデッキがある場合、各デッキに異なるプリセットを割り当てることができます。Ankiはカードを表示する際、そのカードがどのサブデッキに入っているかを確認し、そのデッキのオプションを使用します。ただし、例外もあります：
<!-- If your deck has subdecks, each deck can optionally be assigned a different preset.
When Anki shows a card, it will check which subdeck the card is in, and use the options
for that deck. There are some exceptions: -->

- 一日の新規カード導入枚数 と 一日の復習枚数 の各 [上限](#daily-limits) としていずれのオプションを使用するかは、選択しているスケジューラーのバージョンによって異なります。
- V3スケジューラーの[表示順序](#display-order)オプションは、表示中のカードのデッキではなく、学習を開始する際に選択したデッキのオプションが使用されます。
<!-- - The new cards/day and reviews/day [limits](#daily-limits) behave differently
  depending on the scheduler version you have selected.
- The [display order](#display-order) options in the v3 scheduler are taken from the
  deck you select to study, not the deck of the current card. -->

たとえば、次のコレクションがあるとします:


    - デッキA (プリセット1)
      - デッキA::サブデッキB (プリセット2)
        - カードB1
        - カードB2
<!-- 
For example, let's say you have this collection:

    - Deck A (Preset 1)
      - Deck A::Subdeck B (Preset 2)
        - Card B1
        - Card B2
 -->
プリセット1とプリセット2は、次の2項目以外は同じであるとします:

- プリセット1:
  - 「新規カード」の「学習ステップ」: 1m 10m
  - 「表示順序」の「新規カード表示のタイミング」: 復習に混ぜ込む
- プリセット2:
  - 「新規カード」の「学習ステップ」: 20m 2h
  - 「表示順序」の「新規カード表示のタイミング」: 復習の後に表示
<!-- 
Preset 1 and 2 are identical, with two exceptions:

- Preset 1:
- New Cards - Learning steps: 1m 10m
- Display Order - New/review priority: Mix with reviews
- Preset 2:
- New Cards - Learning steps: 20m 2h
- Display Order - New/review priority: Show after reviews
 -->

その場合、デッキAを選択して学習を開始すると:

- 新規カードの学習ステップはすべて「 1m 10m 」になります（プリセット1が適用されます）<!-- 。。。誤り？　実際は「 20m 2h 」＆「プリセット2が適用」？ -->
- 新規カードはすべて、復習に混ぜ込まれます（プリセット1が適用されます）

一方、デッキBを選択して学習を開始すると:

- 新規カードの学習ステップはすべて「 20m 2h 」になります（プリセット2が適用されます）
- 新規カードはすべて、復習の後に表示されます（プリセット2が適用されます）

<!-- 
If you choose to study Deck A:

- Learning steps for all new cards will be 1m 10m (preset 1 applies)
- All new cards will be mixed with reviews (preset 1 applies)

If you choose to study Subdeck B:

- Learning steps for all new cards will be 20m 2h (preset 2 applies)
- All new cards will be shown after reviews (preset 2 applies)
 -->

## 一日の上限
<!-- ## Daily Limits -->

### 一日の新規カード導入枚数の上限
<!-- ### New Cards/Day -->

Ankiを開いた日に新規カードを何枚まで導入（＝学習を開始）できることにするか、を設定します。この枚数は当日限りのものであり、翌日以降に累積されることはありません。つまり、ある日、設定した上限より少ない枚数しか学習しなかったり、まったく学習しなかったりしても、翌日の上限は増えたりせず、元のままです。

<!-- Controls how many new cards are introduced each day you open the program. If you
study fewer than the limit, or miss a day, the next day the counts will be back
to your limit - they do not accumulate. -->

デッキどうしが入れ子状になっている場合（例：「親デッキ」と「親デッキ::子デッキ」と「親デッキ::子デッキ::孫デッキ」）、上限の適用の仕方はスケジューラーのバージョンによって異なります。
<!-- When decks are nested (eg Parent, Parent::Child, Parent::Child::Grandchild),
the way the limits are applied depends on the scheduler version. -->

- V1では、どちらのデッキをクリックした場合も、親デッキの上限を子デッキに適用します。
- V2では、新規カードについてはV1と同様となります。復習カードについては、クリックした方のデッキの設定を適用します。
- V3では、クリックしたデッキと、その中の各デッキの上限がそれぞれ適用されます。クリックしたデッキの親デッキの上限は無視されます。
  
<!-- - V1 applies parent limits to children, regardless of which deck you click on
- V2 behaves similarly to V1 for new cards. For reviews, only the limits of
  the deck you click on are honored.
- V3 honors the limits of the deck you click on, and any decks inside it.
  Limits from parents above the deck you clicked on are ignored. -->

詳細は、[V3スケジューラー](https://faqs.ankiweb.net/the-2021-scheduler.html#daily-limits)のページをご参照ください。

<!-- For more information, please see the [v3 scheduler](https://faqs.ankiweb.net/the-2021-scheduler.html#daily-limits) page. -->

新規カードを学習すると、一日あたりの復習回数が一時的に増加します。新しく学習した内容は、学習間隔が大きく広がる前に短期間で何度も繰り返す必要があるからです。たとえば毎日20枚ずつ新規カードを学習していくと、一日あたりの復習回数は約200枚ほどになります。一日あたりの新規カードを減らしたり、復習の負担が減るまで新規カードの導入を停止したりすれば、復習回数を減らすのに役立ちます。Ankiを張り切って使い始めて最初の数日間で何百枚もの新規カードを学習して、そのうち、必要な復習量の急増に圧倒されてしまう、というのは失敗パターンの一つです。

<!-- Studying new cards will temporarily increase the number of reviews you need to
do a day, as freshly learnt material needs to be repeated a number of times
before the delay between repetitions can increase appreciably. If you are
consistently learning 20 new cards a day, you can expect your daily reviews to
be roughly about 200 cards/day. You can decrease the reviews required by
introducing fewer new cards each day, or by turning off new card display until
your review burden decreases. More than one Anki user has excitedly studied
hundreds of new cards over their first few days of using the program, and then
become overwhelmed by the reviews required. -->

### 一日の復習枚数の上限
<!-- ### Maximum Reviews/Day -->

Ankiを開いた日に何枚まで復習できることにするか、を設定します。上限に達すると、期日を迎えた復習カードがまだ残っていても、その日はそれ以上復習カードを表示しません。

この設定は、学習を続けていくにあたって、日々の期日カードの枚数を均等化するのに役立ちます。また、学習が少し途絶えてから再開した際に、たまった期日カードに圧倒されることなく一定のペースで取り組みたい場合にも役立ちます。

この設定によって非表示となった復習カードがある場合、学習セッション終了時の「おめでとう」画面に、それを知らせるメッセージが表示されます。時間があれば上限を上げるのが望ましい、という旨のメッセージも、併せて表示されます。
<!-- Allows you to set an upper limit on the number of reviews to show each day.
When this limit is reached, Anki will not show any more review cards for the
day, even if there are some waiting. If you study consistently, this setting can
help to smooth out occasional peaks in due card counts, and can save you from a
heart attack when returning to Anki after a week off. When reviews have been
hidden due to this option, a message will appear in the congratulations screen,
suggesting you consider increasing the limit if you have time. -->

[V3スケジューラー](https://faqs.ankiweb.net/the-2021-scheduler.html#daily-limits)とV1スケジューラーでは、新規カードの場合と同様に、選択したデッキの中のデッキ（子デッキ、孫デッキ、…）の上限より、選択したデッキ（親デッキ）自体の上限が優先されます。
<!-- In [the v3 scheduler](https://faqs.ankiweb.net/the-2021-scheduler.html#daily-limits) and
v1 schedulers, the counts are affected by parents/selected decks in the same way
as new cards. -->

V2スケジューラーでは、選択したデッキの上限のみが適用され、親デッキや子デッキの上限は無視されます。
<!-- In the v2 scheduler, the limit is taken solely from the deck you select - any
limits on its parents or child decks are ignored. -->

V3スケジューラーでは、間隔が１日以上の習得中カードも復習枚数に含まれるため、それらの習得中カードも、この枚数制限の対象になります。
<!-- The v3 scheduler includes learning cards with a 1+ day delay in the review count,
so those learning cards will be subject to the daily limit. -->

### 復習枚数の上限に関係なく新規カードを導入する
<!-- ### New cards ignore review limit -->

[v3スケジューラー](https://faqs.ankiweb.net/the-2021-scheduler.html#daily-limits)を使用する場合、初期設定では、新規カードの導入枚数は復習枚数によっても制限されることに注意してください。

- 例えば、復習枚数の上限を200枚に設定していて、復習の期日を迎えたカードが190枚ある場合、新規カードの導入枚数は最大で10枚となります。もし復習の期日を迎えたカードの枚数が上限（前の例では200枚）に達している場合は、新規カードは導入されません。
  - 「期日を迎えた復習カードがたまっていても新規カードを導入したい」という場合は、復習カードを休止するか、復習枚数の上限を上げることによって、それが可能になります。
  - とは言え、復習を延滞しているときにさらに新規カードを導入しても、復習の遅れをさらに悪化させるだけなので、遅れを解消するまでは新規カードの導入を控えることをお勧めします。
<!-- If using [the v3 scheduler](https://faqs.ankiweb.net/the-2021-scheduler.html#daly-liimits),
please keep in mind that the new count is capped by the review count by default. If your
review limit is set to 200, and you have 190 reviews waiting, a maximum of 10
new cards will be introduced. If your review limit has been reached, no new
cards will be shown. 
If you have a backlog of reviews and still want to
introduce new cards, you can do so by suspending the reviews, or increasing your
review limit. That said, it is recommended you hold off on new cards until you
catch up instead, as introducing more new cards when you're behind will only
make the backlog worse. -->

Anki 2.1.61以降では、上記の制限が解除可能になりました。この「
復習枚数の上限に関係なく新規カードを導入する」をオンにすることによって、上記の制限を常時無効にすることができます。
<!-- From Anki 2.1.61 this feature is optional, and can be deactivated globally from the deck options screen. -->

### デッキ独自の一日の上限
<!-- ### Per-Deck Daily Limits -->

Anki 2.1.55以降では、同じプリセットを異なるデッキ/サブデッキに使用することが可能になりました。これにより、その目的のためだけにプリセットを複製する必要がなくなり、また、多くのデッキが入れ子になっている場合に、サブデッキに個別の上限を設定するのが簡単になりました。

<!-- From version 2.1.55 it is possible to use the same preset for different decks / subdecks, with customized
limits for each one of them. This eliminates the need to create cloned presets just for that
purpose, and makes it easier to set custom limits on sub-decks when you have many nested decks. -->

オプションは次の通りです：

- プリセット: この上限は、このプリセットを使用しているすべてのデッキで共有されます。
- このデッキ この上限は、このデッキにのみ適用されます。プリセットの上限より優先されます。
- 今日だけ: このデッキの上限を一時的に変更します。

<!-- 
The options are:

- Preset: The limit is shared with all decks using this preset.
- This deck: The limit is specific to this deck.
- Today only: Make a temporary change to this deck's limit.
 -->

## 新規カード
<!-- ## New Cards -->

この節の設定は、新規カードと[習得中カード](studying.md#learningrelearning-cards) にのみ影響します。習得学習を終えると、カードは[復習カード](studying.md#review-cards)となり、この節の設定は適用されなくなります。
<!-- The settings in this section only affect new cards and cards in initial
[learning](studying.md#learningrelearning-cards) mode. Once a card
has graduated (i.e. there are no more learning steps for this card), it becomes a
[review card](studying.md#review-cards), and the
settings in this section are no longer applicable. -->

### 習得ステップ
<!-- ### Learning Steps -->

カードを習得する（カードの内容を短期集中的に学習し記憶に定着させる）ための学習の繰り返しの回数と、その学習どうしの時間の間隔を設定します。前の学習からの時間の間隔を定めた一つ一つの習得学習を「`ステップ`」とよび、「1m」「10m」「1d」のように「前の学習からの時間の間隔」を意味する数字と単位で表現します。ステップどうしは、「1m 10m 1d」のように半角スペースをはさんで並べます。回答の際に`正解`を押すたびに、カードは次のステップに進みます。
<!-- Controls the number of learning repetitions, and the delay
between them. One or more delays, separated by spaces must be entered.
Each time you press `Good` during review, the card moves to the next step. -->

例えば、習得ステップが「**1m 10m 1d**」となっている場合、これは、「前の学習から1分(<u>**m**</u>inute)経過してから学習する→前の学習から10分(<u>**m**</u>inutes)経過してから学習する→前の学習から1日(<u>**d**</u>ay)経過してから学習する」という意味です。より具体的には次のような設定を意味しています：
<!-- For example, let's say that your learning steps are **1m 10m 1d**. -->

- 新規カードがあらかじめ最初のステップ（1m）にある状態で習得学習が開始します。このステップで`やり直し`を押すと、カードはこの最初のステップ（1m）をもう一度繰り返し、約1分後に再び表示されます。今後、先のステップに進んだ状態で`やり直し`を押した場合でも、カードは最初のステップ（1m）に戻り、約1分後に再び表示されます。
- この最初のステップ（1m）で`正解`を押すと、そのカードは次のステップ（10m）に進み、約10分後に再び表示されます。
- この2番目のステップ（10m）で`正解`を押すと、そのカードは次のステップ（1d）に進み、1日後、つまり翌日に表示されます。
- この最後のステップ（1d）で`正解`を押すと、そのカードは習得ステップ修了となり、中長期的に記憶を保持するためのカード（`復習カード`）になります。復習カードは、`習得ステップ修了から復習開始までの間隔（日）`で指定された間隔が経過してから、再び表示されます。
<!-- - When you press `Again`, the card goes back to first step, and will be shown
  again approximately 1 minute later.
- When you press `Good` on a new card, or a card answered `Again`, it will move
  to the next step, and be shown again in approximately 10 minutes.
- When you press `Good` on a card after the 10 minute step, it will be delayed
  until the next day.
- When you press `Good` on the card the next day, it will leave learning (i.e. it will graduate), and
  become a review card. It will be shown again after the delay configured by the
  _graduating interval_. -->

他に学習するカードがない場合、Ankiはデフォルトでは習得学習を最大20分前倒ししてカードを表示します。この、習得学習の前倒し（習得中カードの先取り）を許容する時間は[設定→学習](preferences.md#review)で調整できます。
<!-- If there’s nothing else to study, Anki will show cards up to 20 minutes
early by default. The amount of time to look ahead is configurable in
the [preferences](preferences.md). -->

ステップの動作についてより詳しく知りたい場合は、[学習](studying.md#learningrelearning-cards)の項目を参照してください。
<!-- Please see the [learning](studying.md#learningrelearning-cards) section for more info on how
steps work. -->

#### 日付境界線
<!-- #### Day Boundaries -->

Ankiは、「小さなステップ」（＝前のステップと日付が同じステップ）と[前のステップと日付が変わる](./preferences.md#review) ステップを異なる方法で扱います。

小さなステップの場合は、その時間間隔が経過すると、復習カードのような他の待機中カードよりも優先してその習得中カードを表示します。これは、指定された時間間隔とできるだけ同じ時間間隔でユーザーが習得中カードを学習できるようにするためです。

一方、その間隔によって日付が変わるステップの場合は、間隔を自動的に日数に変換します。

<!-- Anki treats small steps and steps that [cross a day boundary](./preferences.md#review) differently.
With small steps, the cards are shown as soon as the delay has passed,
in preference to other waiting cards like reviews. This is done so that
you can answer the card as closely to your requested delay as possible.
In contrast, if the interval crosses a day boundary, it is automatically
converted to days. -->

### 習得ステップ修了から復習開始までの間隔（日）
<!-- ### Graduating Interval -->

次のステップがないステップにある習得中カードで「正解」を選択してから、復習カードとしてそのカードが再び表示されるまでの間隔（日数）。前節の箇条書きの最後の項目に例があります。
<!-- The delay in days between answering "Good" on a learning card with no steps left,
and seeing the card again as a review card. Please see the example in the
previous section. -->

### 「簡単」と回答してから復習開始までの間隔（日）
<!-- ### Easy Interval -->

習得中カードで`簡単`を選択してから、そのカードが復習カードとして初めて表示されるまでの間隔（日数）。
<!-- The delay between answering `Easy` on a learning
card, and seeing it in review mode for the first time. -->

`簡単`ボタンを押すと、習得中カードはただちに復習カードに切り替わり、復習カード用に指定した学習間隔が適用されます。この間隔は通常、「習得ステップ修了から復習開始までの間隔（日）」より数日長くする（少なくとも同じ日数にする）ことが推奨されます。
<!-- The `Easy` button immediately turns a learning card into a review card,
and assigns it the delay you have configured. It should always be at least
as long as the _graduating interval_, and typically a few days longer. -->

### 配置順序
<!-- ### Insertion Order -->

Ankiが新規カードをデッキ内のランダムな位置（新規カード番号）に割り当てるか、追加した通りの順序で割り当てるかを決定します。 このオプションを変更すると、Ankiは選択中のオプションを使用しているデッキ内の新規カードを並べ直し、新規カードの位置（新規カード番号）を自動的に更新します。学習する際は、デフォルトでは、新規カード番号の数字が小さいカードから表示されていきます。
<!-- Controls whether Anki should add new cards into the deck randomly, or in order.
When you change this option, Anki will re-sort the decks using the current
Option Group. Cards with a lower due number will be shown first when studying, by
default. Changing this option will automatically update the existing position of
new cards. -->

「ランダム」を選択している場合の注意点：新規カードをたくさん学習してから、さらに新規カードを追加すると、新たに追加したカードの方が、その前からデッキ内にあったカードよりも統計的に表示されやすくなります。例えば、ランダムに並んだ100枚のカードがあり、最初の50枚をすでに学習した場合、新たに追加するカードの位置（＝新規カード番号）は1から100の間のままですが、最初の50枚をすでに学習しているため、新たに追加するカードの方が先に表示されやすくなります。この偏りを補正したい場合は、いったん「追加順」を選択してから再度「ランダム」を選択すれば、カード全体をランダムに並び変えることができます。
<!-- ※「例えば、～」以降の内容が、V3でもV2でも、試してみると予想する結果にならない。要再検証。 -->
<!-- One caveat with random order mode: if you review many of your new cards, and then
add more new cards, the newly added material is statistically more likely to
appear than the new cards that were already in the deck. For example, if you have 100 cards
in random order, then review the first 50, newly added cards are still given
position 1-100, but as you have already reviewed the first 50, the newly added
cards are more likely to appear earlier. To correct this, you can change the
order to Ordered mode and back again to force a re-sort. -->

「ランダム」を選択すると、Ankiは各ノートをランダムを並べ、同じノートから作られたカードどうし（兄弟関係のカードどうし）を近くに保ちます。兄弟関係カードどうしは、カードタイプの表示順で表示されるため、まとめて導入されます。そのようにしないと、一部のノートではすべてのカードが導入される一方、他のノートではそうならない、という状態になってしまう可能性があるからです。 詳細については、下記の「今日は非表示」関連の項および「表示順序」の項を参照してください。
<!-- ※"bury related"は、非表示関連の項目という意味？それとも実際にそのタイトルの項目がある？ -->
<!-- When you select random order, Anki will randomize your notes, keeping
the cards of a given note close together. The cards of a given note are
shown in the order, in which their card types appear, so that siblings are
introduced consistently — otherwise you could end up in a state where
some notes had all their cards introduced and other notes had only one
or two. Please see the "bury related" and "display order" sections below
for more info. -->

## 復習でのつまずき
<!-- ## Lapses -->

復習の際に`つまずき`があった場合、つまり、復習カードの質問に対する正しい答えを思い出せなかった場合、そのカードを再び短期集中的に学習する必要があります。この学習のことを`再習得`学習といいます。

既定の設定による動作では、つまずいた復習カードで「もう一度」ボタンを選択すると、次の復習までの間隔が1日（つまり、翌日が期日）となるとともに、そのカードは再習得学習のキューに送られ、10分後に再び表示されます。この動作は下記の各オプションでカスタマイズすることができます。

<!-- 
When you forget a review card, it is said to have 'lapsed', and the card must be
relearnt. The default behaviour for lapsed reviews is to reset the interval to
1 (i.e. make it due tomorrow), and put it in the learning queue for a refresher
in 10 minutes. This behaviour can be customized with the options listed below. -->

### 再習得ステップ
<!-- ### Relearning Steps -->

復習でつまずいたカードを対象としているという点以外は、前述の「学習ステップ」と同様です。つまずいた復習カードで「`もう一度`」と回答すると、そのカードは再習得学習のフェーズに入り、`再習得中カード`となります。再習得中カードを復習カードに戻すには、すべてのステップで`正解`するか、いずれかのステップで`簡単`と回答する必要があります。
<!-- 
The same as 'learning steps', but for forgotten reviews. When you fail a card
(press `Again`), the card enters the relearning phase, and before it becomes a
review card again, you will have to pass all the relearning steps — or, alternatively, press
`Easy` on the card. -->

ステップの入力欄を空欄にした場合は、そのカードは再習得学習をスキップし、復習再開後用の新しい間隔が設定された復習カードとなります。
<!-- 
If you leave the steps blank, the card will skip relearning, and will be assigned
a new review delay. -->

### 復習再開時の復習間隔の下限（日）
<!-- ### Minimum Interval -->

再習得学習の最終ステップを「正解」し終わってから最初の復習までに少なくとも何日待機するかを指定します。 デフォルトの設定では1日となっています。これは、最終ステップを「正解」し終わったカードが復習カードとして翌日表示されることを意味します。　
<!-- 
Specifies a minimum number of days a card should wait after it finishes relearning.
The default is one day, meaning once relearning is finished, it will be shown again
the next day. -->

### 苦戦（つまずき多発）の判定についての項目
<!-- ### Leeches -->

復習でのつまずきが多発しているカードをどう扱うかを設定します。詳細は[苦戦（つまずき多発）](leeches.md)の項を参照してください。
<!-- 
Control the way Anki handles leeches. Please see the [leeches](leeches.md)
section for more information. -->

## 表示順序
<!-- ## Display Order -->

この節の各オプションの設定は、学習を開始するときに選択したデッキから取得されます。つまり、選択したデッキのサブデッキのカードを表示する際にも、そのサブデッキのオプションではなく、選択したデッキのオプションでの設定が適用されます。
<!-- The options in this section are taken from the deck you select to study, not
the deck of the currently displayed card. -->

この節の各オプションは、 [V3スケジューラー](https://faqs.ankiweb.net/the-2021-scheduler.html)でのみ使用できます。
<!-- This section is only available when you have [the v3 scheduler](https://faqs.ankiweb.net/the-2021-scheduler.html) enabled. -->

表示順序に関する詳細については、[学習セクション](studying.md#display-order)を参照してください。
<!-- Some further information about display order is available in the [studying section](studying.md#display-order). -->

### 新規カードを集める順序
<!-- ### New Card Gather Order -->

Anki が、導入する新規カードを各サブデッキから集める際に、どのような順序で集めるかを設定します。オプションは次のとおりです。
<!-- Controls how Anki gathers cards from each subdeck. The options are: -->

- デッキの並び順（上から）：選択したデッキとその中のサブデッキのうち、デッキリストで上に並んでいるデッキからカードを集めていきます。つまり、最初は選択したデッキ自体のカードを集めて、次に、一番上のサブデッキのカードを集めて、という順序です。各デッキ内のカードを集める順序は、昇順（次項参照）となります。集めている途中で一日の上限枚数に達した場合は、そのデッキより下に並んでいるデッキのカードは集めません。この順序にすると、大規模なコレクションでも比較的早くカードを集めることができます。なお、優先したいサブデッキがある場合は、下記の方法によって、そのサブデッキを上の方に並べ変えるとよいでしょう。

  同じ階層のデッキどうしは常に数字順・アルファベット順など文字コード順に並んでいるため、例えばデッキ名の先頭に「001」「002」などと数字を付けることによって、デッキどうしの並び順を調整することができます。ちなみに、`_`（アンダーバー）記号で始まる名前のデッキはアルファベット文字で始まるデッキよりも上に並べられ、`~`（チルダ）記号で始まる名前のデッキはアルファベット文字で始まる名前のデッキよりも下に並べられます。

  位置の順序は、最初は前述の「導入する順序」オプションの設定に依存しますが、さまざまな方法によって手動でカードを[並び変える](https://docs.ankiweb.net/browsing.html#cards)ことができます。

<!-- - Deck: gathers cards from each deck in order, starting from the top. Cards from
  each deck are gathered in ascending position. If the daily limit of the selected
  deck is reached, gathering may stop before all decks have been checked. This
  order is fastest in large collections, and allows you to prioritize subdecks that
  are closer to the top.

   Decks / subdecks are always ordered alphabetically, so you can give them a numeric prefix like
  001 to control the order they are shown. You can also use `_` and `~` as a
  prefix to place items at the top or bottom. 
  
  Although position order depends initially on the 'Insertion Order' setting
  above, you can manually
  [reposition](https://docs.ankiweb.net/browsing.html#cards) cards in different
  ways. -->

- 位置（新規カード番号）の昇順: 追加時に各カードに割り当てられた位置（＝新規カード番号）の数字が小さい順にカードを集めます。通常は、各カード中で最初に追加したカード（最古のカード）から集められていきます。
<!-- - Ascending position: gathers cards by ascending position (due #), which is typically the oldest-added first. -->

- 位置（新規カード番号）の降順: 追加時に各カードに割り当てられた位置（＝新規カード番号）の数字が大きい順にカードを集めます。通常は、各カード中で最後に追加したカード（最新のカード）から集められていきます。
<!-- - Descending position: gathers cards by descending position (due #), which is typically the latest-added first. -->

- ランダム（ノート単位）: ランダムに選んだノートからカードを集めます。「兄弟関係のカードの非表示」オプションがオフになっている場合は、同じノートから作成されたカード（例えば、《表面→裏面》カードと《裏面→表面》カード）がすべて同じセッションで表示されます。
<!-- - Random notes: gathers cards of randomly selected notes. When sibling burying is disabled, this allows all cards of a note to be seen in a session (eg. both a front->back and back->front card) -->

- ランダム（カード単位）: 完全にランダムにカードを集めます。
<!-- - Random cards: gathers cards completely randomly. -->

### 集めた新規カードを並べる順序
<!-- ### New Card Sort Order -->

**導入する新規カードを集めた（＝選んだ）後**、それらのカードをどのような順序で表示するかを決定します。
<!-- Controls how new cards are sorted **after they have been gathered**. The options are: -->

- カードタイプ順→集めたときの順序: カードタイプの数字順にグループ分けし、そのグループごとにカードを表示していきます。同じカードタイプどうしのカードは、集めたときの順序で表示されます。「兄弟関係のカードの非表示」が無効になっている場合、例えば、カードタイプが「カード 1」の《表面→裏面》カードをすべて表示してから、カードタイプ「カード 2」の《裏面→表面》カードを表示していきます。兄弟関係のカード（＝同じノートから作られたカード）どうしを同じセッションで表示したいが、近づけすぎないようにもしたい、という場合に適した設定です。
<!-- - Card type: Displays cards in order of card type number. If you have sibling burying disabled, this will ensure all front→back cards are seen before any back→front cards. This is useful to have all cards of the same note shown in the same session, but not too close to one another. -->

- 集めたときの順序: カードを集めたときのままの順序で表示します。「兄弟関係のカードの非表示」が無効になっている場合、通常、兄弟関係のカードどうしは連続して表示されます。
<!-- - Order gathered: Shows cards exactly as they were gathered. If sibling burying is disabled, this will typically result in all cards of a note being seen one after the other. -->

- カードタイプ順→ランダム: 「カードタイプ順」と同じくカードタイプの数字順にグループ分けをしますが、各カードタイプのグループ内のカードをランダムな並びで表示します。カードを集めるときに「位置（新規カード番号）の昇順」で古いカードを優先的に集めた上で、この設定にすることによって、それらのカードをランダムな並びで表示し、兄弟関係のカードどうしを近づけすぎずに表示することができます。
<!-- - Card type, then random: Like Card type, but shuffles the cards of each card type number. If you use Ascending position to gather the oldest cards, you could use this setting to see those cards in a random order, but still ensure cards of the same note do not end up too close to one another. -->

- ランダム（ノート単位）→カードタイプ順: ノートをランダムに並べ、ノートがカードを複数持つ場合（つまり、兄弟関係のカードがある場合）はそれらのカードをカードタイプ順に表示します。
<!-- - Random note, then card type: Picks notes at random, then shows all of their siblings in order. -->

- ランダム（カード単位）: 集めたカードを完全にランダムな並びで表示します。
<!-- - Random: Fully shuffles the gathered cards. -->

### 新規カード表示のタイミング
<!-- ### New/Review Priority -->

新規カードを、復習カードと交ぜて表示していくか、復習カードを表示し始める前に表示していくか、復習カードを表示し終わった後に表示していくか、を設定します。
<!-- Whether new cards should be mixed in with reviews, or shown before or after them. -->

### 日をまたいだステップの習得中（再習得中）カード表示のタイミング
<!-- ### Interday Learning/Review Priority -->

前回の学習との間隔が日をまたいでいるステップの習得中カード（または習得中カード、以下略）を、復習カードと交ぜて表示していくか、復習カードを表示し始める前に表示していくか、復習カードを表示し終わった後に表示していくか、を設定します。習得中カードは復習カードよりも回答するのが難しい傾向があるため、習得中カードを復習カードの後で表示したい（簡単な方から先に取り組みたい）場合や、先に表示したい（難しい方に時間とエネルギーを優先的に充てたい）場合など、好みに応じてここでの設定を選択してください。
<!-- Whether learning cards with a 1+ day delay should be mixed in with reviews, or
shown before or after them. Because learning cards tend to be harder than
reviews, some users prefer to see them at the end (getting the easy stuff done
first), or at the start (allowing more time to review forgotten ones). -->

### 復習カードを並べる順序
<!-- ### Review Sort Order -->

復習カードを、学習中にどのような順序で表示するかを設定します。オプションは次の通りです：
<!-- Controls how review cards are sorted while reviewing. The options are: -->

- 期日超過日数が大きい順→同日数どうしはランダム: デフォルトの設定です。待機期間が長いカードから優先して表示します。延滞（予定の学習日時に達していながらカードを学習していない状態）がない場合や、あったとしても少ない場合に推奨される設定です。長い間学習をしていなかったり、学習ペースが遅れてバックログがたまったりしている場合は、一時的に他の設定（他の選択項目）に変更することを検討したほうがよいかもしれません。
<!-- - Due date, then random: The default option prioritizes cards that have been waiting
  longer, and it's the recomended option when you are up to date, or when you only have a small
  backlog. If you have taken an extended break or have fallen behind in your reviews,
  you may want to consider changing the sort order temporarily. -->
- 期日超過日数が大きい順→同日数どうしはデッキの並び順: この設定でも、待機期間が長いカードから優先して表示します。同日数どうしのカードは、サブデッキの並んでいる順に、サブデッキごとにカードを表示していきます。
<!-- - Due date, then deck. This also prioritizes cards that have been waiting
  longer, and then will show reviews for each subdeck in turn. -->
<!-- ※※※※※※※※※※※※※※※※※※※※※※※※※
typo
Due date, then deck. This also prioritizes~
↓
Due date, then deck: This also prioritizes~
※※※※※※※※※※※※※※※※※※※※※※※※※※※※-->
- デッキの並び順→デッキ内では期日超過日数が大きい順: この設定では、サブデッキの並んでいる順に、サブデッキごとに復習カードを表示していきます。学習内容が一貫して同じ順序で表示され、そのパターンに基づいて答えを推測しやすくなってしまい、記憶の強化に結びつかない可能性があるため、この並び順は一般的には推奨されません。
<!-- - Deck, then due date: This option will ensure reviews are shown for each
  subdeck in turn. This is generally not recommended, as having material appear
  consistently in the same order makes it easier to guess the answer based on context,
  and may lead to weaker memories. -->
- 復習間隔が短い順: 前回の回答時に、次の復習までの間隔（日数）が設定されています。その間隔が短いカード（比較的、未習熟なカード）から表示していきます。
<!-- - Ascending intervals: This will ensure cards with shorter intervals are shown first. -->
- 復習間隔が長い順: 前回の回答時に、次の復習までの間隔（日数）が設定されています。その間隔が長いカード（比較的、習熟しているカード）から表示していきます。
<!-- - Descending intervals: This will ensure cards with larger intervals are shown first. -->
- 易しさが低い順: 最も難しいと評価されているカードを最初に表示します。
<!-- - Ascending ease: This will show most difficult cards first. -->
- 易しさが高い順: 最も易しいと評価されているカードを最初に表示します。易しめのカードから取り組んでいくことができます。
<!-- - Descending ease: This will allow you to work through the easier material first. -->
- 期日超過率が大きい順: [本来の期日までの間隔に対する延滞日数の比率が最も大きい](./filtered-decks.html#order)カードを最初に表示します。
<!-- - Relative overdueness: Display those cards first, that are [most overdue in relation
  to their current interval](./filtered-decks.html#order). -->

## タイマー
<!-- ## Timer -->

Ankiは、日々の学習時間を振り返ることができるように、各カードに回答するのにかかった時間を記録しています。この時間は、学習スケジュールには影響しません。
<!-- Anki monitors how long it takes you to answer each card, so that it
can show you how long was spent studying each day. The time taken does
not influence scheduling. -->

オプションは次の通りです：
<!-- The options are: -->

- 最長回答秒数: デフォルトでは、60秒となっています。この場合、あるカードの回答秒数（問題が表示されてから回答ボタンを押すまでの秒数）がもっと長くても、Ankiは、あなたが画面から離れたり、他のことに気をとられたりしているのだろうと判断し、学習時間の統計が不正確にならないよう、そのカードの回答秒数を60秒と記録します。もし、回答秒数が60秒より長いことがよくある場合は、この設定秒数をもっと大きくするか、より理想的には、カードの内容をもっとシンプルにするとよいかもしれません。
<!-- - Maximum answer seconds: The default limit is 60 seconds. If you take
  longer than that, Anki assumes you have walked away from your computer
  or have been distracted, and limits the recorded time to 60 seconds, so
  that you don’t end up with inaccurate statistics. If you consistently
  take longer than 60 seconds to answer a card (from when question is shown
  until you press an answer button), you may want to either consider raising
  this limit, or ideally, making your cards simpler. -->
- 回答タイマーを表示する: カード学習画面に、表示中のカードの回答秒数をカウントするタイマーを表示します。
<!-- - Show answer timer: In the review screen, show a timer that counts the number
  of seconds you're taking to review each card. -->

## 兄弟関係のカードの非表示
<!-- ## Burying -->

### 兄弟関係の新規カードを同じ日に表示しない
<!-- ### Bury new siblings -->

学習したカードと兄弟関係のカード（※）があり、そのカードが新規カードである場合、そのカードを表示する順番がきたとしても同じ日には表示を行わず、翌日から表示を再開します。

※ 兄弟関係のカード：同じノートから作られたカード。例えば、裏表反転カード。

Ankiは学習画面に表示するカードを準備する際、準備リストにまず「前回のステップと今回のステップとの間隔が日をまたいでいない（＝当日中に最優先で再び学習すべき）習得中/再習得中カード」を並べ、次に「間隔が日をまたいでいる習得中/再習得中カード」、その次に復習カード、最後に新規カードを並べます。この並び方をもとに、どのカードを表示し、どのカードを当日は非表示にするかが次のように決まります：

- すべての非表示オプションが有効になっている場合、リスト内の兄弟どうしのうち、最も先に並んでいるカードのみが表示されます。例えば、リスト内のある復習カードとある新規カードが兄弟どうしの場合、復習カードの方が先に並んでいるので、復習カードが表示され、新規カードは当日は非表示となります。

- リスト内の兄弟どうしのうちで後ろに並んでいるカードの非表示を解除したとしても、先に並んでいる別の種類のカードが代わりに非表示となることにはなりません。例えばリスト内の、ある復習カードとある新規カードが兄弟どうしの場合、たとえ新規カードの非表示を解除して学習したとしても、代わりに復習カードが非表示になってしまうことにはなりません。つまりこの場合は、兄弟どうしである復習カードと新規カードの両方が同じ日に表示されることになります。

<!-- When Anki gathers cards, it first gathers intraday learning cards, then interday learning cards, then reviews, and finally new cards. This affects how burying works:

- If you have all burying options enabled, the sibling that comes earliest in that list will be shown. For example, a review card will be shown in preference to a new card.
- Siblings later in the list can not bury earlier card types. For example, if you disable burying of new cards, and study a new card, it will not bury any interday learning or review cards, and you may see both a review sibling and new sibling in the same session. -->

### 兄弟関係の復習カードを同じ日に表示しない
<!-- ### Bury review siblings -->

学習したカードと兄弟関係のカード（※）があり、そのカードが`復習`カードである場合、そのカードを表示する期日に達していても同じ日には表示を行わず、翌日から表示を再開します。

※ 兄弟関係のカード：同じノートから作られたカード。例えば、裏表反転カード。

<!-- 
Whether other review cards of the same note will be delayed until the next day. -->

Ankiは学習画面に表示するカードを準備する際、準備リストにまず「前回のステップと現在のステップとの間隔が日をまたいでいない（＝当日中に最優先で再び学習すべき）習得中/再習得中カード」を並べ、次に「間隔が日をまたいでいる習得中/再習得中カード」、その次に復習カード、最後に新規カードを並べます。この並び方をもとに、どのカードを表示し、どのカードを当日は非表示にするかが次のように決まります：
<!-- 
When Anki gathers cards, it first gathers intraday learning cards, then interday learning cards, then reviews, and finally new cards. This affects how burying works: -->

- すべての非表示オプションが有効になっている場合、リスト内の兄弟どうしのうち、最も先に並んでいるカードのみが表示されます。例えば、リスト内のある復習カードとある新規カードが兄弟どうしの場合、復習カードの方が先に並んでいるので、復習カードが表示され、新規カードは当日は非表示となります。
<!--
 - If you have all burying options enabled, the sibling that comes earliest in that list will be shown. For example, a review card will be shown in preference to a new card. -->

- リスト内の兄弟どうしのうちで後ろに並んでいるカードの非表示を解除したとしても、先に並んでいる別の種類のカードが代わりに非表示になるということはありません。例えばリスト内の、ある復習カードとある新規カードが兄弟どうしの場合、たとえ新規カードの非表示を解除して学習したとしても、代わりに復習カードが非表示になってしまうことはありません。つまりこの場合は、兄弟どうしである復習カードと新規カードの両方が同じ日に表示されることになります。
<!--
 - Siblings later in the list can not bury earlier card types. For example, if you disable burying of new cards, and study a new card, it will not bury any interday learning or review cards, and you may see both a review sibling and new sibling in the same session. -->

### 兄弟関係の習得中カードで、ステップの間隔が日をまたいでいる場合は、同じ日に表示しない
<!--  ### Bury interday learning siblings -->

学習したカードと兄弟関係のカードがあり、そのカードが`習得中`カードである場合、そのカードの現在のステップの間隔が日をまたいでいる場合に限り、同じ日には表示を行わず、翌日から表示を再開します。
<!-- 
Whether other learning cards of the same note with intervals > 1 day will be delayed until the next day. -->

Ankiは学習画面に表示するカードを準備する際、準備リストにまず「前回のステップと現在のステップとの間隔が日をまたいでいない（＝当日中に最優先で再び学習すべき）習得中/再習得中カード」を並べ、次に「間隔が日をまたいでいる習得中/再習得中カード」、その次に復習カード、最後に新規カードを並べます。この並び方をもとに、どのカードを表示し、どのカードを当日は非表示にするかが次のように決まります：
<!-- 
When Anki gathers cards, it first gathers intraday learning cards, then interday learning cards, then reviews, and finally new cards. This affects how burying works: -->

- すべての非表示オプションが有効になっている場合、リスト内の兄弟どうしのうち、最も先に並んでいるカードのみが表示されます。例えば、リスト内のある復習カードとある新規カードが兄弟どうしの場合、復習カードの方が先に並んでいるので、復習カードが表示され、新規カードは当日は非表示となります。
<!--
 - If you have all burying options enabled, the sibling that comes earliest in that list will be shown. For example, a review card will be shown in preference to a new card. -->

- リスト内の兄弟どうしのうちで後ろに並んでいるカードの非表示を解除したとしても、先に並んでいる別の種類のカードが代わりに非表示になるということはありません。例えばリスト内の、ある復習カードとある新規カードが兄弟どうしの場合、たとえ新規カードの非表示を解除して学習したとしても、代わりに復習カードが非表示になってしまうことはありません。つまりこの場合は、兄弟どうしである復習カードと新規カードの両方が同じ日に表示されることになります。
<!--
 - Siblings later in the list can not bury earlier card types. For example, if you disable burying of new cards, and study a new card, it will not bury any interday learning or review cards, and you may see both a review sibling and new sibling in the same session. -->

兄弟関係のカードの非表示についての詳細は、マニュアルの[この項](./studying.md#siblings-and-burying)をご覧ください。 
<!-- 
For more info about burying cards, please see [this section](./studying.md#siblings-and-burying) of the manual. -->

## オーディオ
<!-- ## Audio -->

デフォルトでは、Ankiはカードの表と裏で自動的に音声ファイルを再生します。「_オーディオを自動再生しない_」をオンにすると、Ankiは「_オーディオを再生_」のアクション（ショートカットキーは `r` または `F5`）を行うまで音声を再生しません。
<!-- 
By default, Anki automatically plays audio on the front and back of
cards. If you check _Don't play audio automatically_, Anki will not play
audio until you press the replay audio key, `r` or `F5`. -->

「_オーディオ再生の際、質問側のオーディオも必ず含める_」は、カードの解答側（裏面）も表示しているときに「オーディオを再生」アクションを選択した場合に、質問側（表面）のオーディオも再生するのかどうかを設定します。このオプションは、解答を表示したときのオーディオの自動再生について設定するわけではないことに注意してください。解答を表示した後のオーディオの自動再生については、[この項](templates/fields.md#special-fields)をご覧ください。
<!--  ※。。。Anki 2.1.66ではこの項目は Skip question when replaying answer になっている。マニュアルの要改訂箇所か。。。-->
<!-- 
_Always include question side when replaying audio_ controls whether audio from
the question side should be played when replaying the audio while an answer is
shown. Please note that it does not control what happens when you show the
answer; for that please see [this section](templates/fields.md#special-fields). -->

## 詳細
<!-- ## Advanced -->

### 復習間隔の上限（日）
<!-- ### Maximum Interval -->

Ankiがカードの再表示を待機する時間の上限を設定できます。デフォルトでは100年（36500日）です。記憶の定着率を下げてでも学習時間を減らしたいという場合は、この値を小さくすとよいでしょう。
<!-- Allows you to place an upper limit on the time Anki
will wait to reshow a card. The default is 100 years; you can decrease
this to a smaller number if you’re willing to trade extra study time for
higher retention. -->

### 復習開始時の「易しさ」〔復習間隔の前回比〕（倍）
<!-- ### Starting Ease -->

「易しさ」の初期値を設定します。この値は、カードが習得ステップを修了する際に、そのカードに設定されます。デフォルトの値2.50の場合、復習カードに`正解`と回答すると、そのカードの次の復習までの間隔は、回答した復習までの間隔の約2.5倍になります（例えば、最初の復習までの間隔が10日だった場合、次の復習までの間隔はおよそ25日になります）。以降の復習でそのカードにどう回答するかによって、「易しさ」はこの初期値から増減していきます。
<!-- Controls the easiness that cards start out with. It is
set when a card graduates from learning for the first time. It defaults
to 2.50, 
meaning that once you have finished learning a card, answering
`Good` on subsequent reviews will increase the delay by approximately
2.5x 
(e.g. if the last delay was 10 days, the next delay would be around 25
days). 
Based upon how you rate the card in subsequent reviews, the
easiness may increase or decrease from its starting value. -->

### 復習で「簡単」と回答した場合のボーナス（倍）
<!-- ### Easy Bonus -->

復習カードに「簡単」と回答した際、そのカードの復習間隔に追加して適用される倍率。デフォルトの値1.30では、「簡単」と回答した場合、次の復習までの間隔は、「正解」と回答した場合の約1.3倍の間隔になります（例えば、「正解」での間隔が10日なら、「簡単」での間隔はおよそ13日になります。
<!-- An extra multiplier applied to the interval when a review card is answered
`Easy`. With the default value of 1.30, `Easy` will give an interval that is
1.3 times the `Good` interval (e.g. if the Good interval was 10 days, the Easy
interval would be around 13 days). -->

### 復習間隔の一括調整（倍）
<!-- ### Interval Modifier -->

すべての復習に適用される追加乗数。デフォルトの1.00では何もしません。例えばこれを0.80に設定すると、復習間隔は通常の80%となります（10日の復習間隔は8日になります）。このように、この倍率を使うことで、復習カードを提示する頻度を高くしたり、低くしたりすることができ、より記憶を定着させるために学習時間を増やすか、逆に、記憶定着の強さや確実さを減らしてでも学習負担を減らすかを調整することができます。
<!-- 
An extra multiplier that is applied to all reviews. At its default of 1.00 it
does nothing. If you set it to 0.80, though, for example, intervals will be generated at
80% of their normal size (so a 10 day interval would become 8 days). You can
thus use the multiplier to make Anki present cards more or less frequently than
it would otherwise, trading study time for retention or vice versa. -->

適度な難しさの教材の場合、平均的なユーザーは、復習のために提示された習熟期のカードの約90%の正答を思い出せる（＝「もう一度」以外を選択できる）と想定されています。自分の正答率（記憶保持率）は、「統計」画面の「回答ボタン」のグラフで確認できます。習熟期のカードの正答率は、グラフの右端のグループに表示されます。ただし、学習を開始してまだ日が浅い場合は、まだ習熟期のカードがない場合があります。習得中カードと未習熟カードの成績はかなり異なる可能性があるため、習熟期のカードの量がそれなりの量になるまでは、自分の記憶保持率について結論を出すのは控えるのが賢明でしょう。
<!-- 
For moderately difficult material, the average user should find they
remember approximately 90% of mature cards that come up for review. You
can find out your own performance by opening the graphs/statistics for a
deck and looking at the Answer Buttons graph - mature retention is the
correct% on the right side of the graph. If you haven’t been studying
long, you may not have any mature cards yet. As performance with new
cards and younger cards can vary considerably, it’s a good idea to wait
until you have a reasonable amount of mature reviews before you start
drawing conclusions about your retention rate. -->

SuperMemoのウェブサイトでは、目標とする記憶保持率のために適切なこのオプションの倍率を計算してみることを提案しています。その計算式を要約すると次の通りです：
<!-- 
On the SuperMemo website, they suggest that you can find an appropriate
multiplier for a desired retention rate. Their formula boils down to: -->


    log(目標とする記憶保持率[%]) / log(実際の記憶保持率[%])
    
<!--  
    log(desired retention%) / log(current retention%) -->

例えば、実際の記憶保持率が85%で、これを90%まで上げたい場合、このオプションの倍率は次の通りとなります（小数第3位四捨五入）：
<!-- Imagine we have a current retention rate of 85% and we want to increase
it to 90%. We’d calculate the modifier as: -->

    log(90%) / log(85%) = 0.65

これは、[Googleの電卓機能で計算](https://www.google.com/search?q=log(90%25)+%2F+log(85%25))することができます。
<!-- You can use Google to [calculate it](https://www.google.com/search?q=log(90%25)+%2F+log(85%25)) for you. -->

この計算結果0.65をこのオプションの倍率として設定すると、記憶保持率（正答率）が目標とする値に近づいていくことが実感できるでしょう。
<!-- If you plug the resulting 65% into the interval modifier, you should
find over time that your retention moves closer to your desired
retention. -->

注意すべき重要な点は、学習に費やす時間と記憶保持率のトレードオフは、単純な直線的関係ではないということです。先ほどの例では、記憶保持率を5%ポイント上げる（85%→90%）ためには、復習間隔の倍率を35%ポイント減らし（1.0 - 0.35 = 0.65）、学習負担を54%ポイント増（100÷65=1.54）すなわち1.54倍の頻度での学習が必要になると見込まれます。学習している内容が非常に重要である場合は、そうした努力の上乗せをする価値があるかもしれませんが、もちろん、それはあなた自身が判断する必要があります。忘れてしまっていることの多さが気になるだけの場合は、初期の習得学習の段階により多くの時間を投資したり、学習内容を深く印象づけるような記憶術を活用したりするほうが、少ない労力でより多くの成果が得られるでしょう。
<!-- ※。。。原文では、「35%より頻繁に学習する必要がある」という意味になるが、誤りか。。。例えばオプション値を50%ポイント減じて0.5にすると、頻度は50％ポイント増ではなく2倍になるはず。。。ちなみにこのオプションの範囲は0.5～2.0となっているようだ。。。 -->
<!-- One important thing to note however is that the trade-off between time
spent studying and retention is not linear: we can see here that to
increase our retention by 5 percentage points, we would have to study 35%
more frequently. If the material you are learning is very important then
it may be worth the extra effort – that is, of course, something you will need to
decide for yourself. If you are simply worried that you are forgetting too
much, then you may find investing more time at the initial learning stage
and/or using mnemonics will give you more gain for less effort. -->

最後に注意すべき点は、Ankiは必ず復習間隔を、一つ前の復習間隔よりも少なくとも1日以上長く設定するということです。これは、同じ学習間隔に永遠に留まり続けてしまうことがないようにするためです。もし、あるカードを数日間毎日1回ずつ学習したい場合は、このオプションの値を調整するのではなく、習得ステップの回数を増やすとよいでしょう。
<!-- One final thing to note is that Anki forces a new interval to be at
least 1 day longer than it was previously, so that you do not get stuck
reviewing with the same interval forever. If your goal is to repeat a
card once a day for multiple days, you can do that by setting more
learning mode steps, instead of by adjusting this modifier. -->

### 復習で「難しい」と回答した場合の間隔〔前回比〕（倍）
<!-- ### Hard Interval -->

復習カードに「難しい」と回答した場合の復習間隔を決めるために使用する乗数。次の復習間隔は、その前の復習間隔にこの値を掛けた日数となります。例：デフォルトの値1.20で、復習間隔10日のカードに「難しい」と回答した場合、次の復習間隔は12日となります（10×1.20＝12）。
<!-- The multiplier used when you use the `Hard` button. The percentage is relative
to the previous interval: e.g. with a default of 1.20, a card with a 10-day interval
will be given 12 days. -->

### 復習再開後の復習間隔〔前回復習比〕（倍）
<!-- ### New Interval -->

復習カードに「もう一度」と回答した場合の、復習再開後の復習間隔を決めるために使用する乗数。デフォルトの0.00は、再習得ステップ修了後の最初の復習までの間隔を、それまで延ばしてきた間隔をリセットしてゼロにすることを意味します（ただし実際には、[復習再開時の復習間隔の下限（日）](#minimum-interval) のデフォルト値および最小値が1なので、復習間隔はデフォルトでは1日になり、他の場合も0日にはなりません）。
<!-- The multiplier used when you use the `Again` button on a review card. The
default 0.00 means that a review card's delay is reset to zero when you forget it
(which then becomes 1 day after the [minimum interval](#minimum-interval) is
applied). -->

このオプションの値を変更すると、つまずいたカードの復習間隔を（一律に下限日数にリセットするのではなく、）それまでの復習間隔の日数に応じて新しい復習間隔を設定することができます。例えば、復習間隔100日のカードでつまずき、このオプションの値が0.20である場合、復習再開後の復習間隔は20日になります（100×0.20＝20）。
<!-- If changed from the default, it is possible for forgotten cards to preserve part
of their previous delay. For example, if a card had a 100 day interval, and you set
the _New Interval_ to 0.20, the new interval would be 20 days. -->

このように以前の復習間隔を復習再開後に反映することは理にかなっているように見えるかもしれませんが、SuperMemoは、以前の復習間隔を反映することが実際には[逆効果になる](https://supermemo.guru/wiki/Post-lapse_stability)可能性があると指摘しています。このため、デフォルトの設定のままにしておくことをお勧めします。

<!-- While preserving part of the interval may seem to make sense, SuperMemo has observed
that preserving part of the delay can actually [be counter-productive](https://supermemo.guru/wiki/Post-lapse_stability). For this reason, we recommend you leave it on the default setting. -->

## カスタムスケジューリング
<!-- ## Custom Scheduling -->

[こちらのページ](https://faqs.ankiweb.net/the-2021-scheduler.html#add-ons-and-custom-scheduling)を参照してください。
<!-- Please see [this page](https://faqs.ankiweb.net/the-2021-scheduler.html#add-ons-and-custom-scheduling). -->
