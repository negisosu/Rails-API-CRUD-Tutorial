# 最低限のCRUD操作のRails API Tutorial

[この記事](https://zenn.dev/forge422/articles/d3ca59ed9e4521)をみながら作成しました。

## 起動
```aiignore
rails server
```
### 全件取得
```aiignore
curl http://localhost:3000/api/v1/blogs
```
### 1件取得
```aiignore
curl http://localhost:3000/api/v1/blogs/1
```
### 新規作成
```aiignore
curl -X POST -H "Content-Type: application/json" -d '{"blog": {"name": "New Blog Post"}}' http://localhost:3000/api/v1/blogs
```
### 更新
```aiignore
curl -X PUT -H "Content-Type: application/json" -d '{"blog": {"name": "Updated Blog Post"}}' http://localhost:3000/api/v1/blogs/1
```
### 削除
```aiignore
curl -X DELETE http://localhost:3000/api/v1/blogs/1
```
