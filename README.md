# Alteryx Weekly Challenges

## 概要

このリポジトリは、Weekly Challenge の解答 Alteryx ワークフローを管理します。

---

## ディレクトリ構成

```text
.
├── 01_Workflows/         # メインのワークフロー (.yxmd)
├── 02_Macros/            # 共通利用するマクロ (.yxmc)
├── 03_Apps/              # 分析アプリ (.yxwz)
├── 04_Documentation/     # 仕様書・データ辞書
├── 05_Samples/           # テスト用サンプルデータ (Git管理対象)
├── .gitignore            # Alteryx用除外設定
└── README.md

```

## Index

- [Challenge499] (./04_Documentation/Challenge499.md)
---

## 開発・運用のルール

### 1. 相対パスの徹底

外部ファイル（CSVやExcel）を参照する場合は、必ずリポジトリ内の相対パスを使用してください。

> **Bad:** `C:\Users\Name\Desktop\Data\sample.csv`

> **Good:** `.\05_Samples\sample.csv`

### 2. コミット前のクリーンアップ

AlteryxのファイルはXML形式です。以下の点に注意してコミットしてください。

* **ツールの配置:** 意味もなくツールを動かすと、XML内の座標データが書き換わり、膨大な差分（Diff）が発生します。

### 3. バージョン管理のコツ

* 大きな変更を行う場合は、メインのワークフローを直接いじるのではなく、機能ごとに**マクロ化**して差分を局所化することを推奨します。

---

## 実行手順

1. このリポジトリを `git clone` します。
2. `01_Workflows/` 内のメインワークフローを開きます。
3. 「実行」ボタンをクリックします。

---

## メンテナンス・連絡先

* 作成者: [yoshi1968]

---