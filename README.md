# 環境構築

## nvm インストール
以下のコマンドでインストールを実行
```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```
以下のコマンドを実行するか、ターミナルを再起動
```sh
. ~/.nvm/nvm.sh
```
以下のコマンドで nvm のバージョンが確認できればインストールは完了
```sh
nvm -v
```
バージョンは、0.39.3である

## Node.js のインストール
以下のコマンドで最新の Node.js をインストール
```sh
nvm install --lts
```
Node.js , npm がインストールされているかどうかを確認
```sh
node -v
npm -v
```
バージョンは、Node.js は v20.15.0、npm は 10.7.0 である

## Vue.js の構築
以下のコマンドを実行し、プロジェクトを作成
```sh
npm create vue@latest
```

以下が出力され、選択肢を選ぶ
```sh
Need to install the following packages:
create-vue@3.10.4
Ok to proceed? (y) y


> npx
> create-vue


Vue.js - The Progressive JavaScript Framework

✔ Project name: … vue-project
✔ Add TypeScript? … No / Yes
✔ Add JSX Support? … No / Yes
✔ Add Vue Router for Single Page Application development? … No / Yes
✔ Add Pinia for state management? … No / Yes
✔ Add Vitest for Unit Testing? … No / Yes
✔ Add an End-to-End Testing Solution? › No
✔ Add ESLint for code quality? … No / Yes
✔ Add Prettier for code formatting? … No / Yes
✔ Add Vue DevTools 7 extension for debugging? (experimental) … No / Yes

Scaffolding project in 

Done. Now run:

  cd vue-project
  npm install
  npm run dev

npm notice
npm notice New minor version of npm available! 10.7.0 -> 10.8.1
npm notice Changelog: https://github.com/npm/cli/releases/tag/v10.8.1
npm notice To update run: npm install -g npm@10.8.1
npm notice
```

作成したプロジェクトに移動し、指示に従って依存関係をインストールし開発サーバーを起動
```sh
cd vue-project
npm install
npm run dev
```

## 参考
- [Macで「nvm」から「Node.js」をインストールする](https://tomozumi-system.com/2023/04/mac-nvm-node-js-install/)
- [Vue.js クイックスタート](https://ja.vuejs.org/guide/quick-start.html)

# 



