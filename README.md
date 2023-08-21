# README

## 概要
- ヨガ予約管理システムの開発

## 画面遷移図
- https://www.figma.com/file/Mt5E8RM2O7Vo9Uan1kZpzo/%E7%84%A1%E9%A1%8C?type=design&node-id=0%3A1&mode=design&t=TpxVdMjVocDux4GP-1
- 雑すぎてすみません笑

## ER図
- https://dbdiagram.io/d/64e313b902bd1c4a5e1ba514


## 環境構築
- git clone git@github.com:k-suke39/yoga_events.git
- cd リポジトリ名
- bundle install
- rails db:create
- rails s

## 主な機能
- ログイン機能
- 新規登録機能
- イベント予約機能
- イベント一覧(確認)機能
- 管理者ログイン機能
- ユーザ管理機能(CRUD)
- イベント管理機能(CRUD)

## 開発Tips
### ブランチの切り方
ブランチの命名規則は下記に基づいてください
```
feature/issue番号/タスク名

ex. feature/133/create-login-form
```
コンフリクトを防ぐために、作業始める前は、**git pull origin main** を行った後に、**git merge 作業ブランチ**で他開発者の作業を取り込むようにしてください。

また、git push 直前にも上記の作業を行ってください。

### ビューについて
一旦見た目はあまり気にしなくていいです。
機能が全て実装されたらテンプレート用意するので、そちらを反映する方針でいこうと思います！

### lint
push前にrubocop(gem インストール済み)を使ってlintチェックをするようにしてください

### PRの作り方
テンプレを使ってください！レビュワーの部分を作間に設定、PR作成後該当のリンクをチャンネルに貼ってください！
```
## 概要
対応Issue (URL)

## 作業内容
作業内容

## 補足
```

## その他
1. sorceryに関してはテーブルを定義しているので、インストールは不要です。管理者画面担当の方は、roleのカラムを追加する必要があると思ってます。バリデーション関連も設定する必要あると思うので、そこらへんはコンフリクトを経験しながらやっていきましょう！
2. カレンダーの一覧に関しては、simple-calendarというgemを使って実装しようと思います。gemは入ってるのでこちらもインストール不要です！
- https://github.com/excid3/simple_calendar
- https://qiita.com/yamaday0u/items/5fa2ab42bdc685711709
- https://zenn.dev/yuma_rails/articles/00b6ea10b87ca5
- https://abillyz.com/moco/studies/551


どうなるかわかりませんが、協力して頑張りましょ〜！！！笑
