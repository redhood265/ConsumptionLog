# 【Rails 初期構築】

・Railsの「Welcome aboard」ページまで環境設定が完了している前提
・その後の作業をメモしていく

・コマンドを利用したview、model、controllerの作成

## controller

```txt
rails generate controller Welcome index
```

- コマンドの内容
  - rails generate controller => Railsのコマンド
  - Welcome => コントローラー名
  - index => コントローラー作成時にデフォルトで作成して欲しいメソッドを記載(index,show,new,edit等)

※メソッドを指定してコントローラを作成した場合、そのメソッドに紐づくviewも作成される
　上記の例だと、indexのメソッドの対応するviewのファイルが自動的に作成される

## model

Railsのモデルは、単数形の名前。対応するテーブル名は複数形

```txt
rails generate model Article title:string text:text
```

- コマンドの内容
  - rails generate model => Railsのコマンド
  - Article => モデル名
  - title:string text:text => モデルが保持するデータ名とそのデータ形式を記載 (例 title => データ名、string => データ形式)


・デフォルトで作成されるerb形式のviewをslimに変換
