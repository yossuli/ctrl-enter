# ctrl-enter (仮名称)

ウェブサービス間で統一されていない送信キー(Enter, ctrl+Enter, alt+Enter)を統一するブラウザ拡張機能

ブラウザ拡張機能用Reactフレームワーク[Plasmo](https://www.plasmo.com/)を用いて開発

## 開発手順

### リポジトリのクローンとパッケージのインストール

Plasmo推奨のpnpmを使用しているため、まず初めにpnpmをインストールする

```sh
corepack enable
```

次にパッケージのインストール

```sh
pnpm i --frozen-lockfile
```

### 開発

```sh
pnpm notios
```

### 拡張機能のインストール

各ブラウザの拡張機能のインストール方法に従ってインストールする

以下はPlasmoのREADME.md

---

This is a [Plasmo extension](https://docs.plasmo.com/) project bootstrapped with [`plasmo init`](https://www.npmjs.com/package/plasmo).

## Getting Started

First, run the development server:

```bash
pnpm dev
# or
npm run dev
```

Open your browser and load the appropriate development build. For example, if you are developing for the chrome browser, using manifest v3, use: `build/chrome-mv3-dev`.

You can start editing the popup by modifying `popup.tsx`. It should auto-update as you make changes. To add an options page, simply add a `options.tsx` file to the root of the project, with a react component default exported. Likewise to add a content page, add a `content.ts` file to the root of the project, importing some module and do some logic, then reload the extension on your browser.

For further guidance, [visit our Documentation](https://docs.plasmo.com/)

## Making production build

Run the following:

```bash
pnpm build
# or
npm run build
```

This should create a production bundle for your extension, ready to be zipped and published to the stores.

## Submit to the webstores

The easiest way to deploy your Plasmo extension is to use the built-in [bpp](https://bpp.browser.market) GitHub action. Prior to using this action however, make sure to build your extension and upload the first version to the store to establish the basic credentials. Then, simply follow [this setup instruction](https://docs.plasmo.com/framework/workflows/submit) and you should be on your way for automated submission!
