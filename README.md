# x-zero

グループチャットの ChatGPT に見せたい前提情報を、GitHub Pages で公開しておくためのリポジトリです。

公式のカスタム指示は ChatGPT 側の設定欄に入れて、ここでは追加で渡したい短い前提だけを `memo.txt` に置く運用にしています。カスタム指示の全文は別ファイルに退避しています。

## 公開先

- トップ: `https://x0raki.github.io/x-zero/`
- 共有用: `https://x0raki.github.io/x-zero/memo.txt`
- 人が読む用: `https://x0raki.github.io/x-zero/memo.md`
- カスタム指示全文: `https://x0raki.github.io/x-zero/custom-instructions.txt`

## ファイル構成

- `index.html`: 公開トップ。用途と共有先を案内するページ
- `memo.txt`: ChatGPT にそのまま渡しやすい軽い補助メモ
- `memo.md`: 人が編集しやすい軽い補助メモの Markdown 版
- `custom-instructions.txt`: 公式欄に入れているカスタム指示の全文控え
- `custom-instructions.md`: 同内容の Markdown 版
- `llms.txt`: AI 向けの短い案内
- `.nojekyll`: GitHub Pages でそのまま静的配信するための設定

## まずどこを見ればいいか

- 補助メモを書き足したいとき: `memo.md`
- ChatGPT に渡る実際の軽いテキストを見たいとき: `memo.txt`
- 公式のカスタム指示全文を見たいとき: `custom-instructions.md` / `custom-instructions.txt`
- ページの見た目を変えたいとき: `index.html`

普段いじるのは、基本 `memo.md` と `memo.txt` だけで十分です。

## GitHub初心者向けの編集方法

GitHub の画面だけで編集できます。アプリやコマンドは不要です。

1. このリポジトリを GitHub で開く
2. 編集したいファイルを開く
3. 右上あたりの鉛筆マーク `Edit this file` を押す
4. 文章を書き換える
5. 下の `Commit changes...` を押す
6. 数分待って `https://x0raki.github.io/x-zero/memo.txt` を見て反映を確認する

初心者向けのおすすめはこれです。

1. まず `memo.md` を開く
2. 書きたい内容をそのテンプレに沿って直す
3. その内容を `memo.txt` にも反映する

## 何をどこに書くか

- 重要なこと、振る舞いの中核、長いルール: `custom-instructions.*`
- 軽い補足、近況、追加で伝えたい前提: `memo.*`
- デザインや案内文: `index.html`

この repo では、`memo.*` は「補助的な内容」だけに絞る想定です。

書く内容は、今の運用だとたぶんこの3枠が中心です。

- 全体に関わること
- らきむぼん（僕）に関わること
- 竜司（友人）に関わること

## md と txt の同期ルール

- `md` と `txt` は内容をそろえておく
- どちらを先に編集してもよい
- 片方を変えたら、新しいほうの内容に合わせてもう片方も更新する
- 迷ったら、見出しつきで読みやすく直しやすい `md` を先に触る
- 最後に `md` と `txt` を見比べて、内容がずれていないか確認する

## 更新するとき

1. `memo.md` と `memo.txt` を必要に応じて更新する
2. `index.html` の案内文とズレていないかだけ見る
3. カスタム指示全文を変えたときだけ `custom-instructions.*` も更新する
4. commit / push する
5. Pages 反映後に `memo.txt` の公開 URL を確認する

## 運用ルール

- 共有先は基本 `memo.txt`
- `memo.md` は人が確認しやすい、同内容の Markdown 版として使う
- 長い設定全文は `memo.txt` に入れず、`custom-instructions.*` に分ける
- `memo.*` には補助的な内容だけを書く
- 普段の内容は「全体」「らきむぼん」「竜司」の3枠で整理すると見やすい
- `md` と `txt` は、どちらか新しいほうに合わせて内容をそろえる
- 友人にも見せられる公開ページとして扱う
- プライベートな情報は、公開されても問題ない範囲にとどめる
- 個人情報、機密情報、限定公開 URL、内輪だけの事情は置かない

## GitHub Pages

まだ未設定なら、GitHub の `Settings -> Pages` で次を選びます。

1. `Build and deployment` の `Source` を `Deploy from a branch`
2. Branch を `main`
3. Folder を `/ (root)`

保存後、数分で `https://x0raki.github.io/x-zero/` に反映されます。
