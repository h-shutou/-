---
分野: フィジカルAI
調査日: 2026-11-10
状態: 候補選定
引用数データベース: OpenAlex
tags: []
---
# フィジカルAI

実際のロボットに新しい学習・制御手法を実装し、物体操作や作業の結果を報告する原著研究を選んだ。対象は実機による操作学習と、言語・視覚・行動の統合である。ここでの「実験的」は実機を動かした研究を指す。フィジカルAIの全分野を網羅した引用ランキングではない。

引用数は2026年11月10日にOpenAlex APIの `cited_by_count` で取得した値。同じデータベースで比較し、各行に集計対象のレコードを示す。引用数は収録範囲や版の統合方法で変わり、研究の質や再現性を直接保証するものではない。興味度は利用者が判断するため空欄。

## 候補一覧

| 論文 | 公開年と掲載先 | OpenAlex引用数 | 実機で何を行うか |
| --- | --- | --- | --- |
| RT-1: Robotics Transformer for Real-World Control at Scale | 初公開2022・RSS 2023 | [2,698](https://openalex.org/W4385430679) | 多数の実演から学習し、把持・配置・引き出し操作などを実行 |
| Do As I Can, Not As I Say: Grounding Language in Robotic Affordances（SayCan） | 初公開2022・CoRL 2022、論文集2023 | [2,544](https://openalex.org/W4224912544) | 言語指示を、移動マニピュレータが実行できる技能列に変換 |
| RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control | 2023・CoRL 2023 | [2,111](https://openalex.org/W4385473486) | 視覚言語モデルの知識を、未知物体の選択や意味理解を伴う実機操作へ移転 |
| Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware（ALOHA／ACT） | 2023・RSS 2023 | [2,099](https://openalex.org/W4385430674) | 双腕ロボットで電池挿入、容器開封などの精密操作を模倣学習 |
| Diffusion Policy: Visuomotor Policy Learning via Action Diffusion | 2023・RSS 2023 | [1,321](https://openalex.org/W4385403811) | 拡散モデルで行動列を生成し、押し操作、マグの反転、ソース操作などを実行 |

Diffusion Policyには[ジャーナル拡張版の別レコード](https://openalex.org/W4403337227)（IJRR、オンライン公開2024、818引用）もある。重複する引用がありうるため、会議版と単純合算していない。SayCanとRT-2は表にリンクしたarXiv DOIに対応するレコードの値を使用する。

## 1 RT-1

**正式タイトル**：RT-1: Robotics Transformer for Real-World Control at Scale  
**著者**：Anthony Brohanほか  
**掲載先**：Robotics: Science and Systems XIX（2023）  
**DOI**：10.15607/RSS.2023.XIX.025

- [会議の論文ページ](https://www.roboticsproceedings.org/rss19/p025.html)
- [著者のプロジェクトと実験動画](https://robotics-transformer1.github.io/)
- [公開論文](https://arxiv.org/abs/2212.06817)

画像と言語指示からロボットの動作を出力するTransformerを提案する。実機13台で17か月かけて収集した13万超のエピソード、700超のタスクを用い、物体の把持・配置や引き出し操作などを学習する。データ量・多様性、未知の指示、背景変化などに対する汎化を実機で調べる。

**読む観点**：大量の実機データをどのような入出力表現で学習させるか。学習済みタスクと未知条件での成功をどう区別するか。

**適用上の留意点**：大規模な実演収集を前提とする。報告されたロボットと作業環境での結果を、別機体や任意の環境にそのまま一般化しない。

## 2 SayCan

**正式タイトル**：Do As I Can, Not As I Say: Grounding Language in Robotic Affordances  
**著者**：Michael Ahn、Anthony Brohan、Brian Ichterほか。PDFの著者はアルファベット順に掲載  
**掲載先**：Conference on Robot Learning 2022、PMLR 205:287–318（論文集公開2023）

- [会議の論文ページ](https://proceedings.mlr.press/v205/ichter23a.html)
- [著者のプロジェクトと実験動画](https://say-can.github.io/)
- [公開論文](https://arxiv.org/abs/2204.01691)

言語モデルによる「指示の達成に有用な技能」の評価と、価値関数による「現在の状態で成功できる技能」の評価を組み合わせる。実際のオフィスキッチンと模擬キッチンで、移動マニピュレータを使い101種類の自然言語タスクを評価する。プロジェクトのPaLM-SayCan更新版では、計画成功84%、実行成功74%と報告する。

**読む観点**：言語的にもっともらしい計画を、実機で可能な行動へ接続する方法。計画の正しさと動作の成功率を分けた評価。

**適用上の留意点**：事前学習された技能と成功可能性の評価に依存する。数値は当該環境・モデル版の実験結果であり、未知の任意作業での成功率ではない。

## 3 RT-2

**正式タイトル**：RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control  
**著者**：Anthony Brohanほか。PDFの著者はアルファベット順に掲載  
**掲載先**：Conference on Robot Learning 2023、PMLR 229:2165–2183

- [会議の論文ページ](https://proceedings.mlr.press/v229/zitkovich23a.html)
- [著者のプロジェクトと実験動画](https://robotics-transformer2.github.io/)
- [公開論文](https://arxiv.org/abs/2307.15818)

視覚言語モデルをウェブ由来の視覚言語タスクとロボット軌跡で共同微調整し、ロボット行動をトークンとして出力するVLAモデルを提案する。約6,000回の評価試行を報告し、未知物体や、数字・記号・大小関係などの意味理解を要する指示への汎化を調べる。

**読む観点**：ウェブで学んだ知識を、視覚入力から物理動作を出力するモデルへ移す方法。事前学習、モデル規模、学習方式の比較。

**適用上の留意点**：意味理解を伴う指示への汎化と、新しい運動技能そのものの獲得を区別して読む。比較実験の改善率をあらゆる実環境に共通する値として扱わない。

## 4 ALOHAとACT

**正式タイトル**：Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware  
**著者**：Tony Z. Zhao、Vikash Kumar、Sergey Levine、Chelsea Finn  
**掲載先**：Robotics: Science and Systems XIX（2023）  
**DOI**：10.15607/RSS.2023.XIX.016

- [会議の論文ページ](https://www.roboticsproceedings.org/rss19/p016.html)
- [著者のプロジェクトと実験動画](https://tonyzhaozh.github.io/aloha/)
- [公開論文](https://arxiv.org/abs/2304.13705)

双腕遠隔操作システムALOHAで実演を収集し、行動を1ステップずつではなく、まとまりとして予測するACT（Action Chunking with Transformers）を提案する。電池の挿入や調味料容器の開封など、精密な接触操作を実機で学習する。論文要旨では、特定の難しいタスクについて約10分の実演データから80–90%の成功率を報告する。

**読む観点**：機体構成、実演の集め方、模倣学習、実機での失敗や外乱への反応が一続きで理解できる。実験研究を読む最初の候補として推奨する。

**適用上の留意点**：「低コスト」は研究用ハードウェアとの比較における表現であり、安価なソフトウェア実験を意味しない。上記成功率は全タスク共通の値ではない。

## 5 Diffusion Policy

**正式タイトル**：Diffusion Policy: Visuomotor Policy Learning via Action Diffusion  
**著者**：Cheng Chi、Siyuan Feng、Yilun Du、Zhenjia Xu、Eric Cousineau、Benjamin Burchfiel、Shuran Song（RSS版）  
**掲載先**：Robotics: Science and Systems XIX（2023）。IJRR拡張版はオンライン公開2024  
**DOI**：10.15607/RSS.2023.XIX.026（RSS版）

- [会議の論文ページ](https://www.roboticsproceedings.org/rss19/p026.html)
- [著者のプロジェクト、コード、実験動画](https://diffusion-policy.cs.columbia.edu/)
- [RSS版論文](https://arxiv.org/abs/2303.04137v4)

視覚条件付き拡散モデルで将来の行動列を生成し、観測を更新しながら繰り返し制御する。実機ではT字物体の押し操作、マグの反転、ソースを注ぐ・広げる作業などを評価し、既存の模倣学習法と比較する。

**読む観点**：複数の妥当な動きがありうる行動分布を、拡散モデルでどう扱うか。連続的で滑らかな動作や外乱への対応。

**適用上の留意点**：シミュレーションと実機の結果を区別する。プロジェクトの「平均46.9%改善」は4ベンチマーク・12タスクのシミュレーション比較に関する記述であり、実機全体の平均成功率ではない。RSS版とIJRR版では著者構成や実験範囲も異なる。

## 目的別の読む順番

- **実機実験の設計から理解したい**：ALOHA／ACT → Diffusion Policy。
- **言語モデルをロボットへ接続したい**：SayCan → RT-1 → RT-2。
- **大規模データと汎化を研究したい**：RT-1 → RT-2。

読む順番は実験内容に基づく整理上の提案。実機実験のある原著論文なので、いずれも性能評価や比較による検証を含む。

## 引用数の確認方法

取得対象のOpenAlexレコード：

- RT-1：`W4385430679`
- SayCan：`W4224912544`
- RT-2：`W4385473486`
- ALOHA／ACT：`W4385430674`
- Diffusion Policy RSS版：`W4385403811`
- Diffusion Policy IJRR版：`W4403337227`

再確認例：[RT-1のOpenAlex API](https://api.openalex.org/works/W4385430679?select=id,display_name,publication_year,cited_by_count,doi)。同じ形式でレコードIDを置き換える。Google Scholarなど別サービスの値と混在させず、版による重複も確認する。
