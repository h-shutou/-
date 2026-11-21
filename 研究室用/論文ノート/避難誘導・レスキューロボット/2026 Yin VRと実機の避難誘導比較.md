---
タイトル: "Validation and Evacuee Modeling of Virtual Robot-guided Emergency Evacuation Experiments"
ジャーナル: "ACM Transactions on Human-Robot Interaction"
掲載先: "ACM Transactions on Human-Robot Interaction"
出版名: "Association for Computing Machinery"
著者名: ["Yinxuan Yin", "Mollik Nayyar", "Daniel Holman", "Ghanghoon Paik", "Savanna Spazak", "Gale Lucas", "Colin Holbrook", "Alan R. Wagner"]
出版年: 2026
初公開日: "2024-06-24"
参照版公開日: "2025-06-04"
論文種別: "VR・実機比較と相互位置予測"
協働ロボット: "有（誘導・操作・監督のHRI。産業用cobot認証の意味ではない）"
使用ロボット: ["VR内の双腕付き移動誘導ロボット", "対応する実機（掲載版の機種は未確認）"]
協働形態: "VRと実機での人への避難誘導・追従"
新規性要約: "対応する物理・VR環境の行動を比較し、VRデータから実環境の軌跡を予測"
DOI: "10.1145/3861077"
URL: "https://doi.org/10.1145/3861077"
PDF: ""
文献ID: "yin2026virtualevacuation"
参照経路: "出版社・arXiv・著者公開資料・機関書誌（Google Scholar以外）"
Google Scholar参照: "未確認"
確認範囲: "PsyArXiv v2全文とACM掲載版の登録書誌・抄録。掲載版全文は未確認"
読書状況: "読書中"
tags: []
作成日: "2026-11-18"
資料確認日: "2026-11-17"
掲載版公開日: "2026-11-07"
公開版著者差分: "PsyArXiv v2はJared Armagostを含む9名。ACM掲載版登録は上記8名"
---
# Validation and Evacuee Modeling of Virtual Robot-guided Emergency Evacuation Experiments

**要点：対応する物理・VR環境の行動を比較し、VRデータから実環境の軌跡を予測。**

確認範囲：PsyArXiv v2全文とACM掲載版の登録書誌・抄録。掲載版全文は未確認。興味度は `tags` に `high`・`middle`・`low` のいずれか1つを設定する。PDFは添付せず出典URLを記載する。

公開版：OSF v1は2024-06-24、参照v2は2025-06-04。掲載版は2026-11-07。以下の人数・詳細は公開版に基づく。

## アブストラクト

実機の避難誘導実験をVRで再現し、出口選択・避難時間・信頼を比較する。公開版v2の詳細と、ACM掲載版抄録の位置誤差0.42 mを区別して記録する。

## 背景

VRで安全に反復できても、実機を前にした行動が再現されるとは限らない。その対応を検討する。（公開版1–2節）

## 方法

公開版v2ではUnity・HMD・Cybershoesを使い、VR25人と過去の実機14人を比較。警報後の近い出口／誘導先の遠い出口への反応を測定し、VR→実環境と逆方向の位置モデル転用を評価する。事前登録を記載。（3–4節）

## 結果

- 公開版：実機12/14人、VR20/25人が追従。（5.1節）
- 公開版：VR→実環境の平均位置誤差41.7 cm、逆方向29 cm。（5.4節、Figs.5–6）
- 公開版要旨の「0.42 centimeters」は本文の41.7 cmと不一致。掲載版抄録は0.42 metersで、0.42 cmの精度とは解釈しない。

## 考察

### 著者の解釈

対応するVRなら、実機実験の費用・場所・倫理上の制約を軽減しながら行動モデルを作れると論じる。（公開版6節）

### 自分の考察

行動が概ね似ていることと統計的同等性は別。警報やVR移動操作が反応へ与える影響を確認したい。

## 先行研究との新規性

仮想実験の行動比較に加え、VRデータから実環境の軌跡を予測する。2026年は掲載年で、初公開はOSF v1の2024-06-24。

## 限界

公開版が挙げる制約は小標本、異なる募集・実施時期、座位の足操作、単純な経路。掲載版全文の変更は未照合。公開版はJared Armagostを含む9著者、ACM登録は8著者で、差分を混同しない。（公開版6節）

## 応用可能性

VRで条件を絞り実機で再評価する実験設計。実災害の生存率改善までは検証していない。

## 疑問と次に調べること

- [ ] 興味度を設定する。
- [ ] 掲載版全文の人数・統計・著者・図表変更を確認する。
- [ ] 複雑な経路と異なる年齢集団で再現する。

## 出典と関連論文

文献ID：`yin2026virtualevacuation`。著者全員は上部プロパティに記録。[掲載・公開版DOI](https://doi.org/10.1145/3861077)。

- [掲載版登録書誌・抄録](https://api.crossref.org/works/10.1145/3861077)
- [公開版v2](https://osf.io/preprints/psyarxiv/mr78s_v2)
- [公開版履歴](https://api.osf.io/v2/preprints/mr78s_v2/versions/)
- [[参考文献/参考文献一覧|共通参考文献一覧]]と `references.bib` に同じ文献IDで登録。
- [[文献探索/避難誘導の後続研究とレスキューロボットの有力論文|8本の候補比較・引用数・取得経路]]。

### 関連ノート

- [[論文ノート/避難誘導・レスキューロボット/2025 Nayyar 避難誘導の実験と行動モデル|2025 Nayyar 避難誘導の実験と行動モデル]]
- [[論文ノート/避難誘導・レスキューロボット/2023 Nayyar 避難者モデルの学習|2023 Nayyar 避難者モデルの学習]]
- [[論文ノート/避難誘導・レスキューロボット/2016 Robinette 避難誘導ロボットへの過信|2016 Robinette 避難誘導ロボットへの過信]]
- [[論文ノート/避難誘導・レスキューロボット/2003 Casper WTC捜索救助の人とロボット|2003 Casper WTC捜索救助の人とロボット]]
- [[論文ノート/避難誘導・レスキューロボット/2013 Nagatani 福島原発事故とQuince|2013 Nagatani 福島原発事故とQuince]]
- [[論文ノート/避難誘導・レスキューロボット/2022 Tranzatto CERBERUSの地下探索概要|2022 Tranzatto CERBERUSの地下探索概要]]
- [[論文ノート/避難誘導・レスキューロボット/2024 Tranzatto CERBERUSの技術と実地評価|2024 Tranzatto CERBERUSの技術と実地評価]]
