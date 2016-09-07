# コントローラ

まず新しいコントローラを作成するには、プロジェクトのディレクトリ内で、

`$ php artisan make:controller {コントローラ名}`

で**自動作成**してくれる。

## コントローラ構文

```php:controller.php

class {ControllerName} extends Controller{
  public function {Method}(){

  }
}
```
> このコードは自動生成されるのであまり気にしなくていい

## *Method*

| HTTPMethod  | URL               | Method    |
|:-----------:|:------------------|:---------:|
| GET         | /test             | `index`   |
| GET         | /test/create      | `create`  |
| POST        | /test             | `store`   |
| GET         | /test/{text}      | `show`    |
| GET         | /test/{text}/edit | `edit`    |
| PUT/PATCH   | /test/{text}      | `update`  |
| DELETE      | /test/{text}      | `destroy` |

## *コマンド*

```php:php
View::make();
DB::
```
などなど。

***

今日はここまで。
