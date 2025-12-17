# Lab Dashboard & CSV Analyzer
##
[text](https://agadaiki.github.io/UWB-csvdata-calculation/)
## プロジェクト概要
GitHub Pagesで動作する、サーバーレスの実験データ解析ダッシュボードです。
Tailwind CSSによるモダンなUIと、JavaScriptによるクライアントサイドでのCSV解析・グラフ化機能を備えています。
##  ファイル構成
* index.html: ポータル画面。各ツールへのリンクと更新履歴を表示。
* analysis.html: CSV解析ツール本体。PapaParseとChart.jsを使用。
## 技術スタック (重要)
このプロジェクトは サーバーレス (Static Site) です。
* Hosting: GitHub Pages
* Frontend Framework: なし (Vanilla JS)
* Styling: Tailwind CSS (CDN版)
* **Libraries**:
    *Chart.js (グラフ描画)
    *PapaParse (CSVパース)

## データ仕様 (CSV)
ユーザーがアップロードするCSVファイル (log_*.csv) の仕様です。
Julesがロジックを改修する際は以下を考慮してください。

* **特記事項**:

* ヘッダー行の列名には、前後に空白が含まれる場合があります（例: " distance"）。

* JS側の PapaParse 設定で transformHeader: header => header.trim() を適用済みです。

## Julesへの開発ロードマップ (指示用)
このプロジェクトを引き継ぐJulesエージェントは、以下のタスクを実施する予定です。
1. 多機能化: distance 以外のカラム（azimuth, elevation）もグラフ表示できるようにセレクトボックスを追加する。
2. 比較機能: 複数のCSVファイルを同時に読み込み、グラフを重ねて比較できるようにする。
3. リファクタリング: コードが長くなった場合、JavaScriptロジックを別ファイル (script.js) に分離する。
Created with Gemini Canvas