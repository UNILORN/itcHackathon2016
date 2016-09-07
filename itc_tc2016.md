# ITC TC Hackathon 2016

## 何する(案)
- 鉄道？(http://niisi.hatenablog.jp/entry/adventCalendar20151226)
- CTF？
- なんかやらん？
- フレームワーク
  - React
  - Lalavel
- ホテルの周辺情報・天気情報をまとめて見れるWebApp
  - 楽天トラベルAPI
  - お天気API
  - Google Map
  - 周辺の駅 etc...


## 何する（決定）
- ホテルの周辺情報・天気情報をまとめて見れるWebApp
  - 楽天トラベルAPI
  - お天気API
  - Google Map
  - 周辺の駅 etc...

## 何使う
- Laravel
- Vue.js
- RasPi 3(?)

## どう分ける

== 古賀 ==
- Laravelの環境構築
- 楽天トラベルAPIからホテルの緯度経度を取得する
- ホテルの緯度経度を元にお天気を取得する
- view（見た目） -> Vue.js

== 青木 ==
- ホテルの緯度経度を元にホテル最寄り駅を取得する
- 現在地（最寄り駅）からホテルの最寄り駅への経路
- View（見た目） -> Vue.js
