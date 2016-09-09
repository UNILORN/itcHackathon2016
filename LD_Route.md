# ルート

## 変更するファイル
__`/app/Http/route.php`__

## 記述方法
```php

Route::get('URL','Controller @ method');
Route::post('URL','Controller @ method');
Route::put('URL','Controller @ method');
Route::delete('URL','Controller @ method');

Route:resource('URL','Controller');

```

## 概要

基本Controller頼りである。

どのURLでどのHTTPメソッドでリクエストが来たら、どのControllerへ飛ばすかを設定するファイル。

**URL　→　HTTPメソッド　→　Controller**

のような形になる。

`GET` や `POST` の場合はメソッドの指定が必須だが、`RESOURCE` だとコントローラ側で操作をするため、いらない。
よって、コントローラでの作業がしやすくなる。
