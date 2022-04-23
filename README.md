### 概要
Tinder風簡易マッチングアプリを作成して、<br>
Webアプリケーションを最後まで作りきることも目的としています。<br>
<br>
使用技術は下記になります。<br>
HTML・CSS・JavaScript・Rubyを使用<br>
データベースはPostgresql<br>
中間テーブルも使用しています。<br>
本番環境はherokuにデプロイしています。<br>
<br>

### 使用
1. マッチングしたユーザー間でチャットすることができる
2. トプ画の変更ができる

### 構成

### 更新予定
herokuの本番環境では画像の生成ができないという使用があるらしく、<br>
現状はバイナリデータをデータベースに保存して、それをviewに表示させる際にデコードしている形をとっています。<br>
これをAWS S3を使用する形式に変更する予定。

### 開発時の基本操作
- 本番環境(heroku)のポスグレ接続
  - heroku pg:psql

- local環境のポスグレ
  - psql -lで一旦確認
  - psql -h localhost -U hanaokayudai -d danger_match_development

