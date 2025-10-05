# AHP-GO 意思決定サポートアプリ
AHP-GO バージョン 1.0.0

## アプリ概要
Next.jsとSupabaseを用いたAHPによる意思決定サポートアプリです。

## サイトイメージ
![アプリ画面](/docs/アプリ画面.png)

## サイトURL
<未定>
- ゲストログイン
- ユーザID: test
- PassWord: pass_123

## 使用技術
- フロントエンド：Next.js XX.XX
- バックエンド：Next.js XX.XX
- データベース：Supabase
- デプロイ：Vercel
- バージョン管理：Git、GitHub
- テスト・デバッグ：DevTools（Safari）
- CI/CD：GitHub Actions（ESLint）

## 設計ドキュメント
[要件定義・基本設計・詳細設計の一覧_Googleスプレットシート](https://docs.google.com/spreadsheets/d/1V91GRCaYrSsLrcwU9XdJmRWXALMv9mCTmsPwTVjy8nw/edit?usp=share_link)

詳細設計時のワイヤーフレーム、E-R図、フローチャートの画像はdocsディレクトリに格納しています。[こちらからアクセス](./docs)

## 機能一覧
- 会員登録、ログイン機能(メールアドレス)
- AHP計算
- 評価基準と商品情報のAI補完
  - GPT 4o 
- 計算履歴保存

## テスト修正の設計及び実施書
[テスト修正の設計及び実施書_Googleスプレットシート]](./)

## アプリの改善案
[アプリの改善案_Googleスプレットシート]](./)

## 備考
[ESLintの実行結果_GitHub_Actions](./)

活用した生成AIとその用途
- ChatGPT: 要件定義、設計、各種リサーチ
- v0: アプリのモック作成

## リファクタリングの規則
-  2つ以上のファイルで使う、行数が10以上のUIコンポーネントはcomponentsディレクトリに移行
-  2つ以上のファイルで使う、行数が10以上の関数はlibディレクトリに移行
-  変数名で2つ以上の単語が入る場合は、「isPublished」のように二つ目以降の単語の頭を大文字にする
