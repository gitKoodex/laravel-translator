# laravel-translator
add some translator to laravel

# INSTALATION
copy translate.php file to your laravel project.
path to copy (your lavavel project path)/vendor/laravel/framework/src/Illuminate/Foundation
-  add this lines to your helper.php at same path
```
use Illuminate\Foundation\GoogleTranslate;
if(! function_exists('tarjome')){
    function tarjome(string $source='en',string $target = 'fa',string $text="hi"){
        return GoogleTranslate::translate($source, $target, $text);
    }
}
```

- at you view add this line of code

```
    {{tarjome('en','fa','hi')}}
    
```

- change en to your source lang. change fa to your target lang. change hi to your text that you want to translate.

## BASED ON
- laravel
- blade
- php
