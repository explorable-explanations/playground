# Deep playground

Deep playgroundは、d3.jsを使用してTypeScriptで記述された、ニューラルネットワークのインタラクティブな可視化ツールです。新しいリクエストやバグの追跡にはGitHubのIssueを使用しています。皆様からのフィードバックをお待ちしております！

**貢献をご希望の場合は、[貢献ガイドライン](CONTRIBUTING.md)を必ずご確認ください。**

## 開発方法

可視化ツールをローカルで実行するには、以下のコマンドを実行してください：
- `npm i`: 依存関係のインストール
- `npm run build`: アプリをコンパイルし、`dist_ja/`ディレクトリに出力
- `npm run serve`: `dist_ja/`ディレクトリからサーバーを起動し、ブラウザでページを開く

開発中に編集・更新のサイクルを速くするには、`npm run serve-watch`を実行してください。
これにより、HTTPサーバーが起動し、TypeScript、HTML、CSSファイルが変更されるたびに自動的に再コンパイルされます。

## メンテナンス用

GitHub Pagesで日本語版を公開するには、以下の手順で`dist_ja/`を`gh-pages`ブランチへデプロイします。
デプロイ先リポジトリは`https://github.com/explorable-explanations/playground`です。
`gh-pages`ブランチが存在しない場合は、初回の`npm run deploy`で作成されます。

```bash
npm run build
git add .
git commit -m "Build Japanese GitHub Pages"
npm run deploy
```

GitHub Pagesの公開元は、`gh-pages`ブランチ作成後にリポジトリ設定で以下のように指定します。

- Source: Deploy from a branch
- Branch: `gh-pages`
- Folder: `/ (root)`

これはGoogleの公式製品ではありません。
