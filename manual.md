#神社API"shmap"の使い方
-----

##概要
APIの名前やバージョン、提供元などの基本情報
APIの名称：shmap
APIのバージョン：version1
提供元：大竹啓之

-----

##提供する機能
・APIのビューアプリ
・APIをJSON形式で返す機能
・API入力フォーム
・DELTE機能

-----

##できる操作
GET：現在スプレッドシートに登録されている情報をJSON形式で表示する。
登録画面ではボタンで取得することができる。
PostmanなどのAPIクライアントなどで実行する場合は、`https://sheetdb.io/api/v1/f1gw7czp8ecyy/search?カラム名=検索したい情報`で情報を得ることができる。
PUT：スプレッドシートに登録されていない情報を登録することができる。
登録画面では、必要項目を入力後、ボタンで登録することができる。
PostmanなどのAPIクライアントなどで実行する場合は、`-GETを参照-f1gw7czp8ecyy?追加したいカラム名=登録したい情報`で情報を登録することができる。

DELETE：スプレッドシートに登録されている情報を削除することができる。
登録画面では、IDを指定することで任意のIDの行を削除することができる。

PostmanなどのAPIクライアントなどで実行する場合は、`https://sheetdb.io/api/v1/f1gw7czp8ecyy/ID/44`などで任意のIDの行の情報を削除することができる。

ビューアプリでは登録されている情報の検索・map表示を見ることができたり、スプレッドシートが見やすくなっている。