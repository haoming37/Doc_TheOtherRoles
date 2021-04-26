# TheOtherRoles

<!-- TOC -->

- [TheOtherRoles](#theotherroles)
  - [概要](#概要)
  - [導入方法](#導入方法)
    - [0. 必要なファイルをダウンロードする](#0-必要なファイルをダウンロードする)
    - [1. インストールディレクトリを開く](#1-インストールディレクトリを開く)
    - [2. au.libhalt.netのプラグインを無効化する](#2-aulibhaltnetのプラグインを無効化する)
    - [3. TheOtherRolesのプラグインを有効化する](#3-theotherrolesのプラグインを有効化する)
    - [4. 起動確認](#4-起動確認)
  - [カスタムロール](#カスタムロール)
    - [インポスター陣営](#インポスター陣営)
      - [Mafia](#mafia)
      - [Morphing](#morphing)
      - [Camouflager](#camouflager)
      - [Vampire](#vampire)
      - [Eraser](#eraser)
      - [Trickster](#trickster)
      - [Cleaner](#cleaner)
      - [Warlock](#warlock)
    - [クルーメイト陣営](#クルーメイト陣営)
      - [Sheriff](#sheriff)
      - [Seer](#seer)
      - [Engineer](#engineer)
      - [Detective](#detective)
      - [Lighter](#lighter)
      - [Medic](#medic)
      - [Mayor](#mayor)
      - [Hacker](#hacker)
      - [Shifter](#shifter)
      - [Time Masters](#time-masters)
      - [Swapper](#swapper)
      - [Tracker](#tracker)
      - [Snitch](#snitch)
      - [Spy](#spy)
    - [第3陣営](#第3陣営)
      - [Child](#child)
      - [Jester](#jester)
      - [Lovers](#lovers)
      - [Jackal](#jackal)
      - [Sidekick](#sidekick)

<!-- /TOC -->

## 概要
できること
- カスタムロールの追加
- 10人以上でのプレイ

## 導入方法
※au.libhalt.netのMod導入済の環境前提

### 0. 必要なファイルをダウンロードする

[TheOtherRoles.dll](https://github.com/haoming37/Doc_TheOtherRoles/raw/master/plugins/TheOtherRoles.dll)  
[me.eisbison.theotherroles.cfg](https://github.com/haoming37/Doc_TheOtherRoles/blob/master/config/me.eisbison.theotherroles.cfg)
### 1. インストールディレクトリを開く
Steamのライブラリ　-> AmongUsを右クリック　→ プロパティ → ローカルファイル　→ ローカルファイルを閲覧
![](images/1.png)
![](images/2.png)
### 2. au.libhalt.netのプラグインを無効化する
2-2. BepingExディレクトリに移動  
2-3. pluginsをplugins_libhaltに名前を変更
2-4. pluginsディレクトリを新規に作成
![](images/3.png)
↓
![](images/4.png)
### 3. TheOtherRolesのプラグインを有効化する
3-1. pluginsディレクトリにTheOtherRoles.dllをコピー  
3-2. configディレクトリにme.eisbison.theotherroles.cfgをコピー

※libhaltの環境で遊ぶ場合はpluginsディレクトリをリネームする(cfgはそのままで問題ないです)

### 4. 起動確認
4-1. ACCOUNTの下にTheOtherRolesの表記があればOK
![](images/menu.png)
4-2. 接続先はCUSTOMを選択する
![](images/custom.png)
※接続できない場合はconfigディレクトリの中身のme.eisbison.theotherroles.cfgの中のIPアドレスが18.177.110.86になっているかを確認する

## カスタムロール
インポスター、クルーメイト、Lovers、Jester、Jackal陣営のロールを追加することができる

### インポスター陣営

---
#### Mafia
3人組のインポスター(インポスター3以上に設定する必要あり)  
Godfather→通常のインポスター  
Mafioso→Godfatherが死ぬと次のインポスターになる、Godfather死ぬまではキルもサボタージュもできない  
Janitor→キルもサボタージュもできない  

---
#### Morphing
近くのプレイヤーをスキャンする→再度使用すると１０秒間スキャンしたプレイヤーの見た目に変身することができる

---

#### Camouflager
カモフラージュボタンを押すと全員の見た目が１０秒間同じになる

---
#### Vampire
キルが噛みつきに変わる  
噛まれた対象は一定時間後に死亡する(デフォルトで10秒)  
※キルクールダウンは死亡後に開始する  
※この時間内にミーティングが開始された場合はミーティング開始時に死亡する  

Vampireがいる場合は全ユーザにニンニクがくばられる  
ニンニクを使用すると設置することができ、その範囲内では噛みつきが通常のキルに変化する(設定でキルそのものができないようにもできる)

---
#### Eraser 
ターゲットにされたプレイヤーは次の会議以降から特殊能力が使えなくなる  
一度使用する毎にクールダウンが10秒ずつ増加していく

---
#### Trickster
他のプレイヤーから見えないボックスを3つ置くことができる  
3つ目が置かれると他のプレイヤーから視認可能になり、Tricksterのみが使用可能なベントになる  
その後、新たな能力として一定時間プレイヤーの視界範囲を狭くすることができる(時間経過で終わる停電状態)

---
#### Cleaner
死体を消すことができる

---
#### Warlock
クルーメイトに呪いをかけることができる
呪いをかけられたクルーメイトが他クルーメイトのそばにいるとき、Warlockは呪いをかけられたクルーメイトで、他クルーメイトを殺すことができる
呪いによって殺すと、呪いは解け、Warlockはしばらく動けなくなる？
呪いによるキルと通常のキルのクールタイムは共通

### クルーメイト陣営

---
#### Sheriff
インポスターを殺すことができる、間違えてクルーメイトを殺そうとした場合は自身が死ぬ（殺そうとした対象は死なない）

---
#### Seer
幽霊が見れる
死んだタイミングで画面が点滅する？
※動作していない気がする

---
#### Engineer
各サボタージュを一度だけどこからでも治せる  
ベントが使える  
エンジニアがベント内にいるとインポスターはベントに青い枠を視認することができる（全てのベントの枠がでる）

---
#### Detective
他のプレイヤーの足跡を見ることができる  
レポートをすると犯人のヒントがゲーム内メッセージでもらえる   
e.g 犯人は暗い色(or 明るい色)だった  
明るい色: pink orange yellow white cyan lime  
暗い色: red blue green grey purple brown  

---
#### Lighter
一定時間（デフォルトで5秒）視野を広くすることができる

---
#### Medic
選択したプレイヤー一人にシールドを張ってキルできなくすることができる。  
メディックが死んだらシールドは消える  
Sheriffがシールドが付いたプレイヤーをキルしようとするとシールドが移動する？  
シールドがついたSheriffがプレイヤーをキルしようとするとシールドが移動する？  
レポートすると死んだ時刻が分かる  

---
#### Mayor
一人で2票分の投票になる  
ミーティングボタンがどこでも押せる  

---
#### Hacker
スキルを有効化すると有効時間内のみ下記の効果が発動する  
Adminがプレイヤーの色付きになる  
Vitalで死亡からの経過時間を見ることができる

---
#### Shifter
選択した他のプレイヤーのロールが奪える  
※第3陣営との入れ替わりが可能  
次の会議が終わると変更が有効になる  
奪われたプレイヤーは普通のクルーメイトになる
インポスター陣営を奪おうとすると自殺する  

---
#### Time Masters
一定時間有効なバリアが貼れる

---
#### Swapper
選択した二人の投票結果の入れ替えができる

---
#### Tracker
選択したプレイヤーのいる方向が矢印で表示されるようになる

---
#### Snitch
タスクが全て終わるとインポスターのいる方向に矢印が出るようになる  
タスクが残り一つになるとインポスター側にSnitchがいる方向に矢印がでるようになる(オプション ON/OFF)

---
#### Spy
インポスターからインポスターと同様に見える  
設定でキル判定について変えることができる
- インポスターがスパイを殺せない
- インポスターがスパイを殺せるが相方のインポスターも殺せる
- Sheriffがスパイを殺せる(オプション ON/OFF)

---

### 第3陣営

---
#### Child
子供から始まって徐々に成長していく
開始時に67%でクルーメイト、33%でインポスターが割当られる

- クルーメイトの場合: 成長が終わる前に追放するとクルーメイト陣営の敗北となる  
- インポスターの場合: 成長中→キルクールダウン2倍　成長後→キルクールダウン2/3倍  

※インポスターは成長するまでChildをキルすることができない

---
#### Jester
てるてる  
釣られたら勝ち

---
#### Lovers
二人組のペア、片方が死んだら両方死ぬ  
両方が生き残った状態でゲームが終了すると勝利になる
相方は名前の色で確認可能だがロールまでは分からない  
インポスターを含めることもできる  
例
```
クルーメイト - クルーメイト  
インポスター - クルーメイト  
```
インポスターとクルーメイトの組み合わせの場合は生存者が下記の組み合わせの場合のみLovers陣営の勝利となる
パターン1　※インポスターも敗北
- Lovers(クルーメイト)
- Lovers(インポスター)

パターン2 ※インポスターも敗北
- Lovers(クルーメイト)
- Lovers(インポスター)
- インポスター

下記のパターンの場合はゲームが終了せずに継続となる  
※lovers(クルーメイト)をキルできればインポスターの勝ち
※クルーメイトをキルできればloversの勝ち
パターン3
- クルーメイト
- Lovers(クルーメイト)
- Lovers(インポスター)
- インポスター

---
#### Jackal
Jackal陣営  
他の陣営のプレイヤーがいなくなると勝利
- タスクなし
- 他の全ての陣営をキルすることができる
- 他のプレイヤーを一人選んでSidekickにすることができる(オプション ON/OFF)
- Jackalが死んだ場合にSidekickがJackalに昇格する(オプション ON/OFF)
- 昇格後に新たなSideKickを選定することができる(オプション ON/OFF)
ベントが使える(オプション ON/OFF)

#### Sidekick
Jackalに選ばれると元々のロールを失ってSideKickになる
- キルができる(オプション ON/OFF)
- ベントが使える(オプション ON/OFF)
