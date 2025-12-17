
# Economy Collaborators Visualizer

GitHub Innovation Graph のデータを活用し、世界各国の経済間におけるコラボレーション（協力関係）をインタラクティブなコード図（Chord Diagram）で可視化するツールです。

## 1. これができること

* **双方向の可視化**: 国から国への「流出」と「流入」を、帯の太さと向きで直感的に把握できます。
* **スマート・ランキング**: 送り手（Source）や受け手（Destination）を選択すると、関連の強い順に国リストが自動で並び替わります。
* **時系列分析**: 年・四半期ごとのデータを切り替えて、関係性の変遷を追うことができます。
* **動的フィルタリング**: 膨大な国々の中から、特定の国同士の関係だけに絞り込んで分析可能です。

## 2. データソースについて

本プロジェクトは、GitHubが公開している **GitHub Innovation Graph** の貴重なデータを分析・学習するために作成されました。素晴らしいデータの公開に深く感謝いたします。

* **参照元データ**: [Top Economy Collaborators](https://innovationgraph.github.com/global-metrics/economy-collaborators#top-economy-collaborators)
* **使用ファイル**: [economy_collaborators.csv](https://github.com/github/innovationgraph/blob/main/data/economy_collaborators.csv)
* 本ツールでは **2025年12月時点** までの最新データを反映して動作することを確認しています。


* **ライセンス**: [CC-1.0 (Creative Commons Zero v1.0 Universal)](https://github.com/github/innovationgraph/blob/main/LICENSE.md)

## 3. 環境要件

* **Webブラウザ**: モダンブラウザ（Google Chrome, Microsoft Edge, Firefox, Safari等）
* **ローカルサーバー環境**: JavaScriptのセキュリティ（CORS）制限により、CSVファイルを読み込むためにローカルサーバーが必要です。
* 例: Python 3.x がインストールされている環境



## 4. セットアップと実行手順

### ステップ 1: ファイルの準備

同じフォルダ内に、以下の2つのファイルを配置してください。

1. `index.html` （作成したHTMLコード）
2. `economy_collaborators.csv` （GitHubからダウンロードしたデータ）

### ステップ 2: ローカルサーバーの起動

ターミナル（またはコマンドプロンプト）を開き、ファイルがあるフォルダへ移動して以下のコマンドを実行します。

```bash
# Python 3の場合
python -m http.server 8000

```

### ステップ 3: ブラウザで表示

サーバーが起動したら、ブラウザのURL欄に以下を入力してください。

`http://localhost:8000`

