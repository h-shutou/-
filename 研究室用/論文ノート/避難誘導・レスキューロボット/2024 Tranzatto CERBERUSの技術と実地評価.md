---
タイトル: "Team CERBERUS Wins the DARPA Subterranean Challenge: Technical Overview and Lessons Learned"
ジャーナル: "Field Robotics"
掲載先: "Field Robotics"
出版名: "Field Robotics（刊行組織の正式名称は未確認）"
著者名: ["Marco Tranzatto", "Mihir Dharmadhikari", "Lukas Bernreiter", "Marco Camurri", "Shehryar Khattak", "Frank Mascarich", "Patrick Pfreundschuh", "David Wisth", "Samuel Zimmermann", "Mihir Kulkarni", "Victor Reijgwart", "Benoit Casseau", "Timon Homberger", "Paolo De Petris", "Lionel Ott", "Wayne Tubby", "Gabriel Waibel", "Huan Nguyen", "Cesar Cadena", "Russell Buchanan", "Lorenz Wellhausen", "Nikhil Khedekar", "Olov Andersson", "Lintong Zhang", "Takahiro Miki", "Tung Dang", "Matias Mattamala", "Markus Montenegro", "Konrad Meyer", "Xiangyu Wu", "Adrien Briod", "Mark Mueller", "Maurice Fallon", "Roland Siegwart", "Marco Hutter", "Kostas Alexis"]
出版年: 2024
初公開日: "2022-07-11"
参照版公開日: "2022-07-11"
論文種別: "実機統合システムの競技評価"
協働ロボット: "有（誘導・操作・監督のHRI。産業用cobot認証の意味ではない）"
使用ロボット: ["ANYmal C", "RMF-Owl", "Alpha Aerial Scout", "Kolibri", "移動通信拠点・中継モジュール"]
協働形態: "監督型自律。最終競技では自律的なロボット間協調手法は未投入"
新規性要約: "地下探索システムの予備走行・最終競技・失敗・運用上の教訓を詳細報告"
DOI: "10.55417/fr.2024009"
URL: "https://doi.org/10.55417/fr.2024009"
PDF: ""
文献ID: "tranzatto2024cerberustechnical"
参照経路: "出版社・arXiv・著者公開資料・機関書誌（Google Scholar以外）"
Google Scholar参照: "未確認"
確認範囲: "arXiv:2207.04914v1全文。2024年掲載版との全差分は未照合"
読書状況: "整理済み"
tags: []
作成日: "2026-11-18"
資料確認日: "2026-11-17"
---
# Team CERBERUS Wins the DARPA Subterranean Challenge: Technical Overview and Lessons Learned

**要点：地下探索システムの予備走行・最終競技・失敗・運用上の教訓を詳細報告。**

確認範囲：arXiv:2207.04914v1全文。2024年掲載版との全差分は未照合。興味度は `tags` に `high`・`middle`・`low` のいずれか1つを設定する。PDFは添付せず出典URLを記載する。

参照本文は2022-07-11のarXiv v1、書誌年・DOIは2024年掲載版。版の全差分は未照合。

## アブストラクト

機体、学習型移動、知覚、地図、探索、通信、運用を詳述し、予備試験と最終競技を評価する。失敗・人の介入・開発上の教訓も扱う。（1、3–5節）

## 背景

地下探索では移動・認識・通信の制約が重なり、人が入る前の状況把握には各要素を統合した頑健なシステムが必要。（1節）

## 方法

ANYmal Cと飛行機を中心に複数センサ知覚、SLAM、地図共有、探索計画、物体検出と中継通信を統合。人一人が高位指示を出す。予備実地試験・予選・60分本走行で得点、距離、自律モード、地図誤差を評価。（3–4節）

## 結果

最終競技は23/40対象。Table 3の四脚機距離は240、687、311、500 mで計1,738 m。CSIROと23点で並び報告時刻で優勝。転倒はなかったが、物体報告の処理や地図生成の課題が残る。（4.2節、Table 3、5.1節）

## 考察

### 著者の解釈

頻繁な実地試験、頑健な機体、複数センサと監督型自律が性能を支えたとする。通信外で個々の機体が探索できることを重視。（5節）

### 自分の考察

ANYmal Parkourのような単体移動研究を対象発見・情報伝達へ接続して読める。人の介入率と失敗回復も評価したい。

## 先行研究との新規性

異種機体の移動・知覚・計画・通信を統合し、実地での性能と教訓を詳しく報告。2022年の概要と同じ競技結果を扱う。

## 限界

著者は知覚劣化、地図計算負荷、意味理解・リスク判断・操作能力の不足を指摘。開発中の自律的なロボット間協調法は最終競技に未投入。実災害の人の搬出は評価しない。（5.1節）

## 応用可能性

鉱山・トンネル・地下施設の探索と先行偵察。追加案は捜索漏れ、通信復帰、操作者負荷を含む評価。

## 疑問と次に調べること

- [ ] 興味度を設定する。
- [ ] 公開データで誤検知・位置誤差・介入を調べる。
- [ ] 競技後の協調法と脚式・飛行機連携を追う。

## 出典と関連論文

文献ID：`tranzatto2024cerberustechnical`。著者全員は上部プロパティに記録。[掲載・公開版DOI](https://doi.org/10.55417/fr.2024009)。

- [参照したarXiv v1](https://arxiv.org/pdf/2207.04914v1)
- [全著者・版履歴](https://arxiv.org/abs/2207.04914)
- [著者公開データ](https://github.com/leggedrobotics/cerberus_darpa_subt_datasets)
- [[参考文献/参考文献一覧|共通参考文献一覧]]と `references.bib` に同じ文献IDで登録。
- [[文献探索/避難誘導の後続研究とレスキューロボットの有力論文|8本の候補比較・引用数・取得経路]]。

### 関連ノート

- [[論文ノート/避難誘導・レスキューロボット/2025 Nayyar 避難誘導の実験と行動モデル|2025 Nayyar 避難誘導の実験と行動モデル]]
- [[論文ノート/避難誘導・レスキューロボット/2026 Yin VRと実機の避難誘導比較|2026 Yin VRと実機の避難誘導比較]]
- [[論文ノート/避難誘導・レスキューロボット/2023 Nayyar 避難者モデルの学習|2023 Nayyar 避難者モデルの学習]]
- [[論文ノート/避難誘導・レスキューロボット/2016 Robinette 避難誘導ロボットへの過信|2016 Robinette 避難誘導ロボットへの過信]]
- [[論文ノート/避難誘導・レスキューロボット/2003 Casper WTC捜索救助の人とロボット|2003 Casper WTC捜索救助の人とロボット]]
- [[論文ノート/避難誘導・レスキューロボット/2013 Nagatani 福島原発事故とQuince|2013 Nagatani 福島原発事故とQuince]]
- [[論文ノート/避難誘導・レスキューロボット/2022 Tranzatto CERBERUSの地下探索概要|2022 Tranzatto CERBERUSの地下探索概要]]
