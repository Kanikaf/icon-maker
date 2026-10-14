# アイコンメーカー

画像の背景をブラウザ内で透過し、正方形（または丸）のアイコン用PNGを作るWebアプリです。
サーバー・APIキー不要、利用料無料。画像は外部に送信されません。

## 使い方
1. 画像をドロップ／クリックして選択／Ctrl+V で貼り付け
2. 切り抜き方法を選ぶ（写真は「AIで自動」、単色背景のイラストは「外側の背景色を消す」）
   - 白い塗りが消える場合は「輪郭で囲まれた内側は消さない」をオン
   - 細かい部分は「残すブラシ／消すブラシ」でプレビューをなぞって手直し
3. 余白・形（四角／丸）・背景（透明／色）・保存サイズを選ぶ
4. 「PNGを保存」

初回のみ切り抜き用AIモデル（約40〜170MB）をダウンロードします。2回目以降はブラウザのキャッシュから読み込みます。

## GitHub Pages での公開手順
1. GitHub で新しいリポジトリを作成（例: `icon-maker`）
2. `index.html` と `README.md` をアップロード（Add file → Upload files → Commit）
3. Settings → Pages → Source を「Deploy from a branch」、Branch を `main` / `(root)` にして Save
4. 1〜2分後、`https://<ユーザー名>.github.io/icon-maker/` で公開されます

## ライセンス上の注意
背景除去ライブラリ [@imgly/background-removal](https://github.com/imgly/background-removal-js) は AGPL-3.0 です。
このリポジトリのソースを公開しておけば、無料で利用・配布できます。
