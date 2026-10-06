# dokuritsu-sim

カリスタ株式会社 社内向け「独立開業 収支シミュレーション」。

- `src/index.html` … シミュレーションの本体（編集するのはこちら）
- `index.html` … 公開用。`src/index.html` をパスワードで暗号化したもの。自動で作られるので手で編集しない
- `.github/workflows/rotate-password.yml` … 毎月1日・15日 9:00（日本時間）にパスワードを作り直し、`index.html` を更新して Slack に通知する

ツールの中身を直したいときは `src/index.html` を差し替え、Actions タブから `rotate-password` を手動実行する。
