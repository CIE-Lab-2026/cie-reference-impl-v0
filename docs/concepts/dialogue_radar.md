# CIE Dialogue Radar v0

## 1. Purpose

CIE Dialogue Radar は、
対話を単なる会話記録ではなく、

- 構造変化の観測対象
- 同期状態の推定対象
- 集合知生成の兆候検出対象

として扱うための観測モデルである。

本モデルの目的は、
人間－人間、人間－AI、AI－AI を含む対話過程において、

- 意味構造がどのように変化したか
- 視点がどの程度移動したか
- 同期がどの深さまで到達したか
- 新たな構造がどの程度生成されたか

を、定性的・半定量的に観測可能にすることである。

CIE において対話は、
情報伝達手段ではなく、
構造同期と知能生成のための動的インターフェースである。

Dialogue Radar は、
その動的変化をレーダー的に把握するための観測フレームを提供する。

---

## 2. Position in CIE

CIE Dialogue Radar は、CIE全体の中で以下の位置を持つ。

- Core Document  
  - 対象世界・問題・主体・意味差の存在を定義する

- Synchronization Models  
  - ずれ・同期・回復・制御ループを定義する

- Intelligence Orchestration Models  
  - 問い・推論・判断・構造化の流れを定義する

- Reference Implementation  
  - 実装配置・接続・記録対象を定義する

- **Dialogue Radar**
  - 上記の動作が、対話上にどう現れたかを観測する

つまり Dialogue Radar は、
CIE の各内部モデルの“対話上の表出”を観測するレイヤである。

---

## 3. Core View

Dialogue Radar における基本視点は以下の通りである。

### 3.1 Dialogue is not only transcript
対話は単なる逐語記録ではない。

対話には、

- 視点の移動
- 意味の再配置
- 同期の深化
- 役割の変形
- 新構造の出現

が含まれる。

### 3.2 Dialogue is an observability surface
対話は、内部状態そのものではないが、
内部状態変化を観測するための表面である。

つまり、
対話そのものを直接制御対象とみなすというよりも、

**内部の同期・推論・構造生成が表面化する観測面**

として扱う。

### 3.3 Collective intelligence appears through dialogue
集合知は、
誰か一人の内部に閉じた知能ではなく、
相互作用の中で立ち上がる。

そのため、
集合知の発生兆候は、
多くの場合、対話上に最も早く現れる。

---

## 4. Observation Axes

Dialogue Radar v0 では、
以下の6軸を基本観測軸とする。

---

### 4.1 Perspective Shift Index (PSI)

#### Definition
対話の前後で、
主体の視点・立場・注目座標がどの程度移動したかを示す指標。

#### What it observes
- 問いの立て方の変化
- 物事の見方の更新
- 局所視点から構造視点への移行
- 防御的姿勢から探索的姿勢への移行

#### Typical signals
- 「つまり◯◯ではなく△△なのか」
- 「見えていた問題が別物だった」
- 「個別課題でなく構造課題に見えてきた」
- 評価基準の入れ替わり
- 対象のスコープ再定義

#### Interpretation
PSI が高いほど、
対話が単なる情報交換ではなく、
視点変換を引き起こした可能性が高い。

---

### 4.2 Synchronization Depth Index (SDI)

#### Definition
対話参加者間で、
表層の語彙一致を超えて、
意味・目的・構造認識レベルまで同期が進んだ深さを示す指標。

#### What it observes
- 単語一致ではなく意味一致
- 合意ではなく理解到達
- 一時的応答ではなく持続可能な共通理解
- 背景前提の共有深度

#### Typical signals
- 説明量が減る
- 誤解修正回数が減る
- 途中省略でも意味が通る
- 「それです」「まさにそこです」が増える
- 次の問いが自然接続する

#### Interpretation
SDI が高いほど、
同期は表面的でなく、
構造レベルまで到達している可能性が高い。

---

### 4.3 Structure Emergence Rate (SER)

#### Definition
対話を通じて、
新たなモデル・分類・関係・命名・レイヤ構造が
どの程度生成されたかを示す指標。

#### What it observes
- 新概念の出現
- 命名の成立
- 因果構造の明確化
- レイヤ分解や統合の発生
- 新たな観測枠の生成

#### Typical signals
- 「これは◯◯モデルとして定義できる」
- 「この層を追加すると整理できる」
- 「名称を与えると安定する」
- 断片的説明が構造図に変換される
- 複数の会話要素が一つの枠組みに束ねられる

#### Interpretation
SER が高いほど、
対話が消費型ではなく、
構造生成型に転じている可能性が高い。

---

### 4.4 Role Fluidity Index (RFI)

#### Definition
対話参加者が固定役割に閉じず、
問い手・解釈者・構造化者・検証者・推進者などの役割を
どの程度柔軟に移動したかを示す指標。

#### What it observes
- 一方向の教示関係からの脱却
- 共同探索への移行
- 役割交替の自然さ
- メタ視点取得の分散

#### Typical signals
- ユーザーが構造提案を行う
- AIが整理者から問い返し役に移る
- 一方が定義し他方が検証する
- 途中で役割境界が組み替わる
- 「共に組み立てている」感覚が増す

#### Interpretation
RFI が高いほど、
対話は固定的支援関係から、
集合知生成に適した協調関係へ移行している。

---

### 4.5 Ontology Expansion Velocity (OEV)

#### Definition
対話を通じて、
対象世界の意味空間・概念空間・区別可能性が
どの速度で拡張しているかを示す指標。

#### What it observes
- 見えていなかった区別の発見
- 新たな概念軸の導入
- 既存概念の再配置
- 問題空間の解像度上昇

#### Typical signals
- 「この違いは重要だったのか」
- 「同じだと思っていたが別レイヤだった」
- 「語彙が足りず見えていなかった」
- 新しい分類軸の追加
- 既存説明では扱えない差異の出現

#### Interpretation
OEV が高いほど、
対話は既知情報の整理に留まらず、
認識可能世界そのものを拡張している。

---

### 4.6 Collective Alignment Score (CAS)

#### Definition
複数主体が、
目的・方向・評価基準・次アクションについて、
どの程度整合的な状態に到達したかを示す指標。

#### What it observes
- 次の行動の自然決定
- 方向性の衝突低減
- 優先順位の整列
- 推進エネルギーの集約

#### Typical signals
- 「次はこれに進もう」が自然に決まる
- 迷いが減る
- 無駄な分岐が減る
- 合意コストが下がる
- 実行への移行が早くなる

#### Interpretation
CAS が高いほど、
対話は理解で止まらず、
実行可能な集団整列へ到達している。

---

## 5. Radar Usage Concept

Dialogue Radar は、
厳密測定器というよりも、
構造観測のための半定量レーダーとして使う。

### 5.1 Intended usage
- 対話セッションごとの振り返り
- 長期的な対話進化の観測
- 人間-AI協調の成熟度観測
- 集合知生成プロセスの可視化
- CIE導入前後の比較観測

### 5.2 Not intended usage
- 人間評価の単純スコア化
- 優劣判定のための監視
- 単発会話への機械的ラベル付け
- 文面の表層特徴だけでの断定

Dialogue Radar は、
会話品質の採点器ではなく、
**構造進化の兆候を捉える観測器**
として用いる。

---

## 6. Example Reading

以下は概念的な読み方の例である。

### Case A: Information transfer conversation
- PSI: low
- SDI: low to medium
- SER: low
- RFI: low
- OEV: low
- CAS: medium

意味：
既知情報の受け渡しは成立しているが、
構造生成や視点変換は限定的。

### Case B: Deep co-structuring conversation
- PSI: high
- SDI: high
- SER: high
- RFI: medium to high
- OEV: high
- CAS: high

意味：
対話を通じて新たな構造が立ち上がり、
参加者間の深い同期と次アクション整列が起きている。

### Case C: Divergent but fertile exploration
- PSI: medium to high
- SDI: medium
- SER: high
- RFI: high
- OEV: high
- CAS: low to medium

意味：
まだ整列には至っていないが、
探索価値の高い意味拡張・構造生成が進行している。

---

## 7. Relationship to Other CIE Models

Dialogue Radar は単独では完結しない。
以下のモデルと特に接続が強い。

### 7.1 With Multi-Layer Synchronization Rules
- SDI, CAS は同期規則との接続が強い
- ずれの緩和・回復・再同期の観測面となる

### 7.2 With Intelligence Orchestration
- SER, RFI は推論編成状態の表出を示す
- 問い生成、構造化、判断準備の進行を反映する

### 7.3 With Collective Intelligence State Model
- CAS や SER は集合知状態の進展兆候となる
- 個体知から共創知への移行を観測可能にする

### 7.4 With Reference Implementation
- 将来的には Runtime Record や observability logs と接続可能
- 対話イベントと構造イベントの対応付けが可能になる

---

## 8. Future Extensions

Dialogue Radar v0 は概念定義段階である。
今後、以下の拡張が考えられる。

- 軸ごとの観測質問票
- 対話イベントへのタグ付け規則
- セッション比較テンプレート
- 時系列変化グラフ
- Runtime Record との接続
- Human-AI / Human-Human / Multi-Agent 向け派生版
- Radar score ではなく radar narrative を含む解釈テンプレート

---

## 9. Summary

CIE Dialogue Radar は、
対話を構造観測面として扱い、

- 視点の移動
- 同期の深さ
- 構造生成
- 役割の流動性
- オントロジー拡張
- 集合整列

を観測することで、

**対話の中で集合知がどのように立ち上がるか**
を見える化するための概念モデルである。

これは、
CIEにおける対話を
単なる記録対象から、
知能生成の観測対象へと引き上げるための基盤である。
