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

## Response JSON

レスポンスを使うには、まず下のファイルを読みこむ

`use Illuminate\Http\Response;`

最後に値を返すときはこう書けばいい。

`return  response() -> json($name);`

## DataBase

ファイル読み込み

`use Illuminate\Support\Facades\DB;`

SELECT文（例）
`$results = DB::select('select * from users');`

- `DB::select()`
- `DB::insert()`
- `DB::update()`
- `DB::delete()`
- `DB::statement()`

## View呼び出し

`return view('{ファイル名}');`

Viewに値を渡したい時 -> `with`

- `return view('{ファイル名}') -> with('text',$text);`
- `return view('{ファイル名}',$text);`
- `return view('{ファイル名}') -> with($hash);`
