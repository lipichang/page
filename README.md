# pagination
数组分页,可定制样式,内置3种样式,稍微修改一下可使用与所有的情形下的数组分页

## Installation
Pagination is available on [Packagist](https://packagist.org/packages/lipichang/pagination).Just add this line to your `composer.json` file:

```json
"lipichang/pagination": "dev-master"
```

or run

```sh
composer require lipichang/pagination:dev-master
```
### Example

``` php
use Lipichang\Pagination;
$pagination = new Pagination($totalPage,['style' => 1,'simple'=>false,'allCounts'=>true,'nowAllPage'=>true,'toPage'=>true],['title' => 'shoes']);

//分页样式的渲染
$page = $pagination->render();
```

### Explanation
|  参数 |  类型 |  说明 |
| ------------ | ------------ |------------ |
| totalPage  | array  | 总页数  |
|  style | int  | 分页样式，可选值1,2,3  |
|  is_style | boolean  | 是否使用默认样式true是 false否 默认true  |
|  simple | boolean  |  true:简单的分页样式,false:复杂的分页样式 |
|  allCounts | boolean  |  显示总页数 |
| nowAllPage  | boolean  |  显示现在的页码 |
|  toPage |  boolean | 跳转页码的功能  |
|  query |  array | 分页其他查询参数  |

### Show

#### simple模式
![simple模式](https://i.loli.net/2019/05/22/5ce4b455bb5ee79418.png)
#### style = 1,2,3
![Image1 text](https://i.loli.net/2019/05/22/5ce4b4d734bd981604.png)

![Image1 text](https://img.mysourcify.com/2022/01/10/317a2985aefc8b1174b9e51918c0e365.png)

![Image1 text](https://i.loli.net/2019/05/22/5ce4b5023ab7654710.png)
#### allCount,nowAllPage,toPage模式
![Image1 text](https://i.loli.net/2019/05/22/5ce4b51192c2325030.png)