# Zotero Japanese AI Summarizer

⚠️ **警告: 開発中のベータ版** ⚠️
> 本プラグインは現在開発中であり、正常に動作しない可能性があります。  
> 実験的な機能の検証用としてのみ使用し、本番環境での使用は推奨されません。

---

Zotero用の日本語PDFファイルを要約するプラグインです。Google AI Studioを使用して、PDFから自動的に日本語の要約を生成し、Zoteroのノートとして追加します。

## 🚧 開発状況

現在、以下の機能を実装中です：
- [ ] PDFファイルからのテキスト抽出
- [ ] Google AI Studioを使用した要約生成
- [ ] Zoteroノートへの保存
- [ ] コンテキストメニューの表示

既知の問題：
- コンテキストメニューが正常に表示されない場合があります
- PDFテキストの抽出が不安定です
- API通信でエラーが発生する可能性があります

## 機能（予定）

- PDFファイルから自動的にテキストを抽出
- Google AI Studioを利用した日本語要約の生成
- 生成された要約をZoteroのノートとして保存
- コンテキストメニューからの簡単な操作

## インストール方法

⚠️ **注意: 現在のバージョンは開発者向けのテスト用です** ⚠️

1. [最新のリリース](https://github.com/TomokiMatsumoto992/zotero-jp-summarizer/releases/latest)から`zotero-jp-summarizer.xpi`をダウンロード
2. Zoteroを起動し、Tools → Add-ons を選択
3. 歯車アイコンをクリックし、「Install Add-on From File...」を選択
4. ダウンロードした.xpiファイルを選択してインストール

## 動作要件

- Zotero 7.0以上
- Google AI StudioのAPIキー
- インターネット接続

## 開発者向け情報

### ビルド方法

```bash
git clone https://github.com/TomokiMatsumoto992/zotero-jp-summarizer.git
cd zotero-jp-summarizer
zip -r [zotero-jp-summarizer.xpi](http://_vscodecontentref_/0) * -x ".*" -x "*.git*"
