# 概要

プログラミングスクールTECH::CAMPカリキュラムでの製作物です！<br>
my_blogは複数人で使用できるブログで、ログイン機能、マイページ、編集削除機能など、railsの基本的な機能が実装されています！

## アプリケーションの機能一覧
・ユーザー新規登録機能<br>
・ユーザーログイン・ログアウト機能<br>
・ブログ投稿機能<br>
.ブログ編集削除機能<br>
・マイページ機能<br>

## 使用技術一覧
|種別|名称|
|------|----|
|開発言語|Ruby(ver 2.5.1)|
|フレームワーク|Ruby on Rails(ver 5.2.4.1)|
|マークアップ|HTML,CSS(Sass)|
|データベース|MYSQL|

# DEMO
![demo](https://raw.github.com/wiki/itokeso/my_blog/gif/image.gif)

##  usersテーブル  
|Column|Type|Options|
|------|----|-------|
|name |string|null: false|
|e-mail|string|null: false|
|password|string|null: false|
### Association
- has_many :posts

## postsテーブル
|Column|Type|Options|
|------|----|-------|
|title|text|---|
|text|text|null: false|
|user_id|integer|null: false, foreign_key: true|
### Association
- belongs_to :user



