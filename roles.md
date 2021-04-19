# TheOtherRoles

<!-- TOC -->

- [TheOtherRoles](#theotherroles)
  - [概要](#概要)
  - [導入方法](#導入方法)
      - [1.インストールディレクトリを開く](#1インストールディレクトリを開く)
      - [2. au.libhalt.netのプラグインを無効化する](#2-aulibhaltnetのプラグインを無効化する)
      - [3. TheOtherRolesのプラグインを有効化する](#3-theotherrolesのプラグインを有効化する)
  - [カスタムロール](#カスタムロール)
    - [インポスター陣営](#インポスター陣営)
      - [Mafia](#mafia)
      - [Morphing](#morphing)
      - [Camouflager](#camouflager)
      - [Vampire](#vampire)
      - [Eraser](#eraser)
      - [Trickster](#trickster)
    - [クルーメイト陣営](#クルーメイト陣営)
      - [Sheriff](#sheriff)
      - [Seer](#seer)
      - [Engineer](#engineer)
      - [Detective](#detective)
      - [Lighter](#lighter)
      - [Medic](#medic)
      - [Time Master](#time-master)
      - [Swapper](#swapper)
      - [Tracker](#tracker)
      - [Snitch](#snitch)
      - [Jackal](#jackal)
      - [Sidekick](#sidekick)
      - [Spy](#spy)
    - [第3陣営](#第3陣営)
      - [Child](#child)
      - [Jester](#jester)
      - [Lovers](#lovers)

<!-- /TOC -->

## 概要
できること
- カスタムロールの追加
- 10人以上でのプレイ

## 導入方法
※au.libhalt.netのMod導入済の環境前提
#### 1.インストールディレクトリを開く
Steamのライブラリ　-> AmongUsを右クリック　→ プロパティ → ローカルファイル　→ ローカルファイルを閲覧
![](images/1.png)
![](images/2.png)
#### 2. au.libhalt.netのプラグインを無効化する
2-2. BepingExディレクトリに移動  
2-3. pluginsをplugins_libhaltに名前を変更
2-4. pluginsディレクトリを新規に作成
![](images/3.png)
↓
![](images/4.png)
#### 3. TheOtherRolesのプラグインを有効化する
3-1. pluginsディレクトリにTheOtherRoles.dllをコピー
3-2. configディレクトリにme.eisbison.theotherroles.cfgをコピー

※libhaltの環境で遊ぶ場合はpluginsディレクトリをリネームし直してください(cfgはそのままで問題ないです)

## カスタムロール
### インポスター陣営
#### Mafia
3人組のインポスター(インポスター3以上に設定する必要あり)  
Godfather→通常のインポスター  
Mafioso→Godfatherが死ぬと次のインポスターになる、Godfather死ぬまではキルもサボタージュもできない  
Janitor→キルもサボタージュもできない  

#### Morphing
近くのプレイヤーをスキャンする→再度使用すると１０秒間スキャンしたプレイヤーの見た目に変身することができる

#### Camouflager
カモフラージュボタンを押すと全員の見た目が１０秒間同じになる

#### Vampire
キルが噛みつきに変わる  
噛まれた対象は一定時間後に死亡する(デフォルトで10秒)  
※キルクールダウンは死亡後に開始する  
※この時間内にミーティングが開始された場合はミーティング開始時に死亡する  

Vampireがいる場合は全ユーザにニンニクがくばられる  
ニンニクを使用すると設置することができ、その範囲内では噛みつきが通常のキルに変化する(設定でキルそのものができないようにもできる)

#### Eraser 
ターゲットにされたプレイヤーは次の会議以降から特殊能力が使えなくなる  
一度使用する毎にクールダウンが10秒ずつ増加していく

#### Trickster
他のプレイヤーから見えないボックスを3つ置くことができる  
3つ目が置かれると他のプレイヤーから視認可能になり、Tricksterのみが使用可能なベントになる  
その後、新たな能力として一定時間プレイヤーの視界範囲を狭くすることができる(時間経過で終わる停電状態)

### クルーメイト陣営
#### Sheriff
インポスターを殺すことができる、間違えてクルーメイトを殺そうとした場合は自身が死ぬ（殺そうとした対象は死なない）

#### Seer
幽霊が見れる
死んだタイミングで画面が点滅する？
※上手く動作していない気がする

#### Engineer
各サボタージュを一度だけどこからでも治せる  
ベントが使える  
エンジニアがベント内にいるとインポスターはベントに青い枠を視認することができる（全てのベントの枠がでる）

#### Detective
他のプレイヤーの足跡を見ることができる  
レポートをすると犯人のヒントがゲーム内メッセージでもらえる   
e.g 犯人は暗い色(or 明るい色)だった
明るい色: pink orange yellow white cyan lime
暗い色: red blue green grey purple brown

#### Lighter
一定時間（デフォルトで5秒）視野を広くすることができる

#### Medic
#### Time Master
#### Swapper
#### Tracker
#### Snitch
#### Jackal
#### Sidekick
#### Spy

### 第3陣営
#### Child
67%でクルーメイト、33%でインポスターになる  
クルーメイトの場合は成長が終わる前に追放するとクルーメイト陣営の敗北となる
インポスターの場合: 成長中→キルクールダウン2倍　成長後→キルクールダウン2/3倍
※インポスターは成長するまでChildをキルすることができない

#### Jester
てるてる  
釣られたら勝ち

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