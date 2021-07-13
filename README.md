

# 使用バージョン一覧

* Ruby version: 2.5.3
* mysql version: 8.0
* rails version: 5.2.6

# ディレクトリ構造

.  
├docker-compose.yml  
├dockerfile  
├initdb.d┐  
┃　　　　├init.sql  
├app-  
├bin-  
├config-  
 
# 環境構築手順

( *dockerは入っている前提です。* 入ってない場合はダウンロード →https://www.docker.com/)

$ git clone  
↓  
$ docker-compose build　　　　　　　　　　　　# コンテナをビルド  
↓  
$ docker-compose -d up　　　　　　　　　　　　# コンテナの一斉起動  
↓  
$ docker-compose run web rails db:create　　　# db作成  

# 参考にしたサイト

https://qiita.com/azul915/items/5b7063cbc80192343fc0
