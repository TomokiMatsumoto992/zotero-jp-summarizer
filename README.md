# Zotero Japanese AI Summarizer

Zotero用の日本語PDFファイルを要約するプラグインです。Google AI Studioを使用して、PDFから自動的に日本語の要約を生成し、Zoteroのノートとして追加します。

## 機能

- PDFファイルから自動的にテキストを抽出
- Google AI Studioを利用した日本語要約の生成
- 生成された要約をZoteroのノートとして保存
- コンテキストメニューからの簡単な操作

## インストール方法

1. [最新のリリース](https://github.com/TomokiMatsumoto992/zotero-jp-summarizer/releases/latest)から`zotero-jp-summarizer.xpi`をダウンロード
2. Zoteroを起動し、Tools → Add-ons を選択
3. 歯車アイコンをクリックし、「Install Add-on From File...」を選択
4. ダウンロードした.xpiファイルを選択してインストール

## 使用方法

1. Google AI StudioのAPIキーを取得（[APIキーの取得方法](https://ai.google.dev/)）
2. Zoteroで要約したいPDFが添付されているアイテムを選択
3. 右クリックして「AIで日本語要約を作成」を選択
4. 初回実行時にAPIキーの入力を求められるので入力
5. 要約が生成され、ノートとして追加されます

## 動作要件

- Zotero 7.0以上
- Google AI StudioのAPIキー
- インターネット接続

## ライセンス

[MIT License](LICENSE)

## 開発者向け情報

### ビルド方法

```bash
git clone https://github.com/TomokiMatsumoto992/zotero-jp-summarizer.git
cd zotero-jp-summarizer
zip -r [zotero-jp-summarizer.xpi](http://_vscodecontentref_/0) * -x ".*" -x "*.git*"
