# むにむにGLBビューア 💕

GLB / glTF ファイルを、**解像度を落とさずそのまま**プレビューできる Android アプリです。
ファイルを再圧縮しないので、4096px のテクスチャも元のまま表示されます。

![正面](screenshots/front.png)
![お顔アップ](screenshots/face.png)

## ダウンロード

[**Releases ページ**](https://github.com/atomudorori-alt/MuniGLBViewer/releases) から最新の `MuniGLBViewer-v1.1.apk` をダウンロードしてください。

## インストール方法

1. APK ファイルをタップ
2. 「不明なアプリのインストール」を聞かれたら、このファイル（ブラウザ／ファイルアプリ）からのインストールを許可
3. インストール完了！

※ Android 8.0 以降対応。Play ストア外での配布のため、インストール時に確認画面が出ますが、このリポジトリで配布している公式ファイルです。

## 使い方

- 「GLBを開く」からファイルを選ぶだけ
- ファイルアプリで GLB を「アプリで開く」→ むにむにGLBビューア でも開けます
- 指でドラッグ： 回転 ／ ピンチ： 拡大・縮小 ／ 2本指ドラッグ： 移動
- 🔄 自動回転の ON/OFF
- 🎨 背景色の切り替え（ピンク／グレー／白／黒／水色）
- 📸 今の角度を写真として保存（ギャラリーの Pictures/MuniGLBViewer）

## 特長

- 元の GLB を再圧縮せず読み込むので、テクスチャは最大 4096px のまま（端末の WebGL 上限まで）
- 表示エンジン（Google model-viewer）をアプリ内に内蔵しているので **完全オフライン動作**、広告なし、データ収集なし

## 動作環境

- Android 8.0（API 26）以降
- WebView が最新に近い端末を推奨（Android System WebView / Chrome の更新）

## 開発について

- WebView + [model-viewer](https://modelviewer.dev/)（Apache License 2.0）で構築
- ソースコードは `app/src/main/` 以下（Java + HTML/JS）

## ライセンス

このアプリ自体のライセンスは未設定です（© らとれす / むにむに）。
同梱している model-viewer は Apache License 2.0 です。
