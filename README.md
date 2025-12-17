# UWB analysis | UWBデータ解析ツール
##
[text](https://agadaiki.github.io/UWB-csvdata-calculation/)
## 概要
UWB analysisは, 「MURATA UWB Type 2BP」 の出力ファイルに焦点を当てた解析ツールである.
##  ファイル構成
* index.html: ポータル画面。各ツールへのリンクと更新履歴を表示。
* analysis.html: CSV解析ツール本体。PapaParseとChart.jsを使用。
* **Libraries**:
    *Chart.js (グラフ描画)
    *PapaParse (CSVパース)


* **特記事項**:

* ヘッダー行の列名には、前後に空白が含まれる場合があります（例: " distance"）。

* JS側の PapaParse 設定で transformHeader: header => header.trim() を適用済みです。
