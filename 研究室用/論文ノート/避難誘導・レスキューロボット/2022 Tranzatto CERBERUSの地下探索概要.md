---
タイトル: "CERBERUS in the DARPA Subterranean Challenge"
ジャーナル: "Science Robotics"
掲載先: "Science Robotics"
出版名: "American Association for the Advancement of Science"
著者名: ["Marco Tranzatto", "Takahiro Miki", "Mihir Dharmadhikari", "Lukas Bernreiter", "Mihir Kulkarni", "Frank Mascarich", "Olov Andersson", "Shehryar Khattak", "Marco Hutter", "Roland Siegwart", "Kostas Alexis"]
出版年: 2022
初公開日: "2022-05-25"
参照版公開日: null
論文種別: "Viewpoint（競技システムの概要）"
協働ロボット: "有（誘導・操作・監督のHRI。産業用cobot認証の意味ではない）"
使用ロボット: ["ANYmal C", "飛行ロボット", "移動通信拠点・中継モジュール"]
協働形態: "人1人の高位監督と複数機の運用"
新規性要約: "脚式・飛行ロボットと知覚・探索・通信を統合する地下探索システムの概要を提示"
DOI: "10.1126/scirobotics.abp9742"
URL: "https://doi.org/10.1126/scirobotics.abp9742"
PDF: ""
文献ID: "tranzatto2022cerberus"
参照経路: "出版社・arXiv・著者公開資料・機関書誌（Google Scholar以外）"
Google Scholar参照: "未確認"
確認範囲: "出版社抄録・機関書誌・共著者解説。掲載版本文は未確認"
読書状況: "読書中"
tags: []
作成日: "2026-11-18"
資料確認日: "2026-11-17"
---
# CERBERUS in the DARPA Subterranean Challenge

**要点：脚式・飛行ロボットと知覚・探索・通信を統合する地下探索システムの概要を提示。**

確認範囲：出版社抄録・機関書誌・共著者解説。掲載版本文は未確認。興味度は `tags` に `high`・`middle`・`low` のいずれか1つを設定する。PDFは添付せず出典URLを記載する。

## アブストラクト

DARPA SubT最終競技で優勝したCERBERUSの技術と戦略を紹介する。歩行・飛行ロボットによる知覚・地図・探索・通信を統合した概要論文。（抄録、共著者解説）

## 背景

地下の暗所・煙・不整地・GPS欠如・通信断が同時に起こるため、技術の個別性能だけでは探索継続性を保証できない。

## 方法

複数機を人一人の高位監督下で運用する。60分で40対象を探索し種類と位置を報告する競技を扱う。詳細な条件と評価は2024年の技術報告ノートへ分ける。（共著者解説）

## 結果

共著者の公開解説では四脚機4台が計1.7 km超を移動し23/40対象を得点。CSIROとの同点を最終得点の報告時刻で制し優勝。実被災者の救出件数を示すものではない。

## 考察

### 著者の解釈

機体の補完関係、知覚の冗長性、監督型自律を成功の要素として説明する。（共著者解説）

### 自分の考察

全体の見取り図として読み、詳細報告で失敗や介入を確認するとよい。同じ競技を独立した2回の実験と数えない。

## 先行研究との新規性

複数技術を統合した地下探索システムの要点と実地成果を提示。単一アルゴリズムの比較実験が中心の論文ではない。

## 限界

短いViewpointで、機関書誌はReview Articleとも分類する。掲載版本文は未確認。完全なロボット間自律協調を最終競技で実証したとは断定しない。

## 応用可能性

地下災害の先行偵察や施設点検。現場転用では危険度・通信・見逃しを含めた別評価を要する。

## 疑問と次に調べること

- [ ] 興味度を設定する。
- [ ] 掲載版本文を確認する。
- [ ] 詳細報告と公開走行データを対応づける。

## 出典と関連論文

文献ID：`tranzatto2022cerberus`。著者全員は上部プロパティに記録。[掲載・公開版DOI](https://doi.org/10.1126/scirobotics.abp9742)。

- [ETH機関書誌](https://www.research-collection.ethz.ch/entities/publication/d362c6ae-694e-4ae5-a936-01709fe1310e)
- [共著者による解説](https://takahiromiki.com/explainers/cerberus-science-robotics/)
- [[参考文献/参考文献一覧|共通参考文献一覧]]と `references.bib` に同じ文献IDで登録。
- [[文献探索/避難誘導の後続研究とレスキューロボットの有力論文|8本の候補比較・引用数・取得経路]]。

### 関連ノート

- [[論文ノート/避難誘導・レスキューロボット/2025 Nayyar 避難誘導の実験と行動モデル|2025 Nayyar 避難誘導の実験と行動モデル]]
- [[論文ノート/避難誘導・レスキューロボット/2026 Yin VRと実機の避難誘導比較|2026 Yin VRと実機の避難誘導比較]]
- [[論文ノート/避難誘導・レスキューロボット/2023 Nayyar 避難者モデルの学習|2023 Nayyar 避難者モデルの学習]]
- [[論文ノート/避難誘導・レスキューロボット/2016 Robinette 避難誘導ロボットへの過信|2016 Robinette 避難誘導ロボットへの過信]]
- [[論文ノート/避難誘導・レスキューロボット/2003 Casper WTC捜索救助の人とロボット|2003 Casper WTC捜索救助の人とロボット]]
- [[論文ノート/避難誘導・レスキューロボット/2013 Nagatani 福島原発事故とQuince|2013 Nagatani 福島原発事故とQuince]]
- [[論文ノート/避難誘導・レスキューロボット/2024 Tranzatto CERBERUSの技術と実地評価|2024 Tranzatto CERBERUSの技術と実地評価]]
