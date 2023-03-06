快速入门
-----------
### 安装
```console
composer require free2one/hyperf-php-accessor
```
### 发布配置
```console
php bin/hyperf.php vendor:publish free2one/hyperf-php-accessor
```

### 通过`#[HyperfData]`注解原始类
除了PHP Accessor原有的注解外,需要额外使用该注解来标识其可被Hyperf<a href="https://hyperf.wiki/3.0/#/zh-cn/annotation?id=%e8%87%aa%e5%ae%9a%e4%b9%89%e6%b3%a8%e8%a7%a3">收集</a>.
```php
<?php
namespace App;

use Hyperf\PhpAccessor\Annotation\HyperfData;
use PhpAccessor\Attribute\Data;

#[HyperfData]
#[Data]
class Entity
{
    private int $id;

    private string $name;
}
```


