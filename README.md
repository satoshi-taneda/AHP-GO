## AHP-GO - 意思決定サポートアプリ
- AHP-GO バージョン 2.0.0　楽天APIを使用した商品検索機能の実装
- AHP-GO バージョン 1.0.0　AHPプロジェクト管理機能搭載

## アプリ概要
AHP-GOは、ユーザーが複数の候補（商品やサービス）を合理的に比較し、最適な選択を支援する意思決定サポートアプリです。
AHP（階層分析法）を用いて、ユーザーが自分の重視する基準（価格・デザイン・ブランドなど）を記入し構造的に行えます。

## 対応する課題とソリューション概要
差別化ポイント：広告なし・シンプルUI・AHP専用スコアリングを実装。楽天やAmazonのようなECとは異なり、「意思決定支援」に特化。

## サイトイメージ
![アプリ画面](/docs/HomePage.png)

## サイトURL
[https://ahp-go-app.vercel.app](https://ahp-go-app.vercel.app)
以下のユーザでゲストログイン可能です。
- ユーザID: q1dj1e527m@sute.jp
- PassWord: Test0804

## 使用技術
- フロントエンド：Next.js、React(React HooksまたはContext API)、Tailwind CSS
- バックエンド：Next.js
- データベース：Supabase
- デプロイ：Vercel
- バージョン管理：Git、GitHub
- テスト・デバッグ：DevTools（Safari）
- CI/CD：GitHub Actions（ESLint）
- API: GoogleOAuth、Supabase Auth、Rakuten Developers

## 設計ドキュメント
[要件定義・基本設計・詳細設計の一覧_Googleスプレットシート](https://docs.google.com/spreadsheets/d/1V91GRCaYrSsLrcwU9XdJmRWXALMv9mCTmsPwTVjy8nw/edit?usp=share_link)

詳細設計時のワイヤーフレーム、E-R図、フローチャートの画像はdocsディレクトリに格納しています。[こちらからアクセス](./docs)

## 機能一覧
- 会員登録・ログイン機能
  - メールアドレス
  - Google認証
- AHP実施
- AHP計算(総合評価の算出)
- 棒グラフ表示
- プロジェクト管理
  - 最終目標・評価基準・候補の作成
  - 最終目標・評価基準・候補の編集
  - 最終目標・評価基準・候補の削除
- 楽天APIを使用した候補(商品など)検索 

## テスト修正の設計及び実施書
[テスト修正の設計及び実施書_Googleスプレットシート](https://docs.google.com/spreadsheets/d/1l6FGZCC654AA0JGc9Yi5ejwNrD9lYrjsGLORNtGYA0Y/edit?usp=sharing)

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
