# Deep playground

Deep playgroundは、d3.jsを使用してTypeScriptで記述された、ニューラルネットワークのインタラクティブな可視化ツールです。新しいリクエストやバグの追跡にはGitHubのIssueを使用しています。皆様からのフィードバックをお待ちしております！

**貢献をご希望の場合は、[貢献ガイドライン](CONTRIBUTING.md)を必ずご確認ください。**

## 開発方法

可視化ツールをローカルで実行するには、以下のコマンドを実行してください：
- `npm i`: 依存関係のインストール
- `npm run build`: アプリをコンパイルし、`docs/`ディレクトリに出力
- `npm run serve`: `docs/`ディレクトリからサーバーを起動し、ブラウザでページを開く

開発中に編集・更新のサイクルを速くするには、`npm run serve-watch`を実行してください。
これにより、HTTPサーバーが起動し、TypeScript、HTML、CSSファイルが変更されるたびに自動的に再コンパイルされます。

## メンテナンス用
本番環境へのプッシュ：`git subtree push --prefix docs origin gh-pages`

これはGoogleの公式製品ではありません。
