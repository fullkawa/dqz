# +-÷Xan

『Xan』は「四則演算」を基本システムとするカードゲームです。  
四則演算とは、足し算・引き算・掛け算・割り算のことです。  
プレイヤー全員で協力して計算式を完成させ、シナリオクリアを目指しましょう！  

## 目次

1. カードの作り方
2. [カードおよび用語の説明](https://github.com/fullkawa/dqz/edit/xan/README.md#1-%E3%82%AB%E3%83%BC%E3%83%89%E3%81%8A%E3%82%88%E3%81%B3%E7%94%A8%E8%AA%9E%E3%81%AE%E8%AA%AC%E6%98%8E)  
3. [遊び方](https://github.com/fullkawa/dqz/edit/xan/README.md#2-%E9%81%8A%E3%81%B3%E6%96%B9)  
3.1. 準備  
3.2. ゲームの流れ  
3.3. ゲーム終了  
3.4. 選択ルール  
3.5. 2人プレイ  
3.6. ソロプレイ  
4. [ライセンス](https://github.com/fullkawa/dqz/edit/xan/README.md#3-%E3%83%A9%E3%82%A4%E3%82%BB%E3%83%B3%E3%82%B9)  

## 1. カードの作り方

### 必要なモノ

* プリンタ + A4用紙
* カードスリーブ(MTGサイズ=幅63mm, 高さ89mm)  
※ 100円ショップに売っているものとかで十分です！
* 不要なTCGカード

### 作成手順

1. [ファイル一式](https://github.com/fullkawa/dqz/archive/xan.zip)をダウンロード＆解凍する。
2. 基本セットカード(card.html), シナリオ#1カード(scenario/s1_card.html)をダブルクリックしてブラウザ(Chrome推奨)に表示する。
3. ブラウザの印刷コマンドからプリンタで印刷する。
4. ハサミで切り離す。
5. 切り離したカードをスリーブに入れる。このとき一緒にTCGカードを入れて補強すると良い。

## 2. カードおよび用語の説明

### 【フィールドカード】  

- 【キャラクター】が利用できる土地の力を表します。
- 1～5の数字が各３枚ずつあります。

### 【クラスカード】

- プレイヤーが担当する【キャラクター】を表します。
- 「＋」「－」「×」「÷」の記号が1枚ずつあります。

### 【スキルカード】

- キャラクターが使えるスキルを表します。
- 「( )」「※」「＋－×÷」「∴」「⇒」「x2」の記号が1枚ずつあります。
- 使用できるクラスが限定されているカードと、どのクラスでも使用できるカードとがあります。

### 【シーンカード】

- プレイヤーがいる場所・置かれた状況を表します。
- 【カード番号】がカード左上に記述されています。
- 【フィールドカード】の配置を表す【フィールドパターン】がカード右下に記述されています。

### 【イベントカード】

- プレイヤーがクリアすべき障害を表します。
- それが戦闘である場合、【バトルカード】とも呼びます。
- 【カード番号】がカード左上に記述されています。
- イベントをクリアするための条件【クリア条件】がカード右下に記述されています。
- 【クリティカル条件】【ファンブル条件】がカード右上に記述されています。

### 【SP条件】

- クリティカル条件とファンブル条件をまとめてSP条件と呼びます。

### 【クリティカル】

- イベントを通常より“鮮やかに”クリアした場合です。ボーナスとして得られる効果がクリティカル条件の下に記述されています。

### 【ファンブル】

- イベントはなんとかクリアできたものの、何らかの“代償”を伴う場合です。代償の内容はファンブル条件の下に記述されています。

### 【シナリオカード】

- シーンカードとイベントカードをまとめて【シナリオカード】と呼びます。

### 【パーティー】

- 全プレイヤーは一緒に冒険を行う仲間【パーティー】です。

### 【ストーリーテラー】

- ストーリーテラーはゲームの進行役です。

### 【Lv(レベル)】

- キャラクターが習得できるスキルの上限を表します。レベル1のキャラクターは最高1枚のスキルカードを取得・使用できます。

## 3. 遊び方

### 3.1. 準備

まず、プレイヤーの中から一人、ストーリーテラーを決めます。本ゲームに慣れた方、場を盛り上げるのが上手い方が望ましいでしょう。  
ストーリーテラーはシナリオカードを順番([『シナリオ#1 カードリスト』](scenario/scenario_1.md)参照)に並べ、裏向きに置きます。(→下図(1))  
他のプレイヤーで手分けしてフィールドカード(→下図(2))・スキルカード(→下図(3))をシャッフルし、裏向きに置きます。  

[初期配置]
```
 [(2)] [(1)] [   ] [   ] [(3)]
```
※ "[   ]"はカードが配置されるスペースを表します(以下同様)

各プレイヤーは、自分が担当するキャラクター(クラスカード)を選びます。  

### 3.2. ゲームの流れ

_プレイヤー全員で協力し、イベントクリアを目指しましょう！_  
まず、ストーリーテラーがシナリオカードを1枚めくります。  
それがシーンカードだった場合、カードを下図(4)に置きます。さらに、フィールドパターン通りにフィールドカードを裏向きで並べます。(下図(6)～(11))  

フィールドパターン = 3×2 のとき  
```
 [(2)] [(1)] [(4)] [(5)] [(3)]
 
 [(6)] [   ] [(7)]  [   ] [(8)]
 [   ]       [   ]        [   ]
 [(9)] [   ] [(10)] [   ] [(11)]
```

めくったシナリオカードがイベントカード(バトルカード)だった場合、カードを上図(5)に置きます。そして、クリア条件、SP条件を皆で確認します。  

_数字(フィールドカード)と記号(クラスカード・スキルカード)を組み合わせてイベントクリア条件を満たす計算式を作りましょう！_  
行動順に一人ずつ手番を開始します。行動順は常に、盗賊を先頭として時計回りです。  

自分のクラスカードを任意のフィールドカード間に表向きで(＝記号が見えるように)置きます。このとき、他のクラスカードが既に置かれている場所には置けません。  

しかし、フィールドカードは裏向きになっているため、狙い通りの計算式にするのは困難です。  
クラスカードを置いた後、隣り合う2枚のフィールドカードを手番プレイヤーだけが見ることができます。そして、その部分だけの計算結果と向き(計算した方向)をヒントとしてパーティー全員に報告することが出来ます。  

[例1]
```
 [(6)] [ ÷ ] [(7)] [   ] [(8)]
```
 
占い師(÷)が上図の位置にカードを置き、(6)が「2」、(7)が「5」だったとき、「(7)→(6)で”2”」と報告します。※小数点以下切り捨て  

計算結果からそれぞれのカードの数字をパーティーで推理しあいましょう。そして、どこに残りの記号を置くべきかを協議します。  
ただし、自分が見たカードの数字そのものを口にするのはNGです。  

手番を次のプレイヤーに渡します。  
「【自分の手番】～」と記載されているスキルカードを使うのであればそれまでに使っておかなければいけません。  
スキルカードの効果は配置したときすぐに解決します。  

全てのプレイヤーがクラスカードを配置し終わったとき、1つの計算式として繋がっていない場合はフィールドカードをすべて入れ替えます。そして、クラスカードを一から配置し直します。  
```
 [(6)] [ ÷ ] [(7)]  [   ] [(8)]
 [ + ]       [ - ]        [ × ]  → NG !
 [(9)] [   ] [(10)] [   ] [(11)]
```
何度かやり直しているうちにフィールドカードが足りなくなってしまった場合、即座に _イベントクリア失敗_ となります。  

最後にクラスカードを置いたプレイヤーが計算式の開始位置と終了位置を宣言します。  
このとき、“必ず一度ずつ”すべてのクラスカードを通過するように位置を指定する必要があります。  

使用タイミングの指定がないスキルカードは、自分の手番が終わった後でも配置することができますが、フィールドカードをオープンする前に配置するようにしてください。  

_フィールドカードをオープンして最終的な計算結果を算出します。_  
計算は通常の数学的ルールに基づきます。すなわち…  
* 足し算・引き算より先に、掛け算・割り算を計算します。  
* 0で割ることは出来ません。この場合、 _イベントクリア失敗_ となります。  

[例2]
```
 [(6)] [ ÷ ] [(7)]  [ × ] [(8)]
 [ + ]*      [   ]        [ - ]
 [(9)] [   ] [(10)] [   ] [(11)]
```
※ * = スキルカード「()」  
「開始位置(9)→終了位置(11)：((9)＋(6))÷(7)×(8)－(11)」または「開始位置(11)→終了位置(9)：(11)－(8)×(7)÷((6)＋(9))」のどちらかを選ぶことができます。  

[例3]
```
 [(6)] [   ] [(7)]  [   ] [(8)]
 [   ]       [   ]        [   ]
 [(9)] [   ] [(10)] [   ] [(11)]
```
「開始位置：(6)→(7)→(10)→(9)→終了位置：(6)」「開始位置：(9)→(10)→(7)→(6)→終了位置：(9)」などのパターンが選択できます。  
しかし、「開始位置：(6)→(7)→(10)→終了位置：(9)」はすべてのクラスカードを通過していないので指定できません。  

計算結果がクリア条件を満たせなければ、そこでイベント失敗。ゲーム終了となります。  

計算結果がクリア条件を満たしているとき、見事イベントクリアとなります。  
さらに、クリティカル条件またはファンブル条件を満たしている場合、カードに書かれている指示に従います。  

クリティカルによりスキルカードを獲得した場合、そのカードに「○○専用」と書かれていればそのクラスのキャラクターがスキルを習得します。書かれていない場合はパーティーで話し合って誰が習得するかを決めます。  
一度獲得したスキルはゲーム終了時まで有効(＝使っても消費しない)ですが、他のキャラクターに譲ることは出来ません。  

クラスカードとスキルカードを回収します。  
使用済みのフィールドカードをシャッフルし、未使用フィールドカードの下に入れてください。  
ストーリーテラーは次のシナリオカードをめくり、シナリオを進めます。  

### 3.3. ゲーム終了

以下のいずれかの条件を満たしたとき、ゲーム終了となります。  
* イベントのクリア条件を満たせなかったとき(ゲームオーバー)  
* 用意されたイベントをすべてクリアしたとき(シナリオクリア)  

### 3.4. 選択ルール

* 【推奨】初めてのプレイヤーがパーティーにいる場合かつ1つめのイベントに限り、フィールドカードを表向きに(=数字が見えるように)してプレイする。これは「計算式を組み立てる」イメージを早く掴むために有効です。
* 行動順(クラスカードを配置する順番)は好きなだけ遅らせることが出来ます。  
 例：行動順＝盗賊→占い師→魔法使い→戦士の場合、盗賊は「占い師の後」「魔法使いの後」「戦士の後」のいずれかに行動を遅らせることができます。行動キャンセル(クラスカードを配置しない)はできません。
* シナリオカードをオープンするときにストーリーテラーがシナリオノートを参考に状況説明を行うと、ゲームをより楽しむことができるでしょう。アドリブも大歓迎！
* 用意されたシナリオだけでなく、プレイ可能時間等に合わせてシナリオカードを減らしたり順番を入れ替えたりしても構いません。

### 3.5. 2人プレイ

通常プレイと2人プレイの違いは以下の通りです。

* 一人で2人のキャラクター(クラスカード)を担当します。  
持っているクラスカードのどちらから出してもOKですが、プレイヤーは交互になるようにします。盗賊を担当するプレイヤーが先に出します。  
 例: 占い師(プレイヤー1)→ 戦士(プレイヤー2)→盗賊(プレイヤー1)→魔法使い(プレイヤー2)

### 3.6. ソロプレイ

通常プレイとソロプレイの違いは以下の通りです。

* ストーリーテラーを決める必要はありません。(全部自分でやるしかないので！)
* 一人で4人のキャラクター(クラスカード)を担当します。
* クラスカードを配置したら、隣り合うフィールドカードをオープンに(＝数字が見えるように)します。

## 4. ライセンス

『Xan』は [Creative Commons 表示 2.1 日本 License](http://creativecommons.org/licenses/by/2.1/jp/) で公開されています。  
![クリエイティブ・コモンズ・ライセンス](http://i.creativecommons.org/l/by/2.1/jp/88x31.png)  

よって、あなたはこのリポジトリをForkし、ゲームのルール・カード等を自由に作成・修正することができます！
さらに言うなら商品化し、販売することも自由です。  
『Xan』は"open-design-game"でもあるのです。  
→ ["open-design-game"とは？](http://open-design-games.net/index.php/about)  
