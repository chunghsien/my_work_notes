### 設定 laravel-ide-helper ###
> 1. composer require barryvdh/laravel-ide-helper --dev
> 2. 編輯 ./config/app.php 文件
> 3. 加入以下設定至 'providers' => [... Barryvdh\LaravelIdeHelper\IdeHelperServiceProvider::class, ],
> 4. php artisan ide-helper:generate
> 5. _Ide_helper.php 生成表示執行成功