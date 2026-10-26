【シンプル漫画サイトひな形】

サイト構成：
- index.html：第1話・第2話・第3話の一覧。キャラ紹介などは入れていません。
- episode1.html / episode2.html / episode3.html：各話の漫画ページ。話ごとに個別URLになります。
- reader.js：横スワイプ、前後ページボタン、ページ数表示
- style.css：デザイン
- images/episode1 など：各話の画像を入れるフォルダ

GitHub Pagesで公開：
1. GitHubで新しいPublicリポジトリ（例：comic-site）を作る。
2. ZIPを解凍し、中のファイル・フォルダをリポジトリ直下へアップロードしてCommit changes。
3. Settings → Pages → Build and deployment → Sourceで「Deploy from a branch」を選ぶ。
4. Branchをmain、フォルダを/(root)にしてSave。
5. 数分後、Settings → Pagesに表示されるURLを開く。

漫画画像の差し替え：
- images/episode1/001.svg などのサンプル画像を、自分の画像に置き換えます。
- JPG/PNGを使う場合は、episode1.htmlなどの data-pages と img src のファイル名を同じ名前に変更してください。
- 各話HTML内の data-pages="画像1,画像2,画像3" に画像を読む順番で記入します。ページ数を増やすときは、カンマで追加してください。
- 新しい話を追加する場合は、既存のepisode HTMLをコピーして番号・タイトル・画像パスを変更し、index.htmlにリンクを1行追加します。
- 同じパスとファイル名で画像を更新すれば、基本的に各話のURLは変わりません。

注意：公開したサイトと漫画画像は誰でも閲覧できます。公開前に個人情報や公開したくない画像が入っていないことを確認してください。
