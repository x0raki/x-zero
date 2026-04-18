# x-zero

GitHub Pages で公開する、グループチャット向けの補助メモ置き場です。

## 最小構成

- `index.html`: 公開トップ
- `memo.md`: 人が編集しやすい Markdown 版
- `memo.txt`: ChatGPT に渡しやすいプレーンテキスト版
- `llms.txt`: AI 向けの簡単な案内

## GitHub Pages の有効化

1. GitHub のこのリポジトリを開く
2. `Settings` -> `Pages`
3. `Build and deployment` の `Source` を `Deploy from a branch` にする
4. Branch は `main`、Folder は `/ (root)` を選ぶ
5. 保存後、数分待つ

公開 URL は通常、`https://<user>.github.io/<repo>/` になります。

## 運用メモ

- 内容更新は `memo.md` と `memo.txt` を編集して push するだけ
- グループチャットでは `memo.txt` の URL を共有するのが単純
- 友人にも見せられる公開ページとして扱う
- プライベートな情報は、公開されても問題ない範囲にとどめる
- 秘密情報、個人情報、限定公開の URL は置かない
