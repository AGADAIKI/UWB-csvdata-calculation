# UWB analysis | UWBデータ解析ツール
##
[https://agadaiki.github.io/UWB-csvdata-calculation/](https://agadaiki.github.io/UWB-csvdata-calculation/)
## 概要
UWB analysisは, 「MURATA UWB Type 2BP」 の出力csvファイルに焦点を当てた解析ツールである.

## TODO 
* 出力グラフの保存
* Type 2BP の .binファイル書き換えのGUI化

##  ファイル構成
* index.html: ポータル画面。各ツールへのリンクと更新履歴を表示。
* analysis.html: CSV解析ツール本体。PapaParseとChart.jsを使用。
* **Libraries**:
    *Chart.js (グラフ描画)
    *PapaParse (CSVパース)

## その他
* **特記事項**:

* ヘッダー行の列名には、前後に空白が含まれる場合があります（例: " distance"）。

* JS側の PapaParse 設定で transformHeader: header => header.trim() を適用済みです。
