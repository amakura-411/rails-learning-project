# 📘 Rails 学習用プロジェクト README

## 📝 概要

このリポジトリは、[Rails公式ガイド（Getting Started）](https://guides.rubyonrails.org/getting_started.html?utm_source=chatgpt.com) をもとに、
Ruby on Railsの基礎を学習するためのプロジェクトです。

RailsはRubyで書かれたWebアプリケーションフレームワークで、
「少ないコードで多くを実現できる」ことを目的に設計されています。([Ruby on Rails Guides][1])

---

## 🎯 学習目的

- Railsの基本構造を理解する
- MVC（Model / View / Controller）の概念を理解する
- CRUD操作（Create / Read / Update / Delete）を実装できるようになる
- RESTfulな設計の基礎を学ぶ

---

## 🧱 学習内容（このプロジェクトでやること）

Railsガイドに沿って、以下を順番に学びます：

1. Railsのインストール
2. 新規アプリケーションの作成
3. サーバー起動と動作確認
4. コントローラの作成
5. モデルの作成（Active Record）
6. データベースマイグレーション
7. CRUD機能の実装（記事投稿アプリ）
8. ルーティングの理解

👉 RailsではMVC構造により、

- Model：データとロジック
- View：画面表示
- Controller：処理の流れ
  を分離して開発します。([Ruby on Rails ガイド：体系的に Rails を学ぼう][2])

---

## 🛠️ 開発環境

- Ruby
- Ruby on Rails
- SQLite（開発用DB）

### セットアップ

```bash
# Railsインストール
gem install rails

# プロジェクト作成
rails new myapp

# ディレクトリ移動
cd myapp

# サーバー起動
rails server
```

ブラウザで以下にアクセス：

```
http://localhost:3000
```

---

## 📂 ディレクトリ構成（重要な部分）

```
store/
 ├── app/
 |     ─ models/        # データ（Active Record）
 |    ├── views/         # HTMLテンプレート
 |     ├── controllers/   # リクエスト処理
 |    config/
 |     └── routes.rb      # URLルーティング
 └── db
     └── migrate/       # DB変更履歴
```

---

## 🔑 重要な概念

### 1. Convention over Configuration

Railsは「設定より規約」を重視し、
決まりに従うことで設定を減らせます。([Ruby on Rails Guides][1])

---

### 2. Active Record

- データベースと連携する仕組み
- Rubyのオブジェクトとしてデータを扱える

---

### 3. Scaffold / Generator

Railsではコマンドで雛形を自動生成できる：

```bash
rails generate scaffold Article title:string body:text
```

---

## 🚀 今後やりたいこと

- 認証機能（ログイン）
- バリデーション追加
- UI改善（CSS / Tailwind）
- デプロイ（Render / Fly.io など）

---

## 📚 参考

- [Rails公式ガイド](https://guides.rubyonrails.org/getting_started.html?utm_source=chatgpt.com)
- [日本語版Railsガイド](https://railsguides.jp/getting_started.html?utm_source=chatgpt.com)

---

## ✍️ メモ

学習用なので、理解したこと・詰まったことをIssueやコメントに残す。

---

## 🙌 最後に

Railsは「全部入り」のフレームワークで、
フロント〜バックエンドまで一気に学べるのが強みです。([rubyonrails.org][3])

[1]: https://guides.rubyonrails.org/getting_started.html?utm_source=chatgpt.com "Getting Started with Rails"
[2]: https://railsguides.jp/getting_started.html?utm_source=chatgpt.com "Rails をはじめよう - Railsガイド"
[3]: https://rubyonrails.org/?utm_source=chatgpt.com "Ruby on Rails: Accelerate your agents with convention over ..."
