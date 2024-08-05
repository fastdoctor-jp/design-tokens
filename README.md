# Design-tokens

このリポジトリは、Fast DOCTORのデザイントークンを管理するためのパブリックリポジトリです。
デザイントークンは、デザインシステムやスタイルガイドを一貫性のある形で実装するために使用されます。

## ディレクトリ構成

```plaintext
.
├── token
│   ├── tailwindTheme.js    # TailwindCSSテーマ設定ファイル
│   └── tokens.json         # デザイントークンの定義ファイル
├── package.json
└── README.md
```

## 使用方法

``` bash
npm install fastdoctor-jp/design-tokens
```

### TailwindCSSでの使用

TailwindCSSテーマをプロジェクトに適用するには、tailwind.config.jsファイルを次のように設定します。

``` js
const tailwindTheme = require('@fastdoctor-jp/design-tokens/token/tailwindTheme');

module.exports = {
  theme: {
    extend: {
        ...tailwindTheme,
        // その他の設定...
    },
  },
};
```
