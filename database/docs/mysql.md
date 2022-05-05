# MySQL

1. `$ mysql -uroot`   
passwordを設定していないからか、`mysql -uroot -p`と打つと以下のようなエラーが出る。  
`ERROR 1045 (28000): Access denied for user 'root'@'localhost' (using password: YES)`  

2. 
  ```mysql
  mysql> show databases;
  +--------------------+
  | Database           |
  +--------------------+
  | information_schema |
  | mysql              |
  | performance_schema |
  | studydb            |
  | sys                |
  +--------------------+
  5 rows in set (0.00 sec)
  ```

3.   `mysqlsampledatabase.sql`のような形で、webからダウンロードしてきたdatabaseを読み込ませる   
    `source ~/Downloads/mysqlsampledatabase.sql` で読み込み   
    `show databases;`で実際に追加されているか確認できる

  