# x-zero

グループチャットの ChatGPT に見せたい前提情報を、GitHub Pages で公開しておくためのリポジトリです。

今は「現在のカスタム指示」を公開メモとして置いています。共有するときは、基本的に `memo.txt` の URL をそのまま渡します。

## 公開先

- トップ: `https://x0raki.github.io/x-zero/`
- 共有用: `https://x0raki.github.io/x-zero/memo.txt`
- 人が読む用: `https://x0raki.github.io/x-zero/memo.md`

## ファイル構成

- `index.html`: 公開トップ。用途と共有先を案内するページ
- `memo.txt`: ChatGPT にそのまま渡しやすいプレーンテキスト版
- `memo.md`: 人が編集しやすい Markdown 版
- `llms.txt`: AI 向けの短い案内
- `.nojekyll`: GitHub Pages でそのまま静的配信するための設定

## 更新するとき

1. `memo.md` と `memo.txt` を必要に応じて更新する
2. `index.html` の案内文とズレていないかだけ見る
3. commit / push する
4. Pages 反映後に `memo.txt` の公開 URL を確認する

## 運用ルール

- 共有先は基本 `memo.txt`
- `memo.md` は人が確認しやすい、同内容の Markdown 版として使う
- 友人にも見せられる公開ページとして扱う
- プライベートな情報は、公開されても問題ない範囲にとどめる
- 個人情報、機密情報、限定公開 URL、内輪だけの事情は置かない

## GitHub Pages

まだ未設定なら、GitHub の `Settings -> Pages` で次を選びます。

1. `Build and deployment` の `Source` を `Deploy from a branch`
2. Branch を `main`
3. Folder を `/ (root)`

保存後、数分で `https://x0raki.github.io/x-zero/` に反映されます。
