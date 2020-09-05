## アプリケーションの概要
楽器演奏に特化した投稿SNSサービス（ https://enjoybackmusic.com ）

## 技術的ポイント
- AWS EC2/RDSを用いたRails本番環境構築
- AWS ACMでSSL証明書を発行し、SSL化
- 独自ドメイン取得、使用
- Dockerを用いたRails開発環境構築
- CircleCIによる自動ビルド＆テスト
- RSpecでテスト記述
- Ajaxを用いた非同期処理（フォロー/未フォロー、お気に入り登録/未登録などの切り替え表示）
- Bootstrapによるレスポンシブ対応
- Rubocopを使用したコード規約に沿った開発
- 10のモデルをそれぞれ関連付けて使用


## アプリケーションの機能
- 録音した音声の投稿
- 音声の再生、一時停止
- フォロー
- お気に入り登録
- コメント
- メモ（ユーザー個人だけが参照できる）
- 通知（フォロー、お気に入り登録、コメントがあった場合）
- 検索（Ransackを使用）
- 投稿の並び順の切替（最新順、人気順）
- ページネーション
- ログイン
- ログイン状態の保持

## 環境
 ■フレームワーク

　Ruby on Rails

 ■インフラ

　AWS EC2, Docker

 ■データベース

　AWS RDS, PostgreSQL

 ■アプリケーションサーバー

　Puma

 ■Webサーバー

　Nginx