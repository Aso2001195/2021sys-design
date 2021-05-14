```uml
@startuml
ユーザー->webサーバー:商品を選択し確定
webサーバー->DBサーバー:商品の情報照会
DBサーバー->DBサーバー:商品の情報と一致する商品を検出
DBサーバー->webサーバー:一致した商品情報
activate ユーザー
alt 商品の在庫有
webサーバー->ユーザー:購入情報の提示
else 
webサーバー->ユーザー:完売と表示
end
deactivate ユーザー
@enduml
```
